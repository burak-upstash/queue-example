# Run the worker
php artisan queue:listen --queue=default

# Run the server
php artisan serve --verbose


# Prerequisites
Install php, composer, laravel

# Notes
- run the commands from the main directory

- app/Jobs/BigWork.php defines the Bigwork Jobs with /bigwork url

- app/Jobs/ExampleJob.php defines the Smallwork Jobs with /smallwork url

- Urls are defined in routes/web.php, /smallwork --> creates small job, /bigwork --> creates 32+kb job
 
### create .env file, and set the following with upstash config
```
REDIS_URL=redis://default:........

```


