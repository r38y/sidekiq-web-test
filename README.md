I'm having trouble getting Rails to recognize the sidekiq web app as an
endpoint, even though doing nearly the same thing with resque seems to
work. Any ideas? This is on Ruby 1.9.3-p125. 

# Repeat results:

1. bundle install
2. rake routes - shows both apps
3. rails server
4. visit http://localhost:3000/resque -- see it works
5. visit http://localhost:3000/sidekiq -- see it doesn't work
6. Check out config/routes.rb - I tried adding .new to the sidekiq one,
   no dice.
