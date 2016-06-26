# How to Install
## Before getting started
###Set up the environment
- Make your sublime text command global 
    >watch the youtube and run it in terminal : http://www.youtube.com/watch?v=NcIPANwBghU
    >or simply creat an alias to run the command : 
    `alias subl='"/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl"'`

- Install Composer
- Install Sequel Pro : A database manager on local and remote. http://www.sequelpro.com 
- Set up SSH KEY | https://help.github.com/articles/generating-an-ssh-key/ or https://confluence.atlassian.com/bitbucket/set-up-ssh-for-git-728138079.html
- Homebrew 
    _ Once Homebrew is installed, install Cask 
         `brew install caskroom/cask/brew-cask`

## Before getting started
###install Vagrant and Virtual Box

`brew cask install vagrant`
`brew cask install virtualbox`
`vagrant box add laravel/homestead`

####If you encounter SSL error*
*error no 50 or 60 : security setting*
`vagrant box add laravel/homestead http://atlas.hashicorp.com/laravel/boxes/homestead`
`vagrant box add --insecure -c laravel/homestead http://atlas.hashicorp.com/laravel/boxes/homestead`
*error no 54 : internet connection lose*
`vagrant up`

And then, choose virtual box as your provider in the progress of installation. 

## Finally, Let's Install Homestead
_missing_
> you can create a laravel project on your VM using composer command. 

## Connect to local database with Sequel Pro
### Create a database
- Open the application
- Create a folder : e.g. homestead
- Create a file : e.g. yourprojectname
- Enter local host information : refer to the .env file in your laravel project

### Migrate Laravel database 
In terminal, on your project folder on the VM, run php artisan. 
`php artisan migrate`





