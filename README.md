\# 🎧 Spotify Profile Viewer



> A web app for visualizing personalized Spotify data



Built with a bunch of things, but to name a few:



\- \[Spotify Web API](https://developer.spotify.com/documentation/web-api/)

\- \[Create React App](https://github.com/facebook/create-react-app)

\- \[Express](https://expressjs.com/)

\- \[Reach Router](https://reach.tech/router)

\- \[Styled Components](https://www.styled-components.com/)



\## Setup



1\. \[Register a Spotify App](https://developer.spotify.com/dashboard/applications) and add `http://localhost:8888/callback` as a Redirect URI in the app settings

1\. Create an `.env` file in the root of the project based on `.env.example`

1\. `nvm use`

1\. `yarn \&\& yarn client:install`

1\. `yarn dev`



\## Deploying to Heroku



1\. Create new heroku app



&nbsp;  ```bash

&nbsp;  heroku create app-name

&nbsp;  ```



2\. Set Heroku environment variables



&nbsp;  ```bash

&nbsp;  heroku config:set CLIENT\_ID=XXXXX

&nbsp;  heroku config:set CLIENT\_SECRET=XXXXX

&nbsp;  heroku config:set REDIRECT\_URI=https://app-name.herokuapp.com/callback

&nbsp;  heroku config:set FRONTEND\_URI=https://app-name.herokuapp.com

&nbsp;  ```



3\. Push to Heroku



&nbsp;  ```bash

&nbsp;  git push heroku master

&nbsp;  ```



4\. Add `http://app-name.herokuapp.com/callback` as a Redirect URI in the spotify application settings



5\. Once the app is live on Heroku, hitting http://app-name.herokuapp.com/login should be the same as hitting http://localhost:8888/login

