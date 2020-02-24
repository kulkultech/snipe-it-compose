# How to Use it

## Generate App key

```bash
docker-compose exec snipe-it php artisan key:generate
```

Notes:

Add that APP_KEY to your docker env-file (we left a placeholder for it in your starting docker env file, above). **Make sure to include the base64: prefix if it is given!** If you're not using an env-file, you will need to pass the APP_KEY as an environment variable to your docker container.

## Replace the App key place holder

Replace placeholder in `APP_KEY=<<Fill in Later!>>` with the key you get, don't forget to bring the **base64:** prefix.

## Running the app

After you set the key here is you can run the app

```bash
# run the app on detach mode
docker-compose up -d

# see the logs
docker-compose logs -f snipe-it # snipe-it
```

For more information see [this document](https://snipe-it.readme.io/docs/docker).
