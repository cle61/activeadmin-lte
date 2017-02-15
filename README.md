# ActiveAdmin::LTE

Theme for ActiveAdmin

![Alt text](/doc/skin.png?raw=true "Optional Title")

## Installation

Add this line to your application's Gemfile:
```
gem "activeadmin-lte", git: "https://github.com/jstumbaugh/activeadmin-lte"
```
and run:
```
bundle install
```

Disable stylesheets of ActiveAdmin in your project. By default, remove these
lines to active_admin.scss
```
@import "active_admin/mixins";
@import "active_admin/base";
```

Create the file `config/initializers/active_admin_lte.rb` and configure the
colorscheme.
```
ActiveAdmin::LTE.configure.skin='blue'
```

The color options are:

   - blue
   - black
   - green
   - purple
   - red
   - purple
   - blue-light
   - black-light
   - green-light
   - purple-light
   - red-light
   - purple-light

The `light` options make the left navigation bar white instead of the default
black.

You will also need to tell Rails to add the custom css to the precompiled asset
pipeline. To do that, create the file `config/initializers/assets.rb` and add the
following line:
```
Rails.application.config.assets.precompile += %w( active_admin.css )
```

## Usage

TODO

## Version

AdminLTE - Version 2.3.0

### Version of Rails tested

- 4.2.4
