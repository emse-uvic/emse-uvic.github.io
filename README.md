# README

## Running the Site Locally

### Non-Managed dependencies

Make sure you have ruby and the bundler gem installed.
See the links below for installation tutorials:

- [Ruby](https://www.ruby-lang.org/en/documentation/installation/)
- [Bundler](https://bundler.io)

### To start the site locally (for development purposes)

1. Clone this repository
2. Via the terminal (or command prompt, depending on your OS) `cd` into this repository.
3. Run `bundle install` to install all t he required dependencies listed in the `Gemfile`.
(This step only needs to be executed once, or when new dependencies are added to the Gemfile)
4. Run `bundle exec jekyll serve` to start the server locally.
5. In your browser, navigate to `http://127.0.0.1:4000` to preview the site.

## Caveats about Jekyll

These a couple of things to keep in mind while developing websites using Jekyll.
For a more comprehensive list, see the [official Jekyll tutorial](https://jekyllrb.com/docs/).

- Never make changes to anything in the `_site` directory.
This directory is generated dynamically by Jekyll from all the other files.
While it does contain the finished version of the site, changes made in this directory do not "stick".
- The server watches for changes and regenerates the `_site` directory on the fly.
This does not apply, however, to changes made to the `_config.yml` file.
If you make changes there, you will need to stop the bundle process and restart it again (See step 4).
