# lighnting-out-heroku

A barebones Node.js app using [Express 4](http://expressjs.com/).

This application is to demonstrate the Salesforce Lightning Out feature.

Checkout the Salesforce repo: [SF Lightning Out](https://github.com/tiaanswart/sf-lightning-out)

## Pre-deployment steps

1. Make sure you follow the Post Deployment steps from [SF Lightning Out](https://github.com/tiaanswart/sf-lightning-out)
2. Use the Community URL you copied and replace the Community URL in: `views/partials/header.ejs`
3. Replace the Community URL with you Community URL `views/partials/lightning-out.ejs`

## Post-deployment steps

1. Make sure you add the Heroku URL to SF CORS `Setup -> CORS -> New`
2. Make sure you add the Heroku URL to SF CSP Trusted Sites `Setup -> CSP Trusted Sites -> New Trusted Site`

## Running Locally

Make sure you have [Node.js](http://nodejs.org/) and the [Heroku CLI](https://cli.heroku.com/) installed.

```sh
$ git clone git@github.com:tiaanswart/lighnting-out-heroku.git # or clone your own fork
$ cd lighnting-out-heroku
$ npm install
$ npm start
```

Your app should now be running on [localhost:5000](http://localhost:5000/).

## Deploying to Heroku

```
$ heroku create
$ git push heroku master
$ heroku open
```
or

[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

## CORS

CORS must be enabled in Salesforce as well as the Node.js app, best to develop in Safari with CORS disabled

## Documentation

For more information about Salesforce Lightning Out, see these articles:

- [Lightning Components Developer Guide](https://developer.salesforce.com/docs/atlas.en-us.lightning.meta/lightning/lightning_out.htm)
- [Idea Exchange: Lightning Components Anywhere / Everywhere](https://success.salesforce.com/ideaView?id=08730000000cJO9AAM)
