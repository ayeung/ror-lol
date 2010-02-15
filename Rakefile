# Add your own tasks in files placed in lib/tasks ending in .rake,
# for example lib/tasks/capistrano.rake, and they will automatically be available to Rake.

require(File.join(File.dirname(__FILE__), 'config', 'boot'))

require 'rake'
require 'rake/testtask'
require 'rake/rdoctask'

require 'tasks/rails'

namespace :deploy do
  desc "Creates a file before migrations"
  task :before_migrate do
    `touch before_migrate`
  end
  desc "Creates a file before symlink"
  task :before_symlink do
    `touch before_symlink`
  end
  desc "Creates a file before restart"
  task :before_restart do
    `touch before_restart`
  end
  desc "Creates a file after restart"
  task :after_restart do
    `touch after_restart`
  end
end