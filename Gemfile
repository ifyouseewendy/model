source 'https://rubygems.org'
gemspec

gem 'rom', git: 'https://github.com/rom-rb/rom.git', branch: 'master'
gem 'rom-sql', git: 'https://github.com/rom-rb/rom-sql.git', branch: 'master'
gem 'rom-repository', git: 'https://github.com/rom-rb/rom-repository.git', branch: 'master'

unless ENV['TRAVIS']
  gem 'byebug', require: false, platforms: :mri
  gem 'yard',   require: false
end

gem 'hanami-utils', '~> 1.0.0.beta1', require: false, github: 'hanami/utils', branch: '1.0.x'

platforms :ruby do
  gem 'sqlite3', require: false
  gem 'pg',      require: false
  gem 'mysql2',  require: false
end

platforms :jruby do
  gem 'jdbc-sqlite3',  require: false
  gem 'jdbc-postgres', require: false
  gem 'jdbc-mysql',    require: false
end

gem 'simplecov',          require: false
gem 'coveralls',          require: false
gem 'rubocop', '~> 0.45', require: false
