== README


Reflect (in your app's README): What is the best approach to storing environment variables (like a Weather Underground Key)? Why?

you put those keys in your .bash_profile, so that they are stored locally only. Therefore, when you push your code to someone else, they cannot see or use your key.
This protects your unique key from being overused or picked up by bots that steal and abuse things!



Reflect (in your app's README): Do you ever run migrations on the test database?

You can and do when need be. Say for example you make changes to your migration files, like add a new column or something,
you will need to re-migrate your test db as well as your prod db. I think rake db:migrate will migrate all, but sometimes you will not want to migrate all, and want to
test the development worked before your migrate the production one that users may be using.












This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...


Please feel free to use a different markup language if you do not plan to run
<tt>rake doc:app</tt>.
