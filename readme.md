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
