# cordova-plugin-ios-detect-screenshot :camera:

This is a simple cordova plugin for iOS that adds ability to detect when a screenshot is taken via a JavaScript event listener.  Unlike Android, iOS does not officially allow you to prevent in app screenshots.  [ScreenShieldKit](https://screenshieldkit.com/) was recently released but their pricing is not clear and it is questionable legally.


## Installation
```
cordova plugin add cordova-plugin-ios-detect-screenshot
```

## Usage

### Detect when a screenshot is taken in your app

``` javascript
window.addEventListener('screenshotDidTake', onScreenshotDidTake, false);

function onScreenshotDidTake() {
  // do whatever you need to do
  // ex. write to an audit log that user X took a screenshot
}
```

## Author

[Ross Martin](https://github.com/rossmartin)

## License

[The MIT License (MIT)](http://www.opensource.org/licenses/mit-license.html)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
