# Twine Mobile

This repository is a fork of [Twine 2.9.2](http://twinery.org/2). The only difference is a few added stylesheet rules to make the toolbars single row and scrollable, in order to make it usable on a smaller screen. 

Here's the CSS rules that I added: 

```css
.button-bar,
.react-tabs__tab-panel--selected .button-bar.orientation-horizontal {
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    overflow-x: scroll;
    overflow-y: clip
}
.button-bar button {
    width: fit-content;
    text-wrap: nowrap
}
.route-toolbar-top {
    overflow-x: scroll
}
```