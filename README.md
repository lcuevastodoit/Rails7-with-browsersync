# Rails 7 with BrowserSync
This is a Rails 7 template, enabled with the `live reloading` of the web page when the code is changed.
Also this rails app have ready:
-  Bootstrap 5
-  Esbuild JSBundling
-  CSS Bundling
-  Auto transpiling any change in assets
-  Example Scaffold "Greetings"
-  Live reloading when view changes in code (localhost:3001)

## Requirements
- Ruby 3.0.3
- yarn
- nodejs

## Installation
1.  Clone the repository with
```
git clone https://github.com/lcuevastodoit/Rails7-with-browsersync.git
```
2.  cd to the recently cloned folder and be sure Ruby version is 3.0.3
    if not you can change it with `rvm use 3.0.3` or  `rbenv local 3.0.3` and after that you must reload your bash profile with `source ~/.bash_profile` or `source ~/.bashrc` or reload your zsh profile with `source ~/.zshrc`
    ```
    ruby -v
    # ruby 3.0.3p157
    ```
    In the case of `rbenv` maybe you need add these lines at the end of your `.bash_profile` or `.bashrc` or `.zshrc`
    ```
    export PATH="$HOME/.rbenv/shims:$PATH"
    eval "$(rbenv init -)"
    ```
3.  Foreman gem must be installed globally
    ```
    gem install foreman
    ```
4.  Install the dependencies with
    ```
    bundle install
    yarn install
    ```
5.  Run the migrations with
    ```
    rails db:migrate
    or
    bundle exec rails db:migrate
    ```
6.  run the web development server with
    ```
    ./bin/dev
    ```
7.  You will be accessing the project with three different ports in   your browser:
    -  http://localhost:3000   - original rails web access
    -  http://localhost:3001   - synced version (real time live reloading)
    -  http://localhost:3002   - BrowserSync all settings

#### More info

  -    [Ruby on Rails web page](https://rubyonrails.org/)
  -    [browsersyncing-rails gem github page](https://github.com/thelucid/browsersyncing-rails)
