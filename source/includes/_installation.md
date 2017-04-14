# Installation

## Getting Set Up

1. Clone Carikotak repository to your hard drive with `git clone https://bitbucket.org/carikotak/carikotak.git`

2. `cd carikotak`

3. Inside the project folder run `composer install`

4. Install package dependencies with `yarn install` if you're using yarn or `npm install` is you're using npm

5. Copy `.env.example` file to `.env` and run `php artisan key:generate`

6. Setup Voyager Admin Panel with `php artisan voyager:install`

7. Setup Laravel Passport with `php artisan passport:install`

8. Run your project with `php artisan serve` then open `localhost:8000` from your browser

## Compile Assets

Carikotak use Laravel Elixir to compile every assets