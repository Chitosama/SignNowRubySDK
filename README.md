#### About SignNow
SignNow is a powerful web-based e-signature solution that streamlines the signing process and overall document flow for businesses of any size. SignNow offers SaaS as well as public and private cloud deployment options using the same underlying API. With SignNow you can easily sign, share and manage documents in compliance with international data laws and industry-specific regulations. SignNow enables you to collect signatures from partners, employees and customers from any device within minutes. 

This library simplifies integrating SignNow's eSignature platform into your existing applications. It is still under development but we welcome you to try it and provide feedback at api@signnow.com.


#### API Contact Information
If you have questions about the SignNow API, please visit [https://help.signnow.com/docs](https://help.signnow.com/docs) or email [api@signnow.com](mailto:api@signnow.com).

## Installation

Add this line to your application's Gemfile:

    gem 'signnow-sdk'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install signnow-sdk

## Usage

Configure your Rails application to load your OAuth credentials when it starts:

   Add a YAML config file to /config

   ```
    development:
      # Your app's Oauth credentials provided by your account manager
      client_id: 0fccdbc73581ca0f9bf8c379e6a96813
      client_secret: 3719a124bcfc03c534d4f5c05b5a196b

      base_url: https://capi-eval.signnow.com
      signing_base_url: https://eval.signnow.com
   ```


   Add signnow.rb to /config/initializers with the following

   ```ruby
   require 'signnow'

   SN::Settings.load("#{::Rails.root}/config/signnow.yml", Rails.env)
   ```
   
# Additional Contact Information

##### SUPPORT
To contact SignNow support, please email [support@signnow.com](mailto:support@signnow.com).

##### SALES
For pricing information please call (800) 831-2050 or email [sales@signnow.com](mailto:sales@signnow.com).
