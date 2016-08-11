BuntoBot
========

[![Build Status](https://travis-ci.org/bunto/buntobot.svg?branch=master)](https://travis-ci.org/bunto/buntobot)

Listens for GitHub post-receive service hooks messages, runs bunto, and pushes the results back to GitHub. Designed to be run on Heroku to generate JSON representations of postdata for bunto-import.tk.

Usage
-----

1. `git clone https://github.com/bunto/buntobot.git`
2. `heroku create` or `heroku git:remote -a <project-name-on-heroku>`
3. Add resulting URL to Repo's settings!
4. Deploy to Heroku with `git push heroku master`!
5. `heroku config:set EMAIL=YOUR_EMAIL_ADDRESS`
6. `heroku config:set GH_USER=YOUR_GITHUB_USER_NAME`
7. `heroku config:set GH_PASS=YOUR_PASSWORD`

Will automatically fire on each commit.
