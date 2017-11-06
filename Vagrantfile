Vagrant.configure("2") do |config|

  # Ubuntu 14.04
  config.vm.box = "ubuntu/trusty64"

  # Create a private network at 192.168.33.10
  config.vm.network "private_network", ip: "192.168.33.22"

  # Share local 'www' folder with the apache webhtml folder
  config.vm.synced_folder "www/", "/var/www/html"

  # Shell bootstrap file
  config.vm.provision :shell, path: "vagrant.sh"

end
