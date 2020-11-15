# Semantically versioned Rails views

## Installation

This is a demo Rails app, so just run the usual Rails commands to get up and running.

Clone the repo, then run `bundle` and `rails s` to start the server.

## Explanation

Check app/views/welcome/index.html.erb — the code is commented.

Essentially we have a list of view partials under _app/views/components_ and we want to load the best available version, given a constraint such as `~> 1.1.2` (following the Gemfile notation).

If it exists, we render it, otherwise we rescue the exception and display an error on the page.
