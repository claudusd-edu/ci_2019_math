# CI Math

require php >= 7.0 && < 8
require php extension : 
 * bcmath
 * zip
require composer

## Docker 

Build image : docker build -f docker/Dockerfile -t deployer-php .
Run App : docker run -it --rm -v $(pwd):/app -w /app deployer-php /bin/bash


## Run

run unit test : bin/phpunit

run integration test : bin/phpunit --group integration