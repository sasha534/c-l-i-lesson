https://code.tutsplus.com/ru/tutorials/how-to-create-custom-cli-commands-using-the-symfony-console-component--cms-31274
# c-l-i-lesson

1) composer require symfony/console

#2) composer.json

{
    "require": {
        "symfony/console": "^4.0"
    }
}
#change:
{
    "require": {
        "symfony/console": "^4.0"
    },
    "autoload": {
         "psr-4": {
             "Console\\": "src"
         },
         "classmap": ["src"]
     }
}

#3) composer dump -o обновить автозагрузчик PSR4

#4) mkdir /bin/console.php
