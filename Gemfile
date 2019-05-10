# encoding: utf-8
source "https://rubygems.org"

gem "activesupport"
gem "json"
gem "unparser"
gem "mime-types"
gem "json_pure"
gem "rest-client"
gem "rubocop", platforms: :mri, groups: [:test, :local_development]
gem "addressable"
gem "ffi" # windows support

gem "reek"
gem "i18n"
gem "parallel" # 1.3.4 disallows 1.9.2
gem "rest-client"
gem "rainbow"

gemspec path: File.expand_path("..", __FILE__)

platform :jruby do
  group :jruby do
    gem "jruby-openssl"
  end
end

group :test, :local_development  do
  gem "pry"
  gem "pry-nav"
end

# Added by devtools
group :development do
  gem "rake"
  gem "yard", group: :yard
end

group :guard do
  gem "guard"
  gem "guard-bundler"
  gem "guard-rspec"

  # file system change event handling
  gem "listen"
  gem "rb-fchange" , require: false
  gem "rb-fsevent" , require: false
  gem "rb-inotify", require: false

  # notification handling
  gem "libnotify",               require: false
  gem "terminal-notifier-guard", require: false
end
