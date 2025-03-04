# frozen_string_literal: true

source 'https://rubygems.org'

# Match ruby version in .ruby-version
ruby File.read('.ruby-version')

gem 'rails', '~> 7.1.0'

# Keeping old sprockets
# https://github.com/rails/sprockets-rails/issues/444#issuecomment-637817050
gem "sprockets", "<4"

gem 'bundler', '>= 2.3.10'

gem 'coffee-rails'
gem 'haml'
gem 'sassc-rails'

# API data
gem 'jsonapi-resources'
gem 'jsonapi-swagger'
gem 'rswag-api'
gem 'rswag-ui'

# CSS framework
gem "bootstrap", ">= 4.6.2"
gem 'material-sass', '4.1.1'

# Icons used by bootstrap/material-sass
gem 'material_icons'

# icons
gem 'font-awesome-sass'

gem 'terser'

gem 'oj' # Speeds up json

# planting and harvest predictions
# based on median values for the crop
gem 'active_median'
gem 'active_record_union'

gem 'flickraw'
gem 'jquery-rails'
gem 'jquery-ui-rails', github: 'jquery-ui-rails/jquery-ui-rails', tag: 'v7.0.0' # See https://github.com/jquery-ui-rails/jquery-ui-rails/issues/146

gem 'cancancan'                    # for checking member privileges
gem 'csv_shaper'                   # CSV export
gem 'gibbon', '~>1.2.0'            # for Mailchimp newsletter subscriptions

# Maps
gem 'leaflet-rails', '>= 1.9.2'
gem 'rails-assets-leaflet.markercluster', source: 'https://rails-assets.org'

gem 'pg'
gem 'ruby-units'                   # for unit conversion
gem 'unicorn'                      # http server

gem "comfortable_mexican_sofa", git: "https://github.com/restarone/comfortable-mexican-sofa.git"

gem 'active_utils'
gem 'sidekiq'

# Markdown formatting for updates etc
gem 'bluecloth'

# Pagination
gem 'will_paginate'
gem 'will_paginate-bootstrap-style'

# user signup/login/etc
gem 'devise'

# nicely formatted URLs
gem 'friendly_id'

# validates URLs
gem "validate_url"

# gravatars
gem 'gravatar-ultimate'

# For geolocation
gem 'geocoder'

# For easy calendar selection
gem 'bootstrap-datepicker-rails'

# DRY-er easier bootstrap 4 forms
gem "bootstrap_form", ">= 4.5.0"

# For connecting to other services (eg Twitter)
gem 'omniauth', '~> 1.3'
gem 'omniauth-flickr', '>= 0.0.15'
gem 'omniauth-twitter'

# Pretty charts
gem "chartkick"

# clever elastic search
gem 'elasticsearch', '~> 7.0.0'
gem 'searchkick'

gem "hashie", ">= 3.5.3"

gem 'rake', '>= 10.0.0'

# locale based flash notices for controllers
gem "responders"

# allows soft delete. Used for members.
gem 'discard', '>= 1.2'

gem 'xmlrpc' # fixes rake error - can be removed if not needed later

gem 'puma'

gem 'loofah', '>= 2.19.1'
gem 'rack-protection', '>= 2.0.1'

# Member to member messaging system
gem 'mailboxer', '>= 0.15.1'

gem 'faraday'

gem 'rack-cors'

gem 'icalendar'

# for signups as requested by email service
gem 'recaptcha'

# External APIs for data
gem "gbifrb"

gem "msgpack"

group :production do
  gem 'bonsai-elasticsearch-rails' # Integration with Bonsa-Elasticsearch on heroku
  gem 'dalli'
  gem 'memcachier'
  gem 'rails_12factor' # supresses heroku plugin injection

  gem 'scout_apm' # monitoring
end

group :development do
  gem 'better_errors'
  gem 'letter_opener'
  gem 'listen'
end

group :development, :test do
  gem 'bullet'                  # performance tuning by finding unnecesary queries
  gem 'byebug'                  # debugging
  gem 'capybara'                # integration tests
  gem 'capybara-email'          # integration tests for email
  gem 'capybara-screenshot'     # for test debugging
  gem 'database_cleaner'
  gem 'factory_bot_rails'       # for creating test data
  gem 'faker'
  gem 'haml-rails'              # HTML templating language
  gem 'pry'
  gem 'query_diet'
  gem 'rspec-activemodel-mocks'
  gem 'rspec-rails'             # unit testing framework
  gem 'rswag-specs'
  gem 'rubocop-rails'
  gem 'rubocop-rspec'
  gem 'webrat'                  # provides HTML matchers for view tests

  gem 'dotenv-rails'

  # cli utils
  gem 'haml-i18n-extractor', require: false
  gem 'haml_lint', '>= 0.25.1', require: false # Checks haml files for goodness
  gem 'i18n-tasks', require: false # adds tests for finding missing and unused translations
  gem 'rspectre', require: false # finds unused code in specs
  gem 'rubocop', require: false
end

group :test do
  gem 'axe-core-capybara'
  gem 'axe-core-rspec'
  gem 'codeclimate-test-reporter', require: false
  gem 'rails-controller-testing'
  gem 'selenium-webdriver'
  gem 'timecop'
  gem 'vcr'
end

group :travis do
  gem 'platform-api'
end

gem "percy-capybara", "~> 5.0.0"
