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
