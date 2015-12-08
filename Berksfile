source 'https://supermarket.chef.io'
"apt"

def opsworks_cookbook(name)
  cookbook name, github: 'lucjan-stepien-tabc/opsworks-cookbooks', branch: 'release-chef-11.10', rel: name
end

%w(dependencies opsworks_initial_setup ssh_host_keys ssh_users mysql::client ebs opsworks_ganglia::client apache2 opsworks_ganglia::configure-client ssh_users mysql::client agent_version deploy::default opsworks_shutdown::default ).each do |cb|
  opsworks_cookbook cb
end
