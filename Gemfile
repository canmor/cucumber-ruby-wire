source "https://rubygems.org"

git_source(:github) { |repo| "https://github.com/#{repo}.git" }

gemspec

if ENV['CUCUMBER_RUBY_CORE']
  gem 'cucumber-core', path: ENV['CUCUMBER_RUBY_CORE']
elsif !ENV['CUCUMBER_USE_RELEASED_GEMS']
  gem 'cucumber-core', github: 'cucumber/cucumber-ruby-core', tag: 'v10.1.0'
end

if ENV['CUCUMBER_RUBY']
  gem 'cucumber', path: ENV['CUCUMBER_RUBY']
elsif !ENV['CUCUMBER_USE_RELEASED_GEMS']
  gem 'cucumber', github: 'cucumber/cucumber-ruby', tag: 'v7.1.0'
end

gem 'aruba', github: 'cucumber/aruba', tag: 'v2.0.0' # lock in v2 for staying with cucumber v7.x
