# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "centos/7"
  config.vm.network :forwarded_port, guest: 8080, host: 8880
  # Provisioning
  provision_cmd = "yum install wget -y; " \
    "wget -O /etc/yum.repos.d/jenkins.repo http://pkg.jenkins-ci.org/redhat/jenkins.repo; " \
    "curl --silent --location https://rpm.nodesource.com/setup_4.x | bash -; " \
    "rpm --import http://pkg.jenkins-ci.org/redhat/jenkins-ci.org.key; " \
    "yum install nodejs jenkins java-1.8.0-openjdk -y; "
  config.vm.provision :shell, :inline => provision_cmd
end
