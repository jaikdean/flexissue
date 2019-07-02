# Symfony Flex/Composer Issue Reproducer

## Instructions

* Clone this repository.
* Run `composer install`.
* **The `composer.lock` file will be incorrectly updated with new versions of packages, equivalent to running `composer update`.**
* Run `git reset --hard` to reset the `composer.lock`.
* Run `composer install` again.
* **The `composer.lock` file will be respected this time, so packages will be downgraded to the correct versions.**
