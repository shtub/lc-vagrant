Vagrant.configure(2) do |config|

  config.vm.box = "ubuntu/xenial64"
  config.vm.network "forwarded_port", guest: 80, host: 8080
  config.vm.provision :ansible do |ansible|
    ansible.playbook = "playbook.yml"
  end
#  config.vm.synced_folder "shared/", "/srv/shared"

end
