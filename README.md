# Rails 5.2 API with devise jwt boilerplate

## Getting started
### clone this repo
```
git clone https://github.com/nkhdo/rails_5.2_api_devise_jwt.git your_project_name
```
### edit `.ruby-gemset` (optional)
```
vim .ruby-gemset
```
### bundle
```
gem install bundle
bundle -j 4
```
### edit `config/database.yml`
Update to reflect your local env
```
vim config/database.yml
```
### Generate rails 5.2 master key
```
rm config/credentials.yml.enc # remove old credentials file, since there's no key to decrypt it
rails credentials:edit # generate new master.key and credentials file
```
Remember to add new entry to the credentials: `jwt_secret`, we need this for devise jwt part. To generate a random key, you can use `rails secret`
### Setup database
```
rails db:setup
```
### Start server
```
rails s
```
You are good to go ^_^

