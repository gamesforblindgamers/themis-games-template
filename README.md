# Blind-Accessible HTML + Javascript Game Template

Blind-accessible HTML/Javascript game template, originally developed and maintained by Themis Games. You can read more about how it works, and the different considerations for web accessible games, [in this excellent write-up](https://docs.google.com/document/d/1J_YLephE5T3NGcvpWablU7TwMfeC04Of71-ohsAUjww).

# Games That Use This

- [Wordvoyance](https://www.themisgames.com/wordvoyance/)

# License
Creative Commons 0 (CC0)

# Usage

- Use the `index.html` file a a starting point. If you wish, you can extract the CSS and JS into separate files
- Make sure you include the Javascript code in the `<body>` tag, because it needs to access the DOM.
- In the `scaleGamecontainer` method, make sure you change the width and height of `authoredWidth` and `authoredheight` so that the game scales correctly.
- Make the same change in the CSS: Specify `#gamecontainer.width` and `#gameContainer.height`. Also update the offsets (`left` and `top`) to half those values respsectively. This will make your game center on-screen.
- Update `sfxFiles` to list any sound files you want to preload. 
- Call `setupAudio()` on the first user gesture. This is a security feature (in Chrome), where this is no longer allowed to be called outside of user gestures. This also causes the audio files to preload.
