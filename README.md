# Tr4n5l4te

Use Google Translate without an API key.

Like me, maybe you've found that Google makes it a pain to work with their API.
Tr4n5l4te gets around all that.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'tr4n5l4te'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install tr4n5l4te

## Usage

```ruby
translator = Tr4n5l4te::Translator.new
english_strings = %w(
  hello
  how are you
)
english_strings.each do |text|
  puts translator.translate(text, :en, :es)
end
# => hola
# => cómo estás
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/midwire/tr4n5l4te.

## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).