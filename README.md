 # TWIG

 ## INITIALISATION DE TWIG

 -initialiser Composer dans le projet:
 
 composer init

 -repondre aux question (en laissant les valeurs par defaut)
 -charger twig avec compser: 
'''''''
 composer require twig/twig 
 ''''
 - inclure l'autoloader dans l'index.php:
 '''PHP 
 require 'vendor/autoloader.php'
'''


## Functionement de base

- charger un loader :
'''PHP

$twig = new Environment ($loader, [
    'debug' =>true,
    'cache' =>__DIR__ . '/cache' // mettre a la cache a false en develeppement pour que la page se recharge lors d une actualisation
]);

'''
-rendre un template : 
php
