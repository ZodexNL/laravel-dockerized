## Start up
- docker compose run --rm npm install
- docker compose run --rm composer dump-autoload
- docker compose run --rm artisan key:generate

- In the root folder remove ".example" from the ".env.example" file
- In the root/src folder remove ".example" from the ".env.example" file


## Follow up
When starting to work on project, run this commands:
- docker compose up -d --build nginx (first time)
- docker compose up -d nginx
- docker compose run --rm npm run dev

You are good to go. Goodluck with your project!

# Production
When going on production you need to make your own certificates.
Run your container like this:
- docker compose -f docker-compose.yml -f docker-compose.prod.yml up --build nginx


## Database
The database (mysql) is run from the docker container.