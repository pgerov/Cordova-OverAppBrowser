OverAppBrowser 1.1
==================

Render a webview over your cordova webview.
	
	//function(strUrl, originx, originy, width, height, isAutoFadeIn)
    oab = new OverAppBrowser('http://www.google.fr', 0, 100, 320, 320, true);
    oab.addEventListener('loadstop', function(){
			oab.insertCSS({code:'#hplogoo {-webkit-transform: rotate(180deg);}'});
    });

    //Fade the webview
    oab.fade(toAlpha, duration);

    //Resize the webview
    oab.resize(originx, originy, width, height);

    //Close the webview
    oab.close();


This loads google.fr over your html app at x=0, y=100, width=320, height=320 and rotates the homepage logo


## License

The MIT License

Copyright (c) 2011 Tommy-Carlos Williams (github.com/devgeeks)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
