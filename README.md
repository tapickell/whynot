[![Gem Version](https://badge.fury.io/rb/whynot.svg)](http://badge.fury.io/rb/whynot)

# whynot

Why not?

## Installation

Add this line to your application's Gemfile:

    gem 'whynot'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install whynot

## Usage

`require 'whynot'`

#### Unconfident Code

Then you can become less confident about your code working. Whynot adds
`Kernel#maybe`, which takes a block, like so:

```ruby
maybe do |x,y|
  x,y = 1,2
  x+y
end
```

Sometimes it'll return 3, and sometimes `nil`. Because, why not?

If you would like your code to mostly or occasionally work, you use
`Kernel#mostly` and `Kernel#occasionally`, respectively.

#### Apathetic Code

Whynot also defines `Kernel#meh`, for when you really don't give a shit.

Sometimes it'll be `true`, sometimes `false`. But you don't care about that,
do you?

## Contributing

1. Fork it ( https://github.com/[my-github-username]/whynot/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
