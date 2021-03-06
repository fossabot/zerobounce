# Zerobounce
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fafrase%2Fzerobounce.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fafrase%2Fzerobounce?ref=badge_shield)

A ruby client for Zerobounce.net API.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'zerobounce'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install zerobounce

## Usage

```ruby
Zerobounce.configure do |config|
  config.api_key = 'key'
end

Zerobounce.validate(email: 'example@example.com')
resp = Zerobounce.validate(email: 'example@example.com', ip_address: '127.0.0.1')
resp.valid? # => true
```

## Development

After checking out the repo, run `bin/setup` to install dependencies.
Then, run `rake spec` to run the tests. You can also run `bin/console`
for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`.
To release a new version, update the version number in `version.rb`,
and then run `bundle exec rake release`, which will create a git tag for
the version, push git commits and tags, and push the `.gem` file to
[rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at 
https://github.com/afrase/zerobounce. This project is intended to be a safe,
welcoming space for collaboration, and contributors are expected to adhere
to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## License

The gem is available as open source under the terms of the
[MIT License](https://opensource.org/licenses/MIT).

[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fafrase%2Fzerobounce.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fafrase%2Fzerobounce?ref=badge_large)

## Code of Conduct

Everyone interacting in the Zerobounce project’s codebases, issue trackers,
chat rooms and mailing lists is expected to follow the 
[code of conduct](https://github.com/afrase/zerobounce/blob/master/CODE_OF_CONDUCT.md).
