[![Bina Commerce](https://binacommerce.com/media/repo/banner-readme.png)](https://binacommerce.com/)

# About the project

A [Magento 2](https://business.adobe.com/products/magento/magento-commerce.html) implementation for my [Bina Commerce](https://binacommerce.com/) brand.

This little implementation allows you to reset a Magento database to its initial state.

## Installation

To proceed with the installation of your module, you need to go to the [document root of your Magento installation](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/docroot.html) and run the following commands:

```
composer require bina/module-reset-database
bin/magento setup:upgrade
bin/magento setup:di:compile
bin/magento setup:static-content:deploy
bin/magento cache:clean
bin/magento cache:flush
```
> **Note**
> To execute `bin/magento setup:static-content:deploy` you need to list all the languages of your store/s using the ISO-639 format. Also, if you are using a platform mode different than production, you need to execute the command using the `-f` flag: `bin/magento setup:static-content:deploy -f` (https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-static-view.html).

> **Note**
> The command `bin/magento cache:flush` is optional (https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-cache.html#config-cli-subcommands-cache-clean).

## Usage

In order to find documentation on the use and related issues, visit the [official page](https://binacommerce.com/reset-database.html) of this development.

## Author

- [LinkedIn](https://www.linkedin.com/in/cristian-marcelo-de-picciotto/) 
