Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-18.04"
   
  config.vm.network "forwarded_port", guest: 80, host: 8000

  config.vm.provision :shell, path: "provision.sh"
  config.vm.provision :shell, path: "bootstrap.sh", run: 'always'

end