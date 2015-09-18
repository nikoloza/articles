## How to debug remote iOS device using Chrome devtools.

![How to debug remote iOS device using Chrome devtools](http://f.cl.ly/items/200p1d3H340B1Y3q2W3Z/Image%202015-09-18%20at%207.55.31%20AM.png)

After whole night surfing in internet, I've found Google's
[repository](https://github.com/google/ios-webkit-debug-proxy) about **proxying DevTools for iOS**. They offer `Safari web inspector`, but you can do it from Safari's developer tab anyways. So, if you're Chrome Devtools dependent developer like me, you need to follow this article.

===

### Installing:

Only thing you need to install is `ios-webkit-debug-proxy` via [homebrew](http://brew.sh/) or `apt-get`:

Mac:

    brew install ios-webkit-debug-proxy

Linux:

    sudo apt-get install \
        autoconf automake \
        libusb-dev libusb-1.0-0-dev \
        libplist-dev libplist++-dev \
        usbmuxd libtool \
        libimobiledevice-dev

    git clone git@github.com:google/ios-webkit-debug-proxy.git
    cd ios-webkit-debug-proxy

    ./autogen.sh
    make
    sudo make install

===

### Running:

Open Safari on your Simulator, or device first and run (for Chrome greater
then 45)

    ios_webkit_debug_proxy -f chrome-devtools://devtools/bundled/inspector.html

It will detect your available devices and list them on port `:9221`:

- list of devices here [localhost:9221](http://localhost:9221)
- fist connected device [localhost:9222](http://localhost:9222)
- second connected device [localhost:9223](http://localhost:9223)
- etc...

**Note:**
due the error that Chrome does not allow opening the `chrome-devtools://` url
from DOM, you may need to navigate there by clicking on `Open in new tab` or
copy the given url and paste it to your address bar.

It should be like this:

    chrome-devtools://devtools/bundled/inspector.html?ws=localhost:{portNumber}/devtools/page/1


**Note 2:**
You'll probably need to enable `Settings > Safari > Advanced > Web Inspector`

For the first time, it'll maybe throw an error that couldn't connect to Safari on device (even if you have `Web Inspector` enabled). Try to remove usb cable and plug it again.
