# Themis Games Blind-Accessible HTML + Javascript Game Template

Blind-accessible HTML/Javascript game template, developed and maintained by Themis Games. You can read more about how it works, and the different considerations for web accessible games, [in this excellent write-up](https://docs.google.com/document/d/1J_YLephE5T3NGcvpWablU7TwMfeC04Of71-ohsAUjww).

Note that the repo owner (Night Blade) is not affiliated with Themis Games in any way, and is simply providing an up-to-date git repo of their code (as much as possible).

# Usage

- Use the `index.html` file a a starting point. If you wish, you can extract the CSS and JS into separate files
- Make sure you include the Javascript code in the `<body>` tag, because it needs to access the DOM.
- In the `scaleGamecontainer` method, make sure you change the width and height of `authoredWidth` and `authoredheight` so that the game scales correctly.
- Make the same change in the CSS: Specify `#gamecontainer.width` and `#gameContainer.height`. Also update the offsets (`left` and `top`) to half those values respsectively. This will make your game center on-screen.
- Update `sfxFiles` to list any sound files you want to preload. 
- Call `setupAudio()` on the first user gesture. This is a security feature (in Chrome), where this is no longer allowed to be called outside of user gestures. This also causes the audio files to preload.
