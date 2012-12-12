# Atwix PHPCS Magento Rules

A set of [PHPCS](http://pear.php.net/package/PHP_CodeSniffer) rules used by
atwix.com team when hacking Magento.

## Pre-Requisites

* [PHPCS](http://pear.php.net/package/PHP_CodeSniffer)

## Installation

### Short Version

Clone this repository into your PHPCS Standards directory, using the directory
name of `Atwix_Mage`

### Long Version

You need to know the directory of your PHPCS install, you can do this by opening
a command prompt and typing in the following:

    pear list-files PHP_CodeSniffer

You should see a load of lines looking like this:

    php    /usr/share/php/PHP/CodeSniffer/Reporting.php
    php    /usr/share/php/PHP/CodeSniffer/Sniff.php
    php    /usr/share/php/PHP/CodeSniffer/Tokens.php

So the PHPCS directory in this case is `/usr/share/php/PHP/CodeSniffer/`, which
means we need to clone this repository into the `Standards/Made` subdirectory like
so:

    git clone https://github.com/Atwix/phpcs-magento-rules /usr/share/php/PHP/CodeSniffer/Standards/Atwix_Mage

You can check the standard got installed by running `phpcs -i` which should show
you something like this:

    The installed coding standards are Atwix_Mage, MySource, Squiz, Zend, PHPCS and PEAR
