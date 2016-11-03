# ClassyLlama OwlCarousel Module for Magento 2

This package makes the JavaScript library [OwlCarousel](https://github.com/OwlCarousel2/OwlCarousel2) available as an M2 module.

Note that this version of OwlCarousel is UMD compliant per [this fork](https://github.com/classyllama/OwlCarousel2).

## Installation Instructions

### Via Composer

Use this installation option if you want to require the OwlCarousel module with Composer. This is the typical installation method.
 
Run the following commands from the root directory of your Magento installation. 

```bash
composer require classyllama/module-owlcarousel:*
bin/magento module:enable --clear-static-content ClassyLlama_OwlCarousel
bin/magento setup:upgrade
bin/magento cache:flush
```

### Via Code Package
 
If you have not already obtained the zip or tar.gz file package, you can obtain it by visiting the "releases" section of the [public repository](https://github.com/classyllama/ClassyLlama_OwlCarousel) and choosing one of the formats under "Downloads" for the most recent release.

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