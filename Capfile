require 'capistrano/setup'
require 'capistrano/deploy'
require 'capistrano/scm/git'
install_plugin Capistrano::SCM::Git
require 'capistrano/rbenv'
set :rbenv_type, :user
set :rbenv_ruby, '2.5.0'
require 'capistrano/rails'
require 'capistrano/puma'
install_plugin Capistrano::Puma
install_plugin Capistrano::Puma::Nginx
install_plugin Capistrano::Puma::Jungle
require 'capistrano/nginx'
require 'capistrano/upload-config'
require 'sshkit/sudo'

Dir.glob('lib/capistrano/tasks/*.rake').each { |r| import r }