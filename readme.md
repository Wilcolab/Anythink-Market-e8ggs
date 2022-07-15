# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

After cloing the repo locally, make sure to have Docker installed. The easiest way would be with chocolatey:

```bat
choco install docker-desktop
```

Once it's installed, you will need to start the Docker Desktop app. It may prompt you to install an update to WSL following instructions from the Microsoft documentaion. Go ahead and install the update, if necessary, then click on the Restart button from the popup. Once Docker Desktop is up and running, you can now go into the repo's root folder on your computer and run:

```bat
docker-compose up
```

The above command will load Anythink's backend and frontend. It might take a while to start everything.

To make sure to the backend is running correctly, open the link [http://localhost:3000/api/ping]. You should get a message saying that it worked. Docker might still need a few more minutes to load the front-end, but once that is ready, open this link [http://localhost:3001/register] and then create a test user.
