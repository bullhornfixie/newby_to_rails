# Building my first app with Ruby on Rails 

- [x] Rails setup
- [x] Created new model via rails scaffold 
- [x] Changed default database from sqlite3 to postgres
- [ ] Install software to enable file uploads in Rails 

## Setup

* Install Homebrew - makes it easy to install and update software on Mac 
* Install Ruby Version Manager - manage different versions of Ruby 
* Install latest version of Ruby with RVM 
* gem install rails --no-document
* brew install yarn - yarn is a package manage for node.js 
* rails -v 
* rails new myapp 
* cd myapp
* rails server 
* Go to http://localhost:3000 in your browser, and you should see the ‘Yay! You’re on Rails!’ page.
* I now have have a working Ruby on Rails programming setup. 

## Scaffolding 

Scaffolding functionality in Rails refers to the auto-generation of a model, views and controller set 
for a single database. 

``
rails generate scaffold idea name:string description:text picture:string 
``

## Default database for Rails 

I discovered Rails uses sqlite3 as it's default database application. I then re-configured the code in config/database.yml, installed 'pg' gem, and then ran rails db:migrate. This setup my ideas table in the new default database. 

The below command was a useful visual on db migration status.

``
rails db:migrate:status
``





