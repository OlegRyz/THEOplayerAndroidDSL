

# THEOplayer Android DSL

The THEOplayer Android DSL is a domain-specific language (DSL) designed to simplify the process of integrating THEOplayer into Android applications. With this library, developers can quickly and easily set up THEOplayer in their Android apps using a simple and intuitive DSL.

## Getting Started

To get started with the THEOplayer Android DSL, you will need to have THEOplayer installed in your Android project. You can download the latest version of THEOplayer from the [THEOplayer website](https://www.theoplayer.com/).

Once you have THEOplayer installed in your project, you can add the THEOplayer Android DSL library to your project by adding the following dependency to your `build.gradle` file

IMPORTANT: Library is not yet released. 

## Usage

To use the THEOplayer Android DSL, simply create an instance of the `TheoPlayerView` class and call the `setup` method with your desired configuration:

```kotlin
val playerView = findViewById<TheoPlayerView>(R.id.playerView)
playerView.setup {
    // Set up THEOplayer configuration here
}
```

The `setup` method takes a lambda expression that contains the configuration for THEOplayer. You can use the DSL to set up various aspects of THEOplayer, including the source, poster image, and playback settings.

```kotlin
playerView.config {
    source {
        hls("https://example.com/my-stream.m3u8")
    }
    posterImage("https://example.com/poster.jpg")
    playbackSettings {
        autoplay(true)
        muted(true)
    }
}
```

For a full list of available configuration options, see the THEOplayer Android DSL documentation.

## Contributing

Contributions to the THEOplayer Android DSL are always welcome. To contribute, please fork the repository and submit a pull request with your changes.

## License

The THEOplayer Android DSL is licensed under the MIT license. See the LICENSE file for more information.
