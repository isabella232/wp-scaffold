# 10up WP Scaffold

This scaffold is the starting point for all 10up WordPress projects.

It contains a bare bones theme and must use plugin for you to base your development off of. Asset bundling is handled entirely by [10up Scripts](https://github.com/10up/10up-scripts).

## How to Setup

1. [Download a zip](https://github.com/10up/wp-scaffold/archive/trunk.zip) of the repository into your project. At 10up, by default we version control the `wp-content` directory (ignoring obvious things like `uploads`). This enables to have plugins, theme, etc. all in one repository. Having separate repositories for each plugin and theme only happens in rare circumstances that are outside of our control.
2. Take what you need. If your project doesn't have a theme, remove the theme. If your project doesn't need any plugin functionality, remove the MU plugin. If your plugin doesn't need CSS/JS, remove it. If your plugin doesn't need to be translated, remove all the translation functionality.

## Scaffold Rules

Much of the functionality in the scaffold is intended to be optional depending on the needs of your project e.g. i18n functionality. However, there are a few important principles that you must follow:

1. [10up Scripts](https://github.com/10up/10up-scripts) must be used for asset bundling. Over the years we've found differences in how assets are built across projects to be very confusing for engineers.  As such, we are standardizing on 10up Scripts (which you can extend as needed). 10up Scripts contains in depth docs on how it works.
2. Functionality should be built into the 10up must-use functionality as much as possible. Presentation should be kept in the theme. Separating these two makes long term development, maintenance, and extensibility much easier.
3. Blocks should be built into the theme and follow the [example block](https://github.com/10up/wp-scaffold/tree/trunk/themes/10up-theme/includes/blocks/example-block) provided.
