source :rubygems

gem "activesupport", "~> 2.3.6.pre"
gem "tlsmail" if RUBY_VERSION <= '1.8.6'
gem "mime-types", "~> 1.16"
gem "treetop", "~> 1.4.8"

group :test do
  gem "ZenTest",    "~> 4.4.0"
  gem "rcov",       "~> 0.9.8"
  gem "rake",       "~> 0.8.7"
  gem "bundler"
  gem "rspec",      "~> 1.3.0"
  gem "diff-lcs"
  case
  when defined?(RUBY_ENGINE) && RUBY_ENGINE == 'rbx'
    # Skip it
  when RUBY_PLATFORM == 'java'
    # Skip it
  when RUBY_VERSION < '1.9'
    gem "ruby-debug"
  when RUBY_VERSION > '1.9' && RUBY_VERSION < '1.9.2'
    gem "ruby-debug19"
  else
    # Skip it
  end
end
