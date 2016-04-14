A sample Nova project. 

### About This Repo

This repo contains the started files for a sample [Nova](http://telescopeapp.org) project. Files included:

- `.meteor`: Meteor's own directory. Do not edit its contents, apart from `packages` and `release`.
- `.meteor/packages`: A list of the Meteor packages used by the app. 
- `.meteor/release`: The Meteor release used by the app. Changing this might break the app, but it's easily reversable.
- `.gitignore`: A list of files to be ignored by Git. 
- `app.json`: metadata used for Heroku deploys.
- `Dockerfile`: metadata used for Docker deploys.
- `scalingo.json`: metadata used for Scalingo deploys. 
- `sample-settings.json`: a sample settings file for your app. 

### Getting Started

[Install Meteor](https://www.meteor.com/install):

```
curl https://install.meteor.com/ | sh
```

Clone this repository locally:

```
git clone git@github.com:TelescopeJS/sample-project.git
```

Install the necessary NPM packages:

```
npm install
```

Then run the app with:

```
meteor
```

### Creating An Admin Account

The first account you create (via Log In > Register) will automatically be given admin rights. 

### Deleting Dummy Content

On its first run, Nova seeds the site with a few dummy posts. You can remove them by opening the console and calling `Meteor.call('removeGettingStartedContent')` while logged in as admin. 

### Configuring Settings

1. Stop your app. 
2. Copy `sample-settings.json` to a new `settings.json` file. 
3. Optionally, edit your `settings.json` file's contents.
4. Run your app with `meteor --settings settings.json`.

If you don't edit the sample settings provided, your app will simply be loaded with dummy settings (watch out for errors caused by dummy API keys). 

You can come back and change them at any time, but note that any category you remove will also need to then be deleted on the site. 

Note that `settings.json` will be gitignored by default. 

### One-Click Deploy

Deploy on Heroku:

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

Note: if you get a `$ROOT_URL, if specified, must be an URL.` error on deployment, double-check that you're providing the correct URL (typically `http://your-app-name-here.herokuapp.com`).

Deploy on Scalingo:

[![Deploy on Scalingo](https://cdn.scalingo.com/deploy/button.svg)](https://my.scalingo.com/deploy?source=https://github.com/TelescopeJS/sample-project/)

### Updating

You can update your app by running `meteor update`. If this upgrades Meteor to a non-compatible version, simply go back to the previous version in `.meteor/release`. 