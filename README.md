A simple utility for running your Meteor applications in different environments.

### Install

Just include the start script in the root of your project. Make sure the start
file has excutable privileges.

```
$ chmod +x start
```

### Project Structure

```
todos/
  app/
  config/
    development/
      env.sh
      settings.json
    test/
    production/
  start
```

**Note: The app directory is your meteor application and the start bash file
goes in the root project folder.**

### Usage

```
$ start
```
Start your application in development, automatically executing the
config/development/env.sh file and loading config/development/settings.json into
Meteor.settings.

```
$ start --env production
```
Run the application in production mode.

```
$ start --checkout`
```
Run the application using a git checkout of meteor source code. Requires the
METEOR_SRC environment variable to be set.
