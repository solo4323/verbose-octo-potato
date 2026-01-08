THIS IS A TEST NOT FINISHED WORK
WIN -> the cursor in windows format
linx -> cursor in linux KDE format MAKE YOUR OWN LINKS

For more info on the cursor you can check the doc (url only for updates): https://docs.google.com/document/d/1VrNFqmwDKE4g4Dz87yeOJnj1WNWjP7LLsV9F6KDfOaU/edit?usp=sharing

[WINDOWS]
You'll need GIMP (I used that one but others image editors may as well know if they have exporting to .ani and .cur)

|
v Non animated
Open the png that you want to make cursor
Export it to .cur another window should pop up asking for where do you want to put the pointer there you can set it changing the numbers
the X and Y coordinates are for where will it act when you click, it start at 0 0 (up left corner, you change the first one it moves to right, if you change the second one it goes down [positive number only])

Animated
open the gif with GIMP and then export it as .ani and as well as the non animated one you have to set the the cordinates of each frame




[LINUX]
In case some cursor dont work you can re create it using xcursorgen
I think it works for any desktop enviroments just the cursor names and links may change

using xcursorgen you can make cursors with:

edit t.in or the *.in file to
<size in pixels> <x> <y> <path to img> [ms duration for animated]

the X and Y coordinates are for where will it act when you click, it start at 0 0 (up left corner, you change the first one it moves to right, if you change the second one it goes down [positive number only])

example:
32 0 0 ralsei.png

in case of animation just repeat
<size> <x> <y> <path to frame> [ms duration 1,000 ms = 1 second]
32 0 0 ralsei1.png 100
32 0 0 ralsei2.png 100
...

on terminal do
xcursorgen inFilePath cursorName
example:
xcursorgen t.in pointer
