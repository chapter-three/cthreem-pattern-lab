# Pattern Lab for the CThreem Drupal 8 theme

This is a fork of the [Standard Edition for Drupal](https://github.com/pattern-lab/edition-php-drupal-standard), but modified to be used along side Chapter Three's [CThreem](https://github.com/chapter-three/cthreem) Drupal 8 theme.

The Standard Edition for Drupal gives developers and designers a clean and stable base from which to develop a Drupal compatible pattern library.

## Prerequistes

- [`composer`](https://getcomposer.org)

## First Time Install

Typically, you'll want to have Pattern Lab files placed inside the theme in a directory called `pattern-lab`. To do so (and it doesn't already exist), from the root of the theme directory:

```bash
composer create-project chapter-three/cthreem-pattern-lab pattern-lab
```

For convenience, it's nice to surface the `pattern-lab/source` directory since you'll be working in it often. Assuming you want a directory called `components` (and it doesn't already exist):

```bash
mv pattern-lab/source components
ln -s components pattern-lab/source
```

## Using It

After installing and committing, others cloning the repo need to run `composer install` to install dependencies.

## Helpful Commands

These are some helpful commands you can use on the command line for working with Pattern Lab.

### One line start

This will compile PL and watch for changes while running the local server:

    composer start

### Generate Pattern Lab

To generate the front-end for Pattern Lab type:

    php core/console --generate

### Start a server to view Pattern Lab

You can use PHP's built-in web server to review your Pattern Lab project in a browser. In a separate window type:

    php core/console --server

Then open [http://localhost:8080](http://localhost:8080) in your browser.

### Updating Pattern Lab

	composer update

## Other Documentation

- [Official Docs](http://patternlab.io/docs/index.html)
- [`pattern-lab/patternengine-twig`](https://github.com/pattern-lab/patternengine-php-twig)
- [`aleksip/plugin-data-transform`](https://github.com/aleksip/plugin-data-transform)
- [Twig templating language](http://twig.sensiolabs.org/documentation)
