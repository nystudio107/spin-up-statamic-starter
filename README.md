# Spin Up Statamic starter

This is a starter kit for adding [Spin Up Statamic](https://github.com/nystudio107/spin-up-statamic) to your existing projects.

Spin Up Statamic allows you to create your own self-contained Statamic project complete site config, Antlers/Blade/Twig template files, assets, and devops shrink-wrapped with Docker, which you can distribute to others or use yourself.

Use it for:
- Spinning up a Statamic site in a browser in GitHub Codespaces
- Shipping a self-contained Statamic site to others
- Providing working example code & projects to others
- Spinning up a local Statamic project using someone else's `composer.json` for support

**N.B.:** This is _not_ intended to be a fully functional local development environment for client sites (there is no `buildchain`, for example).

## Adding Spin Up Statamic to an existing project

You can install the Spin Up Statamic scaffolding into an existing project by running the following command while inside that projects's root directory:

```shell
php please starter-kit:install nystudio107/spin-up-statamic-starter
```

**N.B.** Spin Up Statamic will only copy the `example.env` to `.env` if it doesn't exist already.

If you have an existing `.env` file, you will need to manually copy & paste the following lines into it:

```
# The port to start looking for unused ports from; it will increment until it finds an unused port
INITIAL_SERVER_PORT=8050
# Uncomment DEV_SERVER_PORT if you want to instead explicitly set the port
#DEV_SERVER_PORT=8050
APP_URL="http://localhost:${DEV_SERVER_PORT}/"
STATAMIC_CP_USER="demo@statamic.com"
STATAMIC_CP_PASSWORD="password"
```

Please see the [Spin Up Statamic](https://github.com/nystudio107/spin-up-statamic) repository for more information on using Spin Up Statamic.

## To Do

- Await orders from Jack

Brought to you by [nystudio107](https://nystudio107.com/)
