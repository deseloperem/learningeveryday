# How to install Laravel project via Composer


Download project zip file : https://github.com/laravel/laravel


## Install a project via Composer in Terminal
 
**check *Composer* and *PHP Artisan* are installed on your machine before running laravel installation**
 

In Terminal, hit this command line : 

$`composer create-project --prefer-dist laravel/laravel [yourProjectName]`

**When installation completed, make user that php artisan generate: key has executed properly.**

And then, move your example file to .env in the root folder.

$`'mv .env.example .env'`

>I also created `.env.example` file to share with the team. The developers in the team will refer to this env.example then modify as their preference. Except the API key.

Now you can see the .env file under the root folder. In the .env file, if you don’t have your api key , __**run the key generator again**__. 

$`php artisan key:generate`

> What is API KEY in laravel : 
> it’s salt for your hash method in your application so don’t change once you started development. 

## Setup Gulp.JS 
- localhost
- Livereload
- Browser Sync


