VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.define :web do |node|
    node.vm.box = "chef/centos-6.6"
    node.vm.hostname = "dev-centos"
    node.vm.network :private_network, ip: "192.168.42.30"
    node.vm.network :forwarded_port, guest: 3000, host: 8080
    node.ssh.forward_agent = true

    node.vm.provider :vitualbox do |vb|
      vb.memory = 1024
      vb.cpus = 2
      vb.name = "ansible-centos"

    if Vagrant.has_plugin?("vagrant-cachier")
      node.cache.scope = :box
    end

    end
  end

  config.vm.provision :ansible do |ansible|
    ansible.playbook = "provision/playbook_vagrant.yml"
    ansible.inventory_path = "playbook/hosts"
    ansible.limit = "all"
    ansible.verbose = "v"
  end
end
