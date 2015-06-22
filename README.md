VideoStreamClient
=================

Very basic SWF flash applets to "publish" and "subscribe" RTMP video streams.

videoStreamSubscribe.swf
------------------------
Params:
- connectionUrl [string]: RTMP-url
- streamName [string]: RTMP-stream
- streamData [string]: Parameter to be passed to the RTMP-server 

Methods:
- setVolume(volume [float]): Set the audio volume

videoStreamPublish.swf
----------------------
Params:
- connectionUrl [string]: RTMP-url
- streamData [string]: Parameter to be passed to the RTMP-server 
- autoPublish [bool]: Whether to start publishing video on load

Methods:
- startPublish(): Start publishing video
- stopPublish(): Stop publishing video
- setMicrophoneLevel(level [float]): Set microphone volume

Build
-----
It requires to install [Flex SDK 4.6+](http://www.adobe.com/devnet/flex/flex-sdk-download.html) which has support for `H.264`. 
Build the `publisher` or `subscriber` by running the [ant](http://ant.apache.org/) command accordingly inside publisher/subscriber directory. 
If build fails due to unknown `Flex SDK`, please edit file `build.xml` and add/modify with line
```
<property name="flex.sdk.home" location="/path-to-your/flex_sdk_4.6"/>
```
In most cases it should work if `Flex SDK` is correctly installed in your specific OS.
