# Themis Games Blind-Accessible HTML + Javascript Game Template

Blind-accessible HTML/Javascript game template, developed and maintained by Themis Games. You can read more about how it works, and the different considerations for web accessible games, [in this excellent write-up](https://docs.google.com/document/d/1J_YLephE5T3NGcvpWablU7TwMfeC04Of71-ohsAUjww).

Note that the repo owner (Night Blade) is not affiliated with Themis Games in any way, and is simply providing an up-to-date git repo of their code (as much as possible).

# Usage

Use the `index.html` file a a starting point; feel free to extract the CSS and JS into separate files if you prefer that.

Note that the accessibility code has a `setupAudio()` method which needs to be called on the first user gesture (in Chrome); as part of their security fixes, this is no longer allowed to be called outside of user gestures.
