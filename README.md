Really simple test of HTTParty and JRuby. Try this:

JRUBY_OPTS=--1.9 bundle exec irb
<from inside irb>
require "httparty"
response = HTTParty.get('http://twitter.com/statuses/public_timeline.json')
puts response.body, response.code, response.message, response.headers.inspect


