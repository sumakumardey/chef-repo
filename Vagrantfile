Vagrant::Config.run do |config|
  config.vm.box = "lucid32"
   config.vm.provision :chef_solo do |chef|
     chef.cookbooks_path = "cookbooks"
     chef.add_recipe "redis"
     chef.add_recipe "mysql::server"
     chef.add_recipe "java"
     chef.add_recipe "jenkins::server"
     chef.log_level = :debug
  end 
end