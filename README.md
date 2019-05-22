# laravel app running in docker

You can watch the video tutorial at youtube:


### install composer dependencies
`docker run --rm -v ${pwd}/www/laravel:/app composer install`

### init laravel
`docker-compose exec app php html/artisan key:generate`

`docker-compose exec app php html/artisan optimize`

### common laravel commands
`docker-compose exec app php html/artisan migrate --seed`

`docker-compose exec app php html/artisan make:controller MyController`
