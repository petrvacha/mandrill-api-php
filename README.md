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
Download cacart.pem from [curl.haxx.se/docs/caextract.html](http://curl.haxx.se/docs/caextract.html).
```php
$yourKey = "yourSecretMandrillKey";
$absolutePathToCaCert = "/etc/ssl/certs/cacert.pem";
$mandrill = new Mandrill($yourKey, $absolutePathToCaCert);
```
