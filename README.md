# ZR Media Recipe Installation Guide

To install the ZR Media Recipe, follow the steps below:

1. Open your terminal.
2. Navigate to your project directory. 
3. Ahead of running `composer require zr/RECIPE_NAME` - ensure the below has been added to the root `composer.json` **installer-paths**
    ```sh
    "web/recipes/custom/{$name}": ["type:drupal-recipe"]
    ```
4. Run the following command:

    ```sh
    ddev drush cr
    ddev drush recipe recipes/custom/zr-media-bundle
    ```

This command will execute the ZR Media Recipe installation.
