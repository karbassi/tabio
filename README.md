# [Tabio](http://colebemis.github.io/tabio)

> **Note:** I'm currently working on a major update to Tabio. Development on version 2 is being done in the [tabio-2](https://github.com/colebemis/tabio-2) repo. Stay up to date by following me on Twitter [@colebemis](https://twitter.com/colebemis).

### Effortless tab management for Chrome

Tabio is a Chrome extension designed to make managing lots of browser tabs significantly easier. The extension generates a searchable, scrollable and fully keyboard-accessible list of all open browser tabs.

Available on the [Google Chrome Webstore](https://chrome.google.com/webstore/detail/tabio/bgbhfmeabcmpjblimfddkeikogidjhao).

## Keyboard Shortcuts

| OSX | Windows/Linux | Description |
|---|---|---|
| <kbd>Cmd</kbd> + <kbd>K</kbd> | <kbd>Ctrl</kbd> + <kbd>K</kbd> | Toggle extension<sup>1</sup> |
| <kbd>Cmd</kbd> + <kbd>/</kbd> | <kbd>Ctrl</kbd> + <kbd>/</kbd> | Toggle help menu<sup>2</sup> |
| <kbd>Enter</kbd> | <kbd>Enter</kbd> | Go to selected tab |
| <kbd>Cmd</kbd> + <kbd>Delete</kbd> | <kbd>Ctrl</kbd> + <kbd>Backspace</kbd> | Close selected tab |
| <kbd>Up</kbd> | <kbd>Up</kbd> | Select previous tab |
| <kbd>Down</kbd> | <kbd>Down</kbd> | Select next tab |
| <kbd>Cmd</kbd> + <kbd>Up</kbd> | <kbd>Ctrl</kbd> + <kbd>Up</kbd> | Move selected tab up<sup>2</sup> |
| <kbd>Cmd</kbd> + <kbd>Down</kbd> | <kbd>Ctrl</kbd> + <kbd>Down</kbd> | Move selected tab down<sup>2</sup> |
| <kbd>Cmd</kbd> + <kbd>Shift</kbd> + <kbd>K</kbd> | <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>K</kbd> | Focus search input |
| <kbd>Esc</kbd> | <kbd>Esc</kbd> | Close help menu or extension |

<sup>1</sup> This can be configured in `chrome://extensions`. More information on that [here](http://lifehacker.com/add-custom-keyboard-shortcuts-to-chrome-extensions-for-1595322121).
<sup>2</sup> Coming in v1.3.0

## Contributing

Contributions of any kind are always welcome. Help make Tabio better by submitting a bug report, feature request or pull request. Please refer to the [contribution guidelines](CONTRIBUTING.md) for more infomation.

### Development Dependencies

| Name    | Installation                                                                       |
|---------|------------------------------------------------------------------------------------|
| Node.js | [Instructions](http://nodejs.org/download/)                                        |
| Bower   | [Instructions](http://bower.io/#install-bower)                                     |
| Gulp    | [Instructions](https://github.com/gulpjs/gulp/blob/master/docs/getting-started.md) |

### Setup

* Clone the repository

```
$ git clone https://github.com/colebemis/tabio.git
$ cd tabio
```

* Install npm dependencies

```
$ npm install
```

* Install bower dependencies

```
$ bower install
```

* Create the initial build

```
$ gulp build
```

* Load the extension

  - Open Google Chrome and type `chrome://extensions` inside the address bar
  - Enable `Developer mode`
  - Click on `Load unpacked extension`
  - Select the `/dist` folder

### Gulp Tasks

| Task    | Description                                   |
|---------|-----------------------------------------------|
| `build` | Compile, minify and copy the extension files  |
| `zip`   | Create a zip archive for publishing           |

### Known Issues

* Incorrect drawing occasionally on activation
* Delayed activation on occasion
* Unpredictable pinned tab behavior

## License

Tabio is licensed under the [MIT License](LICENSE.md).
