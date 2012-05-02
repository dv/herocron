HeroCron
========

Herocron is an easy way to use a free Heroku project with the daily cron, to call a webhook every day.

Usage
=====

$ git clone git@github.com:dv/herocron.git
$ heroku create --stack cedar
$ heroku addons:add cron
$ heroku config:add "WEBHOOK=http://hookscope.herokuapp.com/hook/herocron"
$ git push heroku master


Config
======

You can select a different method to use instead of the default GET:

$ heroku config:add METHOD=POST
