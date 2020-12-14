# Mandrill API for PHP
This is a fork of an official library - [bitbucket.org/mailchimp/mandrill-api-php](https://bitbucket.org/mailchimp/mandrill-api-php).

It supports SSL verification.

## Installation
```
composer require petrvacha/mandrill-api-php-ssl
```

## Usage without SSL verification
```php
$yourKey = "yourSecretMandrillKey";
$mandrill = new Mandrill($yourKey);
```

## Usage with SSL verification
```php
$yourKey = "yourSecretMandrillKey";
$absolutePathToCaCert = "/etc/ssl/certs/cacert.pem";
$mandrill = new Mandrill($yourKey, $absolutePathToCaCert);
```
