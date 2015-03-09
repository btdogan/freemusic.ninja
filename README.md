# Free Music Ninja website
[![Gitter](https://badges.gitter.im/Join Chat.svg)](https://gitter.im/FreeMusicNinja/freemusic.ninja?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![Circle CI](https://circleci.com/gh/FreeMusicNinja/freemusic.ninja.png?style=badge)](https://circleci.com/gh/FreeMusicNinja/freemusic.ninja)

This README outlines the details of collaborating on this Ember application.

## Requirements

This project requires [Node.js][].

The following global Node packages are required for development:

* [bower][]
* [ember-cli][]

Install the global dependencies like this:

```bash
$ sudo npm install -g bower ember-cli
```


## Installation

* `git clone` this repository
* `npm install`

If you run into trouble, try this magical command and then start over:

  npm clear cache

## Environment Variables

You'll need to set `API_URL` to `http://localhost:3200`.

## Running

* `ember server`
* Visit your app at http://localhost:4200.

## Running Tests

* `ember test`
* `ember test --server`

## Building

* `ember build`

For more information on using ember-cli, visit [http://www.ember-cli.com/](http://www.ember-cli.com/).

## Deployment

The following environment variables are required to deploy this website to Amazon S3:

* AWS_KEY
* AWS_SECRET

To build and deploy the website to S3:

```
ember deploy -e production  # deploy assets
ember deploy:list -e production  # list revisions
ember deploy:activate --revision "freemusicninja:$(git rev-parse --short HEAD)" -e production  # activate assets for current revision
```


[bower]: http://bower.io/
[ember-cli]: http://ember-cli.com/
[gulp]: http://gulpjs.com/
[node.js]: http://nodejs.org/
