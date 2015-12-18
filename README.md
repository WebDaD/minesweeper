Gardenplay.js
===========
(Based on Minesweeper.js by Michael Butler)

A WebWorker powered Minesweeper game written in JavaScript, HTML and CSS.
The Setting has been changed to be more child friendly.

Demo: [missing]

New Setting:
------------

You play in a garden and must avoid water ponds (you dont want to step into them, right?)  
You may add leafs to mark them.

Features:
-----------
+ Configurable grid size (X, Y)
+ User can choose difficulty level
+ Configurable number of ponds
+ Stopwatch with score keeping (LocalStorage)
+ Stack based grid traversal algorithm for memory efficiency
+ HTML5 web worker (if supported) will be used to perform the stack algorithm outside of the UI thread

How to use:
-----------
Download all the files and open `index.html` in a modern web browser.

Example HTML usage:
-----------
```
<!-- requires jQuery -->
<h1 class="logo">JavaScript GardenPlay
    <div class="invisible ajax-loading"><img src="load.gif" alt="Processing..."/></div>
</h1>
<div id="gardenplay"></div>

<script src="js/GardenPlay.js" type="text/javascript"></script>
<script>
    // set a global instance of GardenPlay
    gardenplay = new GardenPlay();
    gardenplay.init();
</script>
```

To Do:
-----------
+ Auto-clear feature to clear multiple squares at once
+ Add animation and better graphics
+ Bigger Icons and bigger grid
+ check for mobile
+ Enhance UI for a sleek new look
+ Use nice icons for items
+ tune colors


License:
-----------
    GardenPlay.js is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    GardenPlay.js is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with GardenPlay.js.  If not, see <http://www.gnu.org/licenses/>.
