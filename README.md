## Start up
- docker compose run --rm npm install
- docker compose run --rm composer dump-autoload
- docker compose run --rm artisan key:generate

In the root folder remove ".example" from the ".env.example" file
In the root/src folder remove ".example" from the ".env.example" file


## Follow up
When starting to work on project, run this commands:
- docker compose up -d --build nginx (first time)
- docker compose up -d nginx
- docker compose run --rm npm run dev

You are good to go. Goodluck with your project!

## Database
The database (mysql) is run from the docker container.