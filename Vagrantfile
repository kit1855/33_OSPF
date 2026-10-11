# -*- mode: ruby -*-
# vim: set ft=ruby :

# Указываем зеркало для скачивания образов
ENV['VAGRANT_SERVER_URL'] = 'https://vagrant.elab.pro'

Vagrant.configure("2") do |config|

  # ============================================
  # 1. router1 (AlmaLinux 9)
  # ============================================
  config.vm.define "router1" do |r1|
    r1.vm.box = "almalinux/9"
    r1.vm.hostname = "router1"
    r1.vm.provider "virtualbox" do |v|
      v.memory = 2048
      v.cpus = 2
    end

    # Интерфейс для SSH с хоста
    r1.vm.network "private_network", ip: "192.168.50.10", adapter: 2, netmask: "255.255.255.0"

    r1.vm.provision "shell",
      run: "always",
      inline: <<-SHELL
        # This is VM for HW 33 OSPF
        # router1 provisioning placeholder
      SHELL
  end

  # ============================================
  # 2. router2 (AlmaLinux 9)
  # ============================================
  config.vm.define "router2" do |r2|
    r2.vm.box = "almalinux/9"
    r2.vm.hostname = "router2"
    r2.vm.provider "virtualbox" do |v|
      v.memory = 2048
      v.cpus = 2
    end

    # Интерфейс для SSH с хоста
    r2.vm.network "private_network", ip: "192.168.51.10", adapter: 2, netmask: "255.255.255.0"

    r2.vm.provision "shell",
      run: "always",
      inline: <<-SHELL
        # This is VM for HW 33 OSPF
        # router2 provisioning placeholder
      SHELL
  end

  # ============================================
  # 3. router3 (AlmaLinux 9)
  # ============================================
  config.vm.define "router3" do |r3|
    r3.vm.box = "almalinux/9"
    r3.vm.hostname = "router3"
    r3.vm.provider "virtualbox" do |v|
      v.memory = 2048
      v.cpus = 2
    end

    # Интерфейс для SSH с хоста
    r3.vm.network "private_network", ip: "192.168.52.10", adapter: 2, netmask: "255.255.255.0"

    r3.vm.provision "shell",
      run: "always",
      inline: <<-SHELL
        # This is VM for HW 33 OSPF
        # router3 provisioning placeholder
      SHELL
  end

end
