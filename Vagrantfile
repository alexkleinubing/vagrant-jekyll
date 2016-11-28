Vagrant.configure("2") do |config|

  config.vm.hostname = "ak-jekyll"
  config.vm.box = "ubuntu/xenial64"
  config.vm.network "private_network", ip: "192.168.100.179"
  config.vm.network "forwarded_port", host: 4000, guest: 4000
  config.vm.synced_folder ".", "/var/www"
  config.vm.provider :virtualbox do |vb|
    vb.name = "ak-jekyll"
  end

  config.vm.provision :shell, path: "provision/jekyll-setup.sh", privileged: false

end
