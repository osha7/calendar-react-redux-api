Terminal commands:

Building Backend:

cd Develompement
cd [folder-name]
rails new [app-name-here] --api -d=postgresql -T --webpack=react 
cd [app-name-here]
code .

in app terminal command: 
rails db:create
(run rails s and rails c to make sure app running and db connected)
(check postgres app to ensure you development db and test db and they are up and running)

front-end:

npm install -g npm
^^ newest version of Node Package Manager ^^

npx create-react-app [app-name-here]
cd [app-name-here]
code .

npm install
npm start

--------------cors---------------
in backend:

Gemfile:
uncomment:
<!-- gem 'rack-cors' -->

run: bundle install

config/initializers/cors.rb:
uncomment:

<!-- Rails.application.config.middleware.insert_before 0, Rack::Cors do
  allow do
    origins 'example.com'

    resource '*',
      headers: :any,
      methods: [:get, :post, :put, :patch, :delete, :options, :head]
  end
end -->


