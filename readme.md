Run the following commands after cloning or forking:
===
Before anything at all, make sure you have RVM installed and that your `.rvmrc` file is set up with: 

	rvm --create use "ruby-1.9.3@baseline"

1. Don't forget to change `baseline` above to your appname (or whatever name you'd like)
2. make sure that when changing directory into the app top-level directory RVM will kick in, tell RVM not too. (choose 'N')
3. change .rvmrc
4. cd up then cd in again. (i.e. `cd ..` and then `cd <appname>`)
5. tell RVM to do it's magic (choose 'Y')

6. now change the name of the app (I use sublime and I find&replace for 'baseline' and replace it with the app name). **Note!!** it's important to note lower-case/upper-case, e.g. where it's Baseline it should stay with Capital B.


SET UP Upstream if you want to get changes from the baseline

	1. git remote add upstream https://github.com/sharonleon/baseline.git
	2. git fetch upstream
	3. git merge upstream/master 
	
now commit the changes fetched from Upstream.



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
