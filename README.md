[![Gem Version](https://img.shields.io/gem/v/capistrano-rails-logs-tail.svg)](https://rubygems.org/gems/capistrano-rails-logs-tail)

# Capistrano::Rails::Logs

Tail logs from Ruby on Rails server.

## Installation

Add this line to your application's Gemfile:

    gem 'capistrano-rails-logs-tail'

And then execute:

    $ bundle

## Usage

1. Add `require 'capistrano/rails/logs'` in your `Capfile`.
2. Run any of the following tasks to tail your logs:

```
# defaults to role :app and shows 20 lines before
cap staging rails:logs
```

Or to specify a role and/or number of lines
```
# specify a different role as a first argument
cap staging rails:logs[worker_1]

# specify number of lines as a second argument
# default role (:app)
cap staging rails:logs[,100]
# or
cap staging rails:logs[worker_1,100]

# Remember to escape the comma and square brackets if you are using ZSH
cap production rails:logs\[worker_1\,1000\]
```

## Contributing

1. Fork it ( https://github.com/FindHotel/capistrano-rails-logs-tail/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
