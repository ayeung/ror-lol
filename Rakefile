# Add your own tasks in files placed in lib/tasks ending in .rake,
# for example lib/tasks/capistrano.rake, and they will automatically be available to Rake.

require(File.join(File.dirname(__FILE__), 'config', 'boot'))

require 'rake'
require 'rake/testtask'
require 'rake/rdoctask'

require 'tasks/rails'



namespace :before_migrate do
  desc "Creates a file before migrations"
  task :create_file  => :environment do
    `touch before_migrate_test`
  end
end