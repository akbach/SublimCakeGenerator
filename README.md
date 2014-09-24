Cakephp bake generator
===============

Fork of Sublime Text plugin for Laravel 4 Artisan

This plugin allows you the run Cakephp Console commandes directly from the Sublime Text interface.

### Available commands:

##### Cake php supported Commands
- `Cakephp Generate: Project`
- `Cakephp Generate: Model`
- `Cakephp Generate: Controller`
- `Cakephp Generate: View`
- `Cakephp Generate: Helper`
- `Cakephp Generate: Behavior`
- `Cakephp Generate: Component`
- `Cakephp Generate: Cell`
- `Cakephp Generate: Fixture`
- `Cakephp Generate: Shell`
- `Cakephp Generate: Test`
- `Cakephp Generate: Plugin`

- you can add `--help` to commande field to see help

##### Custom Commands
You can add custom commands.
Use `Preferences/Package Settings/Cakephp Generator/Commands – User` menu item.

Simple command structure:

```json
[
    {
        "caption": "Cakephp generator: Deploy Project",
        "command": "sublime_cake_generator",
        "args": {
            "command": "customshell",
            "fill_in": true,
            "fill_in_lable": "paramname"
        }
    }
]
```

Change command `caption` and `command` in `args`.
Use `fill_in: true` if you need some input for your command and `fill_in_lable: "Text"` for message.

### Installation:
Use Package Controller or create a the directory `Laravel 4 Artisan` in your Sublime Text Packages directory with source code, and you're ready to go.

### Usage:
Press Cmd + Shift + P for the dropdown command list, search for `cakephp `, and pick your command. Also you can use `Tools/Cakephp...` menu item

### Notes:
- You need insert in Sublime Text user settings `"show_panel_on_build": true` or use `Tools/Build Results/Show Build Results` menu item for view results.
- Tested with Cakephp 2.4 and 3.0beta and Sublime 3 on osx
- Edit cake_console_path and php_path on `Preferences/Package Settings/Cakephp Generator/Settings – User`
- You can get php path by `which php`
### Original Project:
[Laravel 4 Artisan](https://github.com/evgeny-golubev/Laravel-4-Artisan)

Thanks.
