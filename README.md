# LaTeXML-Ruby

[![Build Status](https://secure.travis-ci.org/authorea/LaTeXML-Ruby.png?branch=master)](http://travis-ci.org/authorea/LaTeXML-Ruby)
[![license](http://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/authorea/LaTeXML-Ruby/master/LICENSE)


A Ruby wrapper for the [LaTeXML](http://dlmf.nist.gov/LaTeXML/) LaTeX to XML/HTML/ePub converter.

Includes support for daemonized conversion runs, for additional performance, via the [latexmls](https://github.com/dginev/LaTeXML-Plugin-latexmls) socket server.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'latexml-ruby'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install latexml-ruby

## Usage

A hello world conversion job looks like:

```ruby
@latexml = LaTeXML.new

response = @latexml.convert(literal: "hello world")

result = response[:result]
messages = response[:messages]

```

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/Authorea/latexml-ruby.

The 0.0.1 release of the wrapper brings support for easy conversion of latex fragments, which only scratches the surface of LaTeXML's versatile conversion use cases. If you are interested in a different workflow that is not yet supported, we will be very happy to hear from you.

## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

