#  ArrowScrollBox Scroll Helper Library, for Firefox older than its version 57.

This project is obsolete and not maintained anymore.

## Abstract

Arrowscrollbox cannot be scrolled by line if its *child* is too large.
In other words, arrowscrollbox works correctly only when there are small children.
This library helps you to scroll such a scroll box by line.

## Usage

### XUL

    <arrowscrollbox id="scrollbox" orient="vertical">
      <vbox>
        <checkbox/>
        <checkbox/>
        <checkbox/>
        <checkbox/>
      </vbox>
    </arrowscrollbox>

### JavaScript

    var box = document.getElementById('scrollbox');
    var base = box.getElementsByTagName('checkbox')[0];
    new window['piro.sakura.ne.jp'].arrowScrollBoxScrollHelper(box, base);
    // 1st argument: DOMNode or ID of an element
    // 2nd argument: DOMNode, ID of an element, or local name of a child element

