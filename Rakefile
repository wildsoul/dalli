require 'rake/testtask'
Rake::TestTask.new(:test) do |test|
  test.libs << 'test'
  test.pattern = 'test/**/test_*.rb'
end

Rake::TestTask.new(:bench) do |test|
  test.libs << 'test'
  test.pattern = 'test/benchmark_test.rb'
end

task :default => :test

task :test_all do
  system('rake test RAILS_VERSION="~> 2.3.0"')
  system('rake test RAILS_VERSION="~> 3.0.0"')
end