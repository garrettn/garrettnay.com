## Deprecation Notice

This repo is no longer the source of my personal website. I've replaced it with a new one. The source of my website as it now stands is not currently available publicly, but it may be in the future. Thanks for visiting!

# garrettnay.com

This is the source code for my website, which is built with
[Hugo](http://gohugo.io/). You probably won’t ever need to use this repo in its
entirety, but if you want to see an how this particular hugo site is structured,
here you go!

[![Build Status](https://img.shields.io/travis/garrettn/garrettnay.com.svg?style=for-the-badge)](https://travis-ci.org/garrettn/garrettnay.com)
[![devDependencies Status](https://img.shields.io/david/dev/garrettn/garrettnay.com.svg?style=for-the-badge)](https://david-dm.org/garrettn/garrettnay.com?type=dev)
[![forthebadge](http://forthebadge.com/images/badges/uses-html.svg)](http://forthebadge.com)
[![forthebadge](http://forthebadge.com/images/badges/uses-css.svg)](http://forthebadge.com)
[![forthebadge](http://forthebadge.com/images/badges/uses-badges.svg)](http://forthebadge.com)

## Development

### Requirements

-   [Hugo binary installed](https://gohugo.io/getting-started/installing) and
    available in your `PATH` (I try to keep up with the latest version, but
    older versions might work)
-   [Node.js](https://nodejs.org) (I highly recommend a version manager like
    [n](https://github.com/tj/n) or [nvm](https://github.com/creationix/nvm))
-   [Yarn](https://yarnpkg.com/) (recommended) or npm (comes with Node)

If you don’t use Yarn, `yarn` can be replaced with `npm` in the commands below.

### Getting Started

Clone this repository:

```
git clone https://github.com/garrettn/garrettnay.com.git
```

Go into the directory and install dependencies:

```
cd garrettnay.com
yarn install
```

### Running the Development Server

```
yarn start
```

This will kick off the Hugo server. The site will now be served from
http://localhost:1313.

### Building the Site

```
$ yarn test
```

This command will building the site with Hugo. I chose to use the `test` command
because 1) it’s automatically run on Travis CI without any configuration, and 2)
it makes sense as a test because I want to see if the site successfully builds.

The site will be built in the `public/` directory.

## Licenses

The source code of this website is licensed under the
[MIT License](LICENSE.txt).

The content of this website is licensed under the
[Creative Commons Attribution-ShareAlike 4.0 International License](LICENSE-content.txt).
