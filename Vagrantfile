# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  #webgoat instance
  config.vm.define "OWASP-Box" do |ow|
    ow.vm.box = "owaspwebgoat/training"
    ow.vm.network "private_network", ip: "172.16.20.10",
      virtualbox__intnet: true
    ow.vm.provider "virtualbox" do |vb|
      vb.gui = false
      vb.cpus = 1
      vb.memory = 2048
    end
  end

  #dvwa instance
  config.vm.define "DVWA-Box" do |dvwa|
    dvwa.vm.box = "mmckinst/dvwa"
    dvwa.vm.network "private_network", ip: "172.16.20.20",
      virtualbox__intnet: true
    dvwa.vm.provider "virtualbox" do |vb|
      vb.gui = false
      vb.cpus = 1
      vb.memory = 1024
    end
  end

  #msf3 instance
  config.vm.define "MSF3-Box" do |msf|
    msf.vm.box = "rapid7/metasploitable3-win2k8"
    msf.vm.network "private_network", ip: "172.16.20.30",
      virtualbox__intnet: true
    msf.vm.provider "virtualbox" do |vb|
      vb.gui = false
      vb.cpus = 2
      vb.memory = 4096
    end
  end

  #kali instance
  config.vm.define "Kali-Box" do |kali|
    kali.vm.box = "kalilinux/rolling"
    kali.vm.network "private_network", ip: "172.16.20.121",
      virtualbox__intnet: true
    kali.vm.hostname = "kali"
    kali.vm.provider "virtualbox" do |vb|
      vb.gui = true
      vb.cpus = 2
      vb.memory = 2048
    end
  end
end
