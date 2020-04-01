# -*- mode: ruby -*-
# vi: set ft=ruby :

$script = <<SCRIPT
apt-get update -y
apt-get install -y flex bison build-essential csh openjdk-6-jdk libxaw7-dev
mkdir -p /usr/class/cs143
chown vagrant /usr/class
cd /usr/class/cs143
wget https://courses.edx.org/asset-v1:StanfordOnline+SOE.YCSCS1+1T2020+type@asset+block@student-dist.tar.gz -O student-dist.tar.gz
tar -xf student-dist.tar.gz
rm student-dist.tar.gz
ln -s /usr/class/cs143 ~vagrant/
echo 'export PATH=/usr/class/cs143/bin:$PATH' >> ~vagrant/.bashrc
SCRIPT


Vagrant.configure("2") do |config|
  config.vm.define "cs143" do |cs143|
    cs143.vm.box = "ubuntu/trusty32"
    cs143.vm.synced_folder "cs143", "/usr/class/cs143"
    cs143.vm.provision "shell", inline: $script
  end
end
