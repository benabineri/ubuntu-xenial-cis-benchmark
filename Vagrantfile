VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
config.vm.box = "ubuntu/xenial64"

  config.vm.provision "shell" do |s|
    s.inline = "apt-get install -y python"
  end

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "main.yml"
  end

end
