# Simple docker for Rails with nginx
Simple docker rails with nginx

## Rails 4

Add `gem 'puma'` to `Gemfile`

## Rails 5

Don't need `config/puma.rb` because it has been already :smiley:


### Using

Build:
`docker-compose build`

Start:
`docker-compose up `

Migrate:
`docker-compose run --rm app bundle exec rake db:migrate`

Rebuild:

`docker-compose build && docker-compose stop && docker-compose rm && docker-compose up`

View containers:

`docker ps`
