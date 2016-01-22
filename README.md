# adwordsandroid


AdWords SDK for Titanium, for Android. Download compiled module from the dist folder.

Just a quick wrapper for the latest Google AdWords SDK for Android (GoogleConversionTrackingSdk-2.2.4).

There is an [existing module](https://github.com/jkotchoff/adwords_conversion_tracking_titanium_module) on Github but it's outdated and using a depricated SDK. For some reasons, I had issues updating it to the latest version, so I decided to create a brand new module from scratch instead of wasting my time any further.


===

### Usage

Add it to your tiapp.xml:

`<module platform="android">me.direcciona.adwords.android</module>`
    

In your controller, call it like this:

    var TiAdwords = require("me.direcciona.adwords.android");
    TiAdwords.sendRequest({
        conversionId:"conversionId here",
        label:"label here",
        value:"value here",
        isRepeatable:true
    });
    
    
All properties are required otherwise it won't work.

Note: it follows all the UI patterns from this module for iOS, to make the code reusable btw platforms

https://github.com/jyounus/TiAdwords

(and I just copied README from this module)