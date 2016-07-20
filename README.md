# ClassyLlama OwlCarousel Module for Magento 2

This package makes the JavaScript library [OwlCarousel](https://github.com/OwlCarousel2/OwlCarousel2) available as an M2 module.

Note that this version of OwlCarousel is UMD compliant per [this active pull request](https://github.com/OwlCarousel2/OwlCarousel2/pull/1048).

## Installation Instructions

### Via Code Package

Use this installation option on most sites intended for production use.
 
If you have not already obtained the zip or tar.gz file package, you can obtain it by visiting the "releases" section of this repository and choosing one of the formats under "Downloads" for the most recent release.

In the root directory of your Magento installation, create the following sub-directory path:
 
```
app/code/ClassyLlama/OwlCarousel
```

Copy all contents of the zip or tar.gz package into the newly created directory, and then run the following commands from the root directory of your Magento installation:

```bash
bin/magento module:enable --clear-static-content ClassyLlama_OwlCarousel
bin/magento setup:upgrade
bin/magento cache:flush
```

### Via Composer

Use this installation option if you want to require the OwlCarousel module with Composer. This is typically the case if you are doing active development on the module, or if you want to use Composer to manage future module upgrades.
 
Run the following commands from the root directory of your Magento installation. (Note that for development, you should use "dev-develop" instead of "*" for the version constraint.)

```bash
composer config repositories.classyllama/owlcarousel git git@github.com:classyllama/ClassyLlama_OwlCarousel.git
composer require classyllama/module-owlcarousel:*
bin/magento module:enable --clear-static-content ClassyLlama_OwlCarousel
bin/magento setup:upgrade
bin/magento cache:flush
```