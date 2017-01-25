# Kona-chan Cleanup
A small userscript to ease browsing of konachan.net and konachan.com

![screenshot](https://raw.githubusercontent.com/Max9403/Kona-chan-Cleanup/master/screenshot.jpg)

## Install
### Firefox
Install [Greasemonkey](https://addons.mozilla.org/en-US/firefox/addon/greasemonkey/), then **[click here to install Kona-chan cleanup](https://github.com/Max9403/Kona-chan-Cleanup/raw/master/kona-chan-cleanup.user.js)**.

Ports of Greasemonkey are available for [SeaMonkey](https://sourceforge.net/projects/gmport/) and [Pale Moon](https://github.com/janekptacijarabaci/greasemonkey/releases/latest).

### Chromium
**Userscript**: Install Violentmonkey ([Opera store](https://addons.opera.com/en/extensions/details/violent-monkey/) / [Chrome store](https://chrome.google.com/webstore/detail/violent-monkey/jinjaccalgkegednnccohejagnlnfdag)) or [Tampermonkey](https://tampermonkey.net/), then **[click here to install Kona-chan cleanup](https://github.com/Max9403/Kona-chan-Cleanup/raw/master/kona-chan-cleanup.user.js)**.

### Safari
Install [JS Blocker](http://jsblocker.toggleable.com/) or [Tampermonkey](http://tampermonkey.net/?browser=safari), then **[click here to install Kona-chan cleanup](https://github.com/Max9403/Kona-chan-Cleanup/raw/master/kona-chan-cleanup.user.js)**.

### WebKitGTK+
- **dwb**: Install the userscripts extension, then save the [script](https://github.com/Max9403/Kona-chan-Cleanup/raw/master/kona-chan-cleanup.user.js) to the `$XDG_CONFIG_HOME/dwb/greasemonkey` or `$HOME/.config/dwb/greasemonkey` directory (creating it if necessary):

  ```
  dwbem -N -i userscripts
  wget -P ${XDG_CONFIG_HOME:-$HOME/.config}/dwb/greasemonkey https://github.com/Max9403/Kona-chan-Cleanup/raw/master/kona-chan-cleanup.user.js
  ```

- **Midori**: Click the link to the [script](https://github.com/Max9403/Kona-chan-Cleanup/raw/master/kona-chan-cleanup.user.js) to install it.

- **Luakit**: Navigate to the [script](https://github.com/Max9403/Kona-chan-Cleanup/raw/master/kona-chan-cleanup.user.js), then type the command `:usi` to install it.

- **uzbl**: Install the script from https://github.com/singpolyma/singpolyma/blob/master/uzbl/data/scripts/userscript.sh, enable it in your config file, and then save [Kona-chan cleanup](https://github.com/Max9403/Kona-chan-Cleanup/raw/master/kona-chan-cleanup.user.js) to `$XDG_DATA_HOME/uzbl/userscripts` (or `$HOME/.local/share/uzbl/userscripts`). The commands below assume you have run uzbl at least once to create its config file.

  ```
  wget -P "${XDG_DATA_HOME:-$HOME/.local/share}/uzbl/scripts" https://raw.githubusercontent.com/singpolyma/singpolyma/master/uzbl/data/scripts/userscript.sh
  chmod +x "${XDG_DATA_HOME:-$HOME/.local/share}/uzbl/scripts/userscript.sh"
  echo '@on_event LOAD_COMMIT spawn @scripts_dir/userscript.sh document-start' >> "${XDG_CONFIG_HOME:-$HOME/.config}/uzbl/config"
  echo '@on_event LOAD_FINISH spawn @scripts_dir/userscript.sh document-end'   >> "${XDG_CONFIG_HOME:-$HOME/.config}/uzbl/config"
  wget -P "${XDG_DATA_HOME:-$HOME/.local/share}/uzbl/userscripts" https://github.com/Max9403/Kona-chan-Cleanup/raw/master/kona-chan-cleanup.user.js
  ```

### MS Edge
Install [Tampermonkey](https://www.microsoft.com/en-us/store/p/tampermonkey/9nblggh5162s), then **[click here to install Kona-chan cleanup](https://github.com/Max9403/Kona-chan-Cleanup/raw/master/kona-chan-cleanup.user.js)**.

## License

    The MIT License (MIT)

    Copyright © 2015 Jeppe Rune Mortensen

    Permission is hereby granted, free of charge, to any person obtaining a copy of
    this software and associated documentation files (the "Software"), to deal in
    the Software without restriction, including without limitation the rights to
    use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
    the Software, and to permit persons to whom the Software is furnished to do so,
    subject to the following conditions:

    The above copyright notice and this permission notice shall be included in all
    copies or substantial portions of the Software.

    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
    FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
    COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
    IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
    CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
