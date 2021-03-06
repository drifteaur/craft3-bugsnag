# Bugsnag plugin for Craft CMS 3.x

Log Craft errors/exceptions to Bugsnag.

![Screenshot](resources/icon.png)

## Requirements

This plugin requires Craft CMS 3.0.0-RC1 or later.

## Installation

To install the plugin, follow these instructions.

1. Open your terminal and go to your Craft project:

        cd /path/to/project

2. Then tell Composer to load the plugin:

        composer require superbig/craft3-bugsnag

3. In the Control Panel, go to Settings → Plugins and click the “Install” button for Bugsnag.

## Bugsnag Overview

Bugsnag's cross platform error monitoring automatically detects crashes in your applications, letting you ship with confidence.

## Configuring Bugsnag

1. Copy the config.php configuration file into your `craft/config` folder.
2. Update `serverApiKey` with a API key from your Bugsnag project.
3. (Optionally) Set the `releaseStage` configuration setting to something. Defaults to `production`.

## Using Bugsnag

It will automatically log most exceptions/errors. If you want to log a exceptions/error from an custom plugin, you may use the service methods:

- For exceptions: `Bugsnag::$plugin->bugsnagService->handleException($exception);`

Brought to you by [Superbig](https://superbig.co)
