source 'https://rubygems.org'

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end

gem 'dotenv-rails',   '~> 2.5'
gem 'faker',          '~> 1.9'
gem 'foreman',        '~> 0.85'
gem 'gruf',           '~> 2.7'
gem 'jbuilder',       '~> 2.5'
gem 'rails',          '~> 5.1.6.2'
gem 'pg', '>= 0.18', '< 2.0'
gem 'puma',           '~> 3.12'
gem 'settingslogic',  '~> 2.0'

group :development, :test do
  gem 'better_errors'
  gem 'binding_of_caller'
  gem 'bundler-audit'
  gem 'grpc-tools'
  gem 'sqlite3', '~> 1.3'
  gem 'byebug', platforms: [:mri, :mingw, :x64_mingw]
end

group :development do
  gem 'web-console', '>= 3.3.0'
  gem 'listen', '>= 3.0.5', '< 3.2'
  gem 'spring'
  gem 'spring-watcher-listen', '~> 2.0.0'
  gem 'pry'
end

group :test do
  gem 'rspec'
  gem 'rspec-rails'
end

gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]
