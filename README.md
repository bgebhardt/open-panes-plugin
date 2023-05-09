# List Open Panes Plugin

This is a simple plugin for Obsidian that adds a command to list the open panes as wiki links at the current selection.

Once installed you and use the command palette to execute "List Open Panes" which pastes in the current open panes (aka tabs) where your current selection is. This will replace any selected text!

I recommend setting a hotkey shortcut to quickly paste in the open panes (aka tabs). I use cmd-control-K.


## How to set up the build

- Clone this repo.
- `npm i` or `yarn` to install dependencies
- `npm run dev` to start compilation in watch mode.

## Manually installing the plugin

- `npm run build` to build the project.
- Copy over `main.js`, `styles.css`, `manifest.json` to your vault `VaultFolder/.obsidian/plugins/your-plugin-id/`.

I will at some point submit this to be a community plugin after I clean up the code.

# Other Notes

This plugin was forked from the Obsidian Sample Plugin (https://github.com/obsidianmd/obsidian-sample-plugin).

This project uses Typescript to provide type checking and documentation.
The repo depends on the latest plugin API (obsidian.d.ts) in Typescript Definition format, which contains TSDoc comments describing what it does.

## First time developing plugins?

Quick starting guide for new plugin devs:

- Check if [someone already developed a plugin for what you want](https://obsidian.md/plugins)! There might be an existing plugin similar enough that you can partner up with.
- Make a copy of this repo as a template with the "Use this template" button (login to GitHub if you don't see it).
- Clone your repo to a local development folder. For convenience, you can place this folder in your `.obsidian/plugins/your-plugin-name` folder.
- Install NodeJS, then run `npm i` in the command line under your repo folder.
- Run `npm run dev` to compile your plugin from `main.ts` to `main.js`.
- Make changes to `main.ts` (or create new `.ts` files). Those changes should be automatically compiled into `main.js`.
- Reload Obsidian to load the new version of your plugin.
- Enable plugin in settings window.
- For updates to the Obsidian API run `npm update` in the command line under your repo folder.

## API Documentation

See https://github.com/obsidianmd/obsidian-api
