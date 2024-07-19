# CLI Commands

| command                                                   | action                                                                                                                                                                                                                                     |
| :-------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `history`                                                 | Shows the commands you have used                                                                                                                                                                                                           |
| `history \| tail`                                         | shows the last ten commands<br><br>(note: the \ is not needed, it is due to Markdown using \| to separate columns in tables)                                                                                                               |
| `history \| grep XXX`                                     | filter the history to show only the commands containing `XXX`                                                                                                                                                                              |
| `composer global require laravel/installer`               | Install or update the `laravel new` command                                                                                                                                                                                                |
| `php -v`                                                  | displays the current version of PHP that is in the system path                                                                                                                                                                             |
| `node -v`                                                 |                                                                                                                                                                                                                                            |
| `npm -v`                                                  |                                                                                                                                                                                                                                            |
| `composer -V`                                             |                                                                                                                                                                                                                                            |
|                                                           |                                                                                                                                                                                                                                            |
| `laravel new`                                             | Interactive command that starts a new Laravel application. The name you give it will be the name of the folder created.                                                                                                                    |
| `laravel new APP_NAME`                                    | as above but creates the folder `APP_NAME`. We seriously suggest using the previous command as it provides better overall control.                                                                                                         |
| `php artisan make:model ModelName`                        | Creates a new model called `ModelName` in the Laravel application. Models MUST be named using Pascal Case and Must be the Singular version of the word. For example `Region` whereas the table created in the migration will be `regions`. |
| `php artisan make:migration create_pluralised_model_name` | Used to create the table migration for the model.<br><br>For example, `create_regions` would be used for the `Region` model.<br>                                                                                                           |
| `php artisan make:migration update_tablename`             | As before, but for updating a model's table.<br><br>When adding or removing fields from a model, name the migrations with `update`.                                                                                                        |
| `php artisan migrate:fresh`                               | Recreate the database structure, by first dropping all existing tables and then creating them again.                                                                                                                                       |
| `php artisan migrate:fresh --seed`                        | As above, but also run all the seed classes executed within the `DatabaseSeeder` class.                                                                                                                                                    |
| `php artisan db:seed --class=RegionSeeder`                | Run a single database seeder class, in this case the `RegionSeeder`.                                                                                                                                                                       |
| `php artisan make:class Classes/ApiResponseClass`         | Create a generic application class                                                                                                                                                                                                         |
| `php artisan route:list`                                  | List all your routes                                                                                                                                                                                                                       |
| `php artisan make:test BrowseRegionsTest --pest`          | Create a new Pest **feature** test                                                                                                                                                                                                         |
| `.vendor/bin/pest`                                        | Execute all the Pest tests                                                                                                                                                                                                                 |
| `composer require --dev knuckleswtf/scribe`               | Add the Scribe API Documentation package written and maintained by KnuckesWTF.                                                                                                                                                             |
| `php artisan vendor:publish --tag=scribe-config`          | Publish the scribe configuration file to the `config` folder.                                                                                                                                                                              |
| `composer require spatie/pest-plugin-test-time --dev`     |                                                                                                                                                                                                                                            |
| `php artisan scribe:generate`                             |                                                                                                                                                                                                                                            |
| `composer require laravel/sanctum`                        |                                                                                                                                                                                                                                            |
| `composer require --dev laravel/pint`                     |                                                                                                                                                                                                                                            |
| `php artisan publish`                                     | Provide an interactive method to publish (copy from the package's vendor folder) configuration, templates, or other components of a package for user modification.                                                                         |
| `php artisan make:model Region --all --api`               |                                                                                                                                                                                                                                            |
| `mkdir database/data`                                     |                                                                                                                                                                                                                                            |
| `mv ~/Downloads/regions.json database/data/`              |                                                                                                                                                                                                                                            |
|                                                           |                                                                                                                                                                                                                                            |
|                                                           |                                                                                                                                                                                                                                            |
|                                                           |                                                                                                                                                                                                                                            |