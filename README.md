# The Infinite Jest

This project is inspired by David Foster Wallace's book, The Infinite Jest. One of the main threads in the book is a film that is so fun that as soon as you start watching it, you can't stop, so you die because of entertainment. What I intended to build here is something like that, but my way of thinking about that film is that it is a eternal thread of youtube videos that have been recommended by someone. 

Each time someone adds a video to the app, it gets in the database in a state that I call future. From all of those future videos, there is always one, and only one that is brought to the _present_ by the function theSource.theMind. When this happens a timeout starts, which ends when the duration of the video is elapsed, and then theMind function is called again. This keeps the amount of 'present' videos always in 1, that is the one that is displayed in the app every time you get in. 

When theMind function is called and there are no more videos in the future, the system calls a function called theSource.bigBang which changed the status of every media from _past_ to _future_, starting the whole process again. This keeps an eternal loop of content running, which is my interpretation of DFW's The Infinite Jest.
