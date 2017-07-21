# Customising Chassis

This repository was created to demonstrate how you can commit a custom `config.yaml` into a repository to create a consistent WordPress development environment for your developers.

We take a default Chassis development environment and config it as follows:
1. We upgrade it from Php `7.0` to Php `7.1`
2. We change the default domain from [http://vagrant.local/](http://vagrant.local/) to [http://wordcamp.local/](http://wordcamp.local/).
3. We change the database name, username, password and prefix.
4. We alter the WordPress username, password and email address.
5. We add extensions for MailHog, XDebug, Tester, Composer and Grunt. 

## Usage

To get up and running with this customised Chassis example you'll want to do the follow in your terminal.
```
git clone https://github.com/Chassis/Chassis wordcamp
cd wordcamp
git clone --recursive https://github.com/BronsonQuick/chassis-wordcamp-demo.git content
vagrant up
```

## Areas of interest

1. [MailHog](http://wordcamp.local:8025)           - [MailHog](http://iankent.uk/project/mailhog/) catches the emails WordPress sends.
2. [Phpinfo](http://wordcamp.local/phpinfo.php)    - View your PHP settings.
3. [Xdebug](https://github.com/Chassis/Xdebug)     - [Xdebug](https://xdebug.org/) is installed and ready to be setup for usage in PHPStorm.
4. [Tester](https://github.com/Chassis/Tester)     - [Phpunit](https://phpunit.de/) has been setup so you can unit test your WordPress plugins and themes.
5. [Composer](https://github.com/Chassis/Composer) - [Composer](https://getcomposer.org/) has been setup on your development server.
6. [Grunt](https://github.com/Chassis/Grunt)       - [Grunt](https://gruntjs.com/) has been setup on your development server.

