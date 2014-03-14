# erlang-idna

A pure Erlang IDNA implementation.

## Quick start

    $ make deps
    ...
    $ make
    ...
    $ erl -pa deps/*/ebin -pa ebin
    ...
    1> idna:start().
    ...
    2> Domain = xmerl_ucs:from_utf8("www.詹姆斯.com").
    ...
    3> idna:to_ascii(Domain).
    ...

> Note: to update unicode data run the following command line:

    $ make dataupdate

## Useful references

[RFC3490](http://www.ietf.org/rfc/rfc3490.txt) (IDNA)

[RFC3492](http://www.ietf.org/rfc/rfc3492.txt) (Punycode)

[addressable](http://github.com/sporkmonger/addressable) (Ruby URI implementation)

[punycode4r](http://raa.ruby-lang.org/project/punycode4r/) (Ruby punycode implementation)

[Unicode Character Database](http://www.unicode.org/Public/UNIDATA/UCD.html)

[UAX #15](http://www.unicode.org/reports/tr15/) (Unicode Normalization Forms)
