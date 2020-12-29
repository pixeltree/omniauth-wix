# Omniauth::Wix

Wix Strategy for OmniAuth 2.0

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'omniauth-wix'
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install omniauth-wix

## Usage

Depends on https://github.com/omniauth/omniauth

Setup OAuth credentials at https://dev.wix.com/

Here's a quick example, adding the middleware to a Rails app in config/initializers/omniauth.rb:

Rails.application.config.middleware.use OmniAuth::Builder do
  provider :wix, ENV['WIX_APP_ID'], ENV['WIX_APP_SECRET']
end

Authenticate the user by having them visit /auth/wix

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/pixetree/omniauth-wix.

