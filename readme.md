Run the following commands after cloning or forking:
===
Before anything at all, make sure you have RVM installed and that your `.rvmrc` file is set up with: 

	rvm --create use "ruby-1.9.3@baseline"

don't forget to change `baseline` below to your appname (or whatever name you'd like)

-----
	
Install all gems

	Bundle install

Generate devise 

	rails generate devise:install
	
As per devise instructions:
Ensure you have defined root_url to *something* in your **config/routes.rb**.
For example:
it's waiting commented on routes.rb
	
	root :to => "home#index"
	
If you decide to take the add_default_MVC branch (it's in by default), you'll get default devised model and controller as well as `root:to => "home#index"` index action on the controller. You'll need to run `bundle exec rake db:migrate`

    bundle exec rake db:migrate
     
Now you should be able to start the rails server
	
	rails s

and access it via your browser
	
	localhost:3000



.

.

.

.

.


This rails app skeleton includes the followin gems:
===
	
### Debug: ###


---
pry-nav

pry-rails


### Authenticasion: ###
---

Devise   

see reference: [https://github.com/plataformatec/devise](https://github.com/plataformatec/devise#information)
