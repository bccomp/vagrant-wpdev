Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"  
  config.vm.network "forwarded_port", guest: 80, host: 8080
  config.vm.synced_folder "./wp-content", "/var/www/html/wp-content"
  config.vm.provision :shell, path: "./bootstrap.sh"
end
