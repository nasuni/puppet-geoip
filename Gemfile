source ENV['GEM_SOURCE'] || 'https://rubygems.org'

# rspec must be v2 for ruby 1.8.7
if RUBY_VERSION >= '1.8.7' and RUBY_VERSION < '1.9'
  gem 'rspec', '~> 2.0'
end

if RUBY_VERSION >= '1.9'
  gem 'rubocop'
end

# Get the gems of the declared version
puppet_ver = ENV.key?('PUPPET_VERSION') ? "#{ENV['PUPPET_VERSION']}" : ['>= 4.0']
facter_ver = ENV.key?('FACTER_VERSION') ? "#{ENV['FACTER_VERSION']}" : ['>= 1.7']

gem 'puppet', puppet_ver
gem 'facter', facter_ver

# Get the latest version of gems
gem 'rake'
gem 'metadata-json-lint'
gem 'puppetlabs_spec_helper'
gem 'puppet-lint'
gem 'rspec-puppet'
gem 'puppet-blacksmith'
gem 'parallel_tests'
gem 'rspec-puppet-facts'
gem 'puppet-strings'