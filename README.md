# Slim Framework 3 Starter Kit

Use this skeleton application to quickly setup and start working on a new Slim Framework 3 application.

This skeleton application was built for Composer. This makes setting up a new Slim Framework application quick and easy.

## Install the Application

Run this command from the directory in which you want to install your new Slim Framework application.

    php composer.phar create-project slim/slim-skeleton [my-app-name]

Replace `[my-app-name]` with the desired directory name for your new application. You'll want to:

* Point your virtual host document root to your new application's `public/` directory.
* Ensure `var/` is web writeable.

That's it! Now go build something cool.

## Test with PHP server ##

1. php -S localhost:8080 -t public
2. open http://localhost:8080/

## Use SQLite3 ##

To use sqlite3 rather than MySQL and seed the sqlite database, do the following:

1. cp app/settings.php.sqlite3 app/settings.php
2. mkdir db
3. sqlite3 db/slim_starter.sqlite < slim_starter.sqlite.txt
