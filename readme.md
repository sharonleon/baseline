Run the following commands after cloning or forking:
===
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
