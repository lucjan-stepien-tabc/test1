source 'https://supermarket.chef.io'
"apt"

def opsworks_cookbook(name)
  cookbook name, github: 'lucjan-stepien-tabc/opsworks-cookbooks', branch: 'release-chef-11.10', rel: name
end

%w(dependencies scm_helper mod_php5_apache2 ssh_users opsworks_agent_monit
   opsworks_java gem_support opsworks_commons opsworks_initial_setup
   opsworks_nodejs opsworks_aws_flow_ruby opsworks_postgresql apache2
   deploy mysql memcached).each do |cb|
  opsworks_cookbook cb
end
