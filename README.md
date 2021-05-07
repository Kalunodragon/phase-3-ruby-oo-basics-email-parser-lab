# Bonus: Email Parser Lab

## Learning Goals

- Build a class that uses an initialize method
- Practice using an attribute accessor macro to make an attribute available to a
  class's methods

## Description

You will write a program that, given a string of email addresses, parses that
string into an array.

Your class, `EmailAddressParser`, should take the string of addresses on
initialization. Instances should respond to a `parse` instance method that
parses the string into individual email addresses and returns them in an array.

I should be able to do this:

```ruby
email_addresses = "john@doe.com, person@somewhere.org"
parser = EmailAddressParser.new(email_addresses)

parser.parse
# => ["john@doe.com", "person@somewhere.org"]
```

**Note:** Your `EmailAddressParser` class should handle a list of email
addresses that are separated by either spaces _or_ commas. Additionally, the
`parse` method should only return unique addresses.

## Instructions

This lab is test-driven, so run the test suite to get started and use the test
output to get the program working.

**Hints:**

In order to get this lab passing, you will need to do some research into the
following topics:

- [Ruby's `String.split` method](https://www.rubydoc.info/stdlib/core/String:split)
- [RegEx](https://www.rubyguides.com/2015/06/ruby-regex/) - you'll use this to
  specify which characters to split the string on

## Resources

- [RegExr: Learn, Build, & Test RegEx](https://regexr.com/)