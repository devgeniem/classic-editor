# Classic Editor
(WordPress plugin)

Restores the Classic Editor and the old-style Edit Post screen layout (TinyMCE, Meta boxes, etc.). Supports the plugins that extend this screen.

## Notes about this fork

This a forked version of the original GitHub repository of the Classic Editor plugin. This repository adds Composer support for the plugin and installs it as a mu-plugin to be used with the [Bedrock Autoloader](https://github.com/roots/bedrock/blob/master/web/app/mu-plugins/bedrock-autoloader.php).

### Installation

You need to have the [Bedrock Autoloader](https://github.com/roots/bedrock/blob/master/web/app/mu-plugins/bedrock-autoloader.php) installed in your mu-plugins folder. After copying the autoloader into your mu-plugins directory, install this with Composer as follows:

```
composer config repositories.classic-editor git git@github.com:devgeniem/classic-editor.git
composer require devgeniem/classic-editor
```

## Description

<strong>Warning: This is beta software, not recommended for production sites!</strong>

Requires WordPress 4.9 or newer and Gutenberg plugin 1.5 or newer.

Classic Editor restores the previous Edit Post screen and makes it possible to use the WordPress plugins that extend it, add old-style meta boxes, or otherwise depend on the previous editor.

It has two modes:

1. Fully replaces the Gutenberg editor and restores the Edit Post template.
2. Adds alternate "Edit" links to the Posts and Pages screens, on the toolbar at the top of the screen, and in the admin menu. Using these links will open the corresponding post or page in the Classic Editor.

The modes can be changed from the Settings => Writing screen.

The current release is intended for testing with the <a href="https://wordpress.org/plugins/gutenberg/">Gutenberg plugin</a> version 1.5 or newer.
