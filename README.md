```sh
rails new rails7_demo
cd rails7_demo
rails generate scaffold post title:string content:text
rails db:migrate
rails action_text:install
bundle
rails db:migrate
./bin/importmap pin local-time --download
rails g resource comment post:references content:text
rails db:migrate
rails g mailer comments submitted
rails test
```
