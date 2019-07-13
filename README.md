# README

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

* ******************* Add devise authentication **********************

* rails generate devise:install

* rails generate devise User

* uncomment Confirmable in the User migration file  and add :confirmable, inside user.rb file 

* rake db:migrate

* go to ApplicationController file , add below line
	before_action :authenticate_user!

* rails generate bootstrap:install static

* rails generate bootstrap:layout application

* rails generate devise:views:locale en

* rails generate devise:views:bootstrap_templates

* remove favicon link from application.html.erb if errors

* add below line to application.js
	//=require jquery
	//= require twitter/bootstrap

* add font-awesome
	gem "font-awesome-rails"
	bundle install

* add to application.css 
	*= require font-awesome