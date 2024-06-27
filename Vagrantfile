Vagrant.configure("2") do |config|

  config.vm.define "centos6"
  config.vm.box = "centos6"
  config.vm.box_url = "file:///D:/vagrant/centos6/package.box"
  config.vm.network "public_network", bridge: 'eth1', :adapter=>2 , ip: "192.168.1.103"
  config.vm.provision :shell, path: "pginstall.sh"


  config.ssh.host = '192.168.1.103'
  config.ssh.username = 'vagrant'
  config.ssh.password = 'vagrant'
  config.ssh.insert_key = false

end