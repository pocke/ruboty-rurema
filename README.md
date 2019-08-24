# Ruboty::Rurema

Search the Ruby Reference Manual via Ruboty.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'ruboty-rurema'
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install ruboty-rurema

## Usage

Ruboty is aware of `Klass`, `Klass#method`, `Klass.method`, and `Klass.#method`.

```
you    > @ruboty rurema Enumerable
ruboty > https://docs.ruby-lang.org/ja/latest/class/Enumerable.html 

you    > @ruboty rurema Object#then
ruboty > https://docs.ruby-lang.org/ja/latest/method/Object/i/then.html 

you    > @ruboty rurema JSON.parse
ruboty > https://docs.ruby-lang.org/ja/2.6.0/method/JSON/m/parse.html 

you    > @ruboty rurema Math.#sin
ruboty > https://docs.ruby-lang.org/ja/latest/method/Math/m/sin.html
```

Ruboty is also aware of free style text. It passes to https://docs.ruby-lang.org/ja/search/ as a query.

```
you    > @ruboty rurema 正規表現
ruboty > https://docs.ruby-lang.org/ja/2.6.0/doc/spec=2fregexp.html

you    > @ruboty rurema then
ruboty > https://docs.ruby-lang.org/ja/2.6.0/method/Object/i/then.html 
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/pocke/ruboty-rurema.


## License


These codes are licensed under CC0, except code that is copied from [bitclust](https://github.com/rurema/bitclust/blob/ba4b07e05ae41694e4930d7be355d32e9f17f396/lib/bitclust/nameutils.rb#L205-L208).

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png "CC0")](http://creativecommons.org/publicdomain/zero/1.0/deed.en)
