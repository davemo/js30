# Dave Moshers js30 challenges

## Challenge Specific Notes

> 01 - JavaScript Drum Kit

- learning that `HTMLMediaElement.play()` returns a promise was cool
- i wanted to limit the scope of `keydown` events so I added a list of valid codes to filter on when the event was fired

> 02 - JS and CSS Clock

- i decided to default the position in the markup and build a little parser to snag the current state of rotation
- this felt easier than tracking that state in a js variable
- named regex capture groups make this pretty easy
- concern: given i never reset the value on the rotation `deg` things might buffer overflow eventually?
- not yet implemented: binding to the actual current time
- bug: setInterval independently means a slight offset in latency for all the hands

