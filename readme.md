# Beer tank

## Project setup
```
git clone https://github.com/davidstar333/Laravel-Beers.git
```

```
composer install
```

```
npm install
```

### Configration
- Create a MySQL database for the project
    - mysql -u root -p
    - create database beer_tank;
    - \q
- Copy .env.example to .env
- Configure your .env file
    - APP_NAME=Beer Tank
    - DB_DATABASE=beer_tank
    - DB_USERNAME=root
    - DB_PASSWORD=null

```
php artisan key:generate
```

```
php artisan migrate
```

```
php artisan db:seed
```

### Compile vue.js files
```
npm run dev
```
or

```
npm run watch
```
### DEMO
- [DEMO](https://test.hopeisfar.live)