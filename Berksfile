source 'https://supermarket.chef.io'
cookbook "apt"

def opsworks_cookbook(name)
  cookbook name, github: 'lucjan-stepien-tabc/opsworks-cookbooks', branch: 'release-chef-11.10', rel: name
end

%w(apache2).each do |cb|
  opsworks_cookbook cb
end
