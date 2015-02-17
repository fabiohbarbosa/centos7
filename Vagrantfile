Vagrant.configure('2') do |config|
  # Droplet name in DigitalOcean
  config.vm.define "my-centos7" do |centos7|
  end

  config.vm.provider :digital_ocean do |provider, override|
    override.ssh.private_key_path = '~/.ssh/id_rsa'
    override.vm.box = 'digital_ocean'
    override.vm.box_url = "https://github.com/smdahlen/vagrant-digitalocean/raw/master/box/digital_ocean.box"

    provider.token = 'SEU_TOKEN'
    provider.image = 'centos-7-0-x64'
    provider.region = 'nyc2'
    provider.size = '512mb'
  end
end
