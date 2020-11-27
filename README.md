# dockerhero-php-8.0-fpm

https://github.com/johanvanhelden/dockerhero

## Available tags
- `latest`

## Building and publishing

Ensure you are logged in locally to hub.docker.com using `docker login` and have access to the hub repository.
(note: your username is used, not your email address).

```
$ docker build ./ --tag johanvanhelden/dockerhero-php-8.0-fpm:TAG
$ docker push johanvanhelden/dockerhero-php-8.0-fpm:TAG
```

Replace `TAG` with the tag you are working on.

## Development

If you want to test a new feature, create a new tag for it. This way, it can not introduce issues in the production image if something is not working properly.

Once it works, delete the custom tag and introduce it into `latest`

## Testing the image locally

```
$ docker-compose up --build
$ docker exec -it dockerhero-php-8.0-fpm-testing bash
```
