# TWENTY:ONE
**2.1.0**

a responsive theme made with ❤️

## Installation

- Download the repository on your local environment.
- Install nodejs and docker.
- Activate the premium font-awesome license with the following commands:

```bash

npm config set "@fortawesome:registry" https://npm.fontawesome.com/
npm config set "//npm.fontawesome.com/:_authToken" FDCB2249-245D-4135-8DCF-9D9771678396

```

- Install all dependecies with:

```bash

npm install

```
- When docker is fully setup, run the command to build the WordPress containers and images

```bash

docker-compose up -d

```
- Everything is done, now compile the theme for the first time with background refresh

```bash

npm run dev

```
- The final host is http://localhost:8008

## Notes

#### The directory of the theme is the same, where the plugins are located:

```bash

|- Local dev folder
|-- plugins
|--- advanced-custom-fields-pro
|--- ...
|-- twentyone-project-one
|-- twentyone-project-two
|-- ...

```

`wp-config.php`

```bash
define('ENVIRONMENT', 'local');
define( 'WP_DEBUG_DISPLAY', false );
define( 'UPLOADS', 'wp-content/media' );
define( 'WP_POST_REVISIONS', 3 );
define( 'IMAGE_EDIT_OVERWRITE', true );
define( 'WP_CACHE', false );
define('WPLANG', 'de_DE');
```
#### WordPress settings are located in `docker-compose.yml`.

#### phpMyAdmin Login Credentials - http://localhost:8088

```bash

WORDPRESS_DB_USER: wordpress
WORDPRESS_DB_PASSWORD: wordpress

```
#### Upload folder is generated in theme `media` folder.

## Authors

- [@mariostrebe](https://www.mariostrebe.com)

