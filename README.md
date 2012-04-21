I'm having trouble getting Rails to recognize the sidekiq web app as an
endpoint, even though doing nearly the same thing with resque seems to
work. Any ideas?

# Repeat results:

1. bundle install
2. rails server
3. visit /resque -- see it works
4. visit /sidekiq -- see it doesn't work
5. Check out config/routes.rb - I tried adding .new to the sidekiq one,
   no dice.
