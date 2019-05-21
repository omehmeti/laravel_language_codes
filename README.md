# laravel_language_codes
Laravel Language Codes by ISO Standard. Ready to deploy and seed automatically

These files will help you add Language Codes easily to your laravel project.

Project includes Names of the languages and 2 character codes of them. For ex: Language Name: Turkish, Code:tr

You need to follow 3 steps:

Step #1

Copy 2019_01_01_000000_create_languages_table.php file under your laravel project on migrations folder which can be found on 
/YOUR_LARAVEL_PROJECT_LOCATION/database/migrations

Step #2
Copy LanguagesTableSeeder.php file under your laravel project on seeds folder which can be found on 
/YOUR_LARAVEL_PROJECT_LOCATION/database/seeds

Step #3
Edit your DatabaseSeeder.php file as show on this project by adding LanguagesTableSeeder::class, line to public function run.
(DatabaseSeeder.php can be found on /YOUR_LARAVEL_PROJECT_LOCATION/database/seeds)

After these 3 steps you are done.

Now run the command to migrate the table to database on console under your project location:

$ php artisan migrate

Then run the command to insert the data and seed the database with language codes

$ php artisan db:seed --class=LanguagesTableSeeder

You are DONE!

Every suggestion is welcomed.
