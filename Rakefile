require "bundler/gem_tasks"
require "bundler/setup" # load up our gem environment (incl. local zanzibar)
require 'rspec/core/rake_task'
require 'zanzibar/version'

RSpec::Core::RakeTask.new(:test)

task :install_local do
  system "rake build"
  system "gem install ./pkg/zanzibar-#{Zanzibar::VERSION}.gem"
end
