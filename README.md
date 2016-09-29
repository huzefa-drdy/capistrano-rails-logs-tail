# Capistrano::Rails::Logs

Tail logs from Ruby on Rails server.

## Installation

Add this line to your application's Gemfile:

    gem 'capistrano-rails-logs-tail'

And then execute:

    $ bundle

## Usage

1. Add `require 'capistrano/rails/logs'` in your `Capfile`.
2. Run task to tail your logs: `cap staging rails:logs`

## Contributing

1. Fork it ( https://github.com/ayamomiji/capistrano-rails-tail-log/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
