[![Contact me on Codementor](https://cdn.codementor.io/badges/contact_me_github.svg)](https://www.codementor.io/amappuji?utm_source=github&utm_medium=button&utm_term=amappuji&utm_campaign=github)
[![Made in Indonesia](https://img.shields.io/badge/made%20in-indonesia-red?style=plastic&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAAAAXNSR0IArs4c6QAAAIRlWElmTU0AKgAAAAgABQESAAMAAAABAAEAAAEaAAUAAAABAAAASgEbAAUAAAABAAAAUgEoAAMAAAABAAIAAIdpAAQAAAABAAAAWgAAAAAAAABgAAAAAQAAAGAAAAABAAOgAQADAAAAAQABAACgAgAEAAAAAQAAAA6gAwAEAAAAAQAAAA4AAAAAoZe4PgAAAAlwSFlzAAAOxAAADsQBlSsOGwAAAVlpVFh0WE1MOmNvbS5hZG9iZS54bXAAAAAAADx4OnhtcG1ldGEgeG1sbnM6eD0iYWRvYmU6bnM6bWV0YS8iIHg6eG1wdGs9IlhNUCBDb3JlIDUuNC4wIj4KICAgPHJkZjpSREYgeG1sbnM6cmRmPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5LzAyLzIyLXJkZi1zeW50YXgtbnMjIj4KICAgICAgPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9IiIKICAgICAgICAgICAgeG1sbnM6dGlmZj0iaHR0cDovL25zLmFkb2JlLmNvbS90aWZmLzEuMC8iPgogICAgICAgICA8dGlmZjpPcmllbnRhdGlvbj4xPC90aWZmOk9yaWVudGF0aW9uPgogICAgICA8L3JkZjpEZXNjcmlwdGlvbj4KICAgPC9yZGY6UkRGPgo8L3g6eG1wbWV0YT4KTMInWQAAAf9JREFUKBV9Ur9PFFEQnvdjd8+DUwv0YrJhQ454PZXFAbEzdDZWZ2FiZcGfQ3Wdl1jQWF1FMBI0FrRG74LIhuM8chAIgd3bfbvznFnwIkad5Nt9b+Z9876ZeQIABMESyoSAgIS/mSRnSIgIgknwFGB5cWWl/bDR8F2lcoEoxVUIrLVgpcQsz1Vve7v/odNprgO818QrP6rX2y9XV/3K7KyBLHM42XVO0sJiQIHWZmlhwc92v7XXe906E4O5Ws13u12DOzuSbsMJiSlsTJZSepWKqc3XfOh1Ayai+h7m+eam42mNVggprm4pOAWPPlQTWlLjhmHOHCaC/fJZiv09gDjm7T9NOA5IY+QMndBzlRmw8wFg9R7tKM8ft02yULMsVWFHx1D5ugfaffwE7ItnYJcbAFNTADkpue7ohMT9UTSNNAX4+Anc1hvQqecCeB7ALRqjS+v/mFUarEtnySQfRZMhZqZwFHJIbjG/X3+SyIaGppWmyFRZLZVklCQqHifMpFlLpOHfAPs4dhHH5vwyUvfvlKTcer0W/jga9Ycnp87x6RnGSSJT6pzJsgK8HpOPY4ejE+dgMOxvtN6GPI5of3DU7Gy8a/sPqv7t6enc0erGk6PnhucXlwXp4HDYBBhE1GMrqIvct/LS81fB2XiMCW1+N67pLsnbaq0Vj5zqFz8BHc350tk1bDEAAAAASUVORK5CYII=)](https://github.com/made-in-indonesia/made-in-indonesia)

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
