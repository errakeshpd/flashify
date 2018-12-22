# Flashify

Animated colored flash messages to your website with few lines of code.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'flashify'
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install flashify

And then add to your application.css

    *= require flashify

And then add to your application.js

    //= require flashify



## Usage

Add this tag to your main layouts

```ruby
<% flash.each do |type, msg| %>
  <%= content_tag :span, msg, class: "flashify flashify-bottom-right #{type}" %>
<% end %>
```

## Customisation

Align the flash position by changing the class of span tag.

```css
flashify-top-right
flashify-top-left
flashify-top-middle
flashify-center
flashify-bottom-right
flashify-bottom-left
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/flashify. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

## Code of Conduct

Everyone interacting in the Flashify project’s codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](https://github.com/[USERNAME]/flashify/blob/master/CODE_OF_CONDUCT.md).
