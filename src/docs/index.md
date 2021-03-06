# Getting started

The only required files are [jQuery](http://jquery.com) and [jmpress.js](#builder) to use.

For a quick and simple example look at the [examples/simple/index.html](https://github.com/shama/jmpress.js/blob/beta/examples/simple/index.html) and [examples/simple/simple.css](https://github.com/shama/jmpress.js/blob/beta/examples/simple/simple.css).

## Migrating from impress.js

Currently jmpress.js includes all of the impress.js features and a lot more.

To migrate simply add jQuery, change impress.js to jmpress.js and call `$(selector).jmpress();` to initialize. Take a look at the [impress.js running on jmpress.js](http://shama.github.com/jmpress.js/examples/impress/) example.

If you use the impress.js api and you want to migrate:

| **impress.js**                | **jmpress.js**                         |
| `impress:stepenter`           | `enterStep`                            |
| `impress:stepleave`           | `leaveStep`                            |
| `impress:init`                | `$(x).afterInit(...)`                  |
| `impress().init()`            | `$(x).jmpress()`                       |
| `impress().goto()`            | `$(x).jmpress("goTo", ...)`            |
| `data-width, data-heigth`     | `viewPort: {width: ..., heigth: ...}`  |
| `max-scale`                   | `viewPort.maxScale`                    |
| `impress-on-ID`               | `step-ID`                              |

