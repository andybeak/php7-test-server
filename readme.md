# Readme

Example of using docker-compose to run a php7 test server for local development.

Place your project in the "src" directory.  Nginx is configured to treat src/public as the document root.

## Swapping PHP versions

Edit the supplied example nginx config file (./docker/nginx/default) and uncomment the line with the version
you want to pass requests to.  Make sure that the other version is commented.

    # fastcgi_pass    php7:9000;
    # fastcgi_pass    php5:9000;