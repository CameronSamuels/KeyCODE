# KeyCODE
A developer tool for `e.keyCode` in webpages. Use this app to find out the `e.keyCode` or `e.which` value to use in your JavaScript code for keyboard events like `onkeydown`, `onkeyup`, and `onkeypress`.
# How to use
Open up [http://cameronsamuels.com/keycode](http://cameronsamuels.com/keycode) and type any key to get the keyCode.

In your JavaScript code, you can use the following for basic usage:
```javascript
document.onkeyup = function(e) { //create a listener function for when a key is lifted up
  switch (e.keyCode || e.which) { //switch statement for evaluating the keyCode
    case 8: alert('backspace'); //show backspace if back key was pressed
    case 13: alert('enter'); //show enter if enter key was pressed
    case 32: alert('spacebar'); //show spacebar if spacebar key was pressed
    default: alert('other key'); //show other key if none of the above
  }
  alert('Ctrl Key: ' + e.ctrlKey); //show if the ctrl key was pressed. Try other modifiers too
}
```
# Apps
I offer a [Chrome extension](https://goo.gl/eQfc6p) for easily checking keycodes without having to search or open a new tab. You can also add the page to your homescreen on your device.
# Contributing
If you want to contribute, you may fork this repo, and submit a PR (pull request). Also, you can add issues in the issues tab if there is an unknown key or bug. I will really appreciate it.
# About
Made by [Cameron Samuels](http://cameronsamuels.com) in June 2017 using JavaScript, HTML, and CSS.
### License
KeyCODE is licensed under the [Cameron Samuels License](LICENSE).
