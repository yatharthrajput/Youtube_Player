![YOUTUBE PLAYER FLUTTER](ypf_banner.png)




Flutter plugin for playing or streaming YouTube videos inline using the official [**iFrame Player API**](https://developers.google.com/youtube/iframe_api_reference).

Supported Platforms:
* **Android** 
* **iOS**

![DEMO](ypf_demo.gif)

## Salient Features
* Inline Playback
* Supports captions
* No need for API Key
* Supports custom controls
* Retrieves video meta data
* Supports Live Stream videos
* Supports changing playback rate
* Support for both Android and iOS
* Adapts to quality as per the bandwidth
* Fast Forward and Rewind on horizontal drag
* Fit Videos to wide screens with pinch gestures

The plugin uses [flutter_inappwebview](https://pub.dartlang.org/packages/flutter_inappwebview) under-the-hood.

Since *flutter_inappwebview* relies on Flutter's mechanism for embedding Android and iOS views, this plugin might share some known issues tagged with the [platform-views](https://github.com/flutter/flutter/labels/a%3A%20platform-views) label.

## Requirements
* Android: `minSdkVersion 17` and add support for `androidx` (see [AndroidX Migration](https://flutter.dev/docs/development/androidx-migration))
* iOS: `--ios-language swift`, Xcode version `>= 11`




         
#### Playing live stream videos
Set the isLive property to true in order to change the UI to match Live Video.

![Live UI Demo](live_ui.png) 

```dart
YoutubePlayerController _controller = YoutubePlayerController(
    initialVideoId: 'iLnmTe5Q2Qw',
    flags: YoutubePLayerFlags(
      isLive: true,
    ),
);

YoutubePlayer(
    controller: _controller,
    liveUIColor: Colors.amber,
),
```



## Quick Links
* [YoutubePlayer](https://pub.dev/documentation/youtube_player_flutter/latest/youtube_player_flutter/YoutubePlayer-class.html)
* [YoutubePlayerController](https://pub.dev/documentation/youtube_player_flutter/latest/youtube_player_flutter/YoutubePlayerController-class.html)
* [YoutubePlayerFlags](https://pub.dev/documentation/youtube_player_flutter/latest/youtube_player_flutter/YoutubePlayerFlags-class.html)
* [YoutubePlayerValue](https://pub.dev/documentation/youtube_player_flutter/latest/youtube_player_flutter/YoutubePlayerValue-class.html)
* [YoutubeMetaData](https://pub.dev/documentation/youtube_player_flutter/latest/youtube_player_flutter/YoutubeMetaData-class.html)

## Download
Download APKs from above(in badge) and try the plugin.
APKs are available in Assets of Github release page.

## Limitation 
Since the plugin is based on platform views. This plugin requires Android API level 20 or greater.


