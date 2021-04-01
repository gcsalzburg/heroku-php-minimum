# HEROKU PHP Minimum Setup

Very quickly setup new PHP instance on Heroku

Steps:

1. Login to Heroku and create new app at: https://dashboard.heroku.com/new-app

2. Clone this repo: 

	```bash
	git clone https://github.com/gcsalzburg/heroku-php-minimum.git
	```

3. In terminal for the cloned repo:

	Login:
	```bash
	heroku login
	```

	Run composer update (generators `vendor` and `composer.lock` files):
	```bash
	composer update
	```

	Add repo for new app:
	```bash
	heroku git:remote -a your-new-app-name
	```

	Push to Heroku
	```bash
	git push heroku main
	```

	Open on Heroku to check
	```bash
	heroku open
	```

## Helpful links

+  Rename heroku app
	```bash
	heroku apps:rename your-renamed-app-name
	```