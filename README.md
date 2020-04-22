# react-flask-heroku
Simple bootstrapping code to get you started with a React frontend and Flask backend ready to deploy to Heroku.

## Dependencies

python3, npm, Heroku CLI

## Setup

1. `pip3 install -r requirements.txt`
2. `npm install`

## Running Locally

1. `npm run build`
2. `heroku local`

The application will be running at http://localhost:5000.

## Deploying

First, create your app on Heroku. Then:

1. `heroku git:remote -a {YOUR_APP_NAME}`
2. `heroku buildpacks:set heroku/python`
3. `heroku buildpacks:add --index 1 heroku/nodejs`
4. `git push heroku master`

## Project Structure

* Flask server is at `app.py`
* React components in `src/`
