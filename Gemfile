source 'https://rubygems.org'

branch = ENV.fetch('SOLIDUS_BRANCH', 'main')
gem 'solidus', github: 'solidusio/solidus', branch: branch
gem 'solidus_auth_devise', github: 'solidusio/solidus_auth_devise', branch: 'master'

if branch == 'main' || branch >= 'v4.0'
  gem 'rails-controller-testing', group: :test
else
  gem 'rails_test_params_backport', group: :test
end

gem 'pg'
gem 'sqlite3'
gem 'mysql2'

gemspec
