---
layout: post
title: BlocJams
feature-img: "img/sample_feature_img.png"
thumbnail-path: "https://d13yacurqjgara.cloudfront.net/users/3217/screenshots/2030974/bloctalk_1x.png"
short-description: BlocJams for iOS is awesome!

---
SongPlayer.js AngularJS Service Case Study

Summary

This service contains the operations used in both playing and pausing songs on a song list in an album view and playing, pausing, skipping, and changing playback time and volume on a player bar.

Explanation

In order to insure a pleasant user experience, Buzz was used to upload songs to the page, and users needed to be able play and pause songs these songs from both the song list and the player bar that would be available at the bottom of the screen.  The player bar, however, needed to do a good bit more to allow the user to skip songs, raise and lower volume, and seek forward and backward through a song.

Problem

One particular problem that arose was that the songs and the user’s ability to manipulate them would disappear if the user browsed other parts of website, meaning the users had to remain on the album view in order for the songs to play.

Solution

The solution to this problem came from creating a separate view and controller for the player bar and having the controller instantiate the SongPlayer.js service and be called using ng-controller on the view.  This way the player bar could be added to any page in the site using ng-include.

Results

This resulted in the user being able to browse other parts of the website while maintaining the ability to operate the player bar at the bottom of each page.

Conclusion

In order for a webpage to be able to use songs and manipulate those songs, many different parts have to operate together.  AngularJS offers solutions to this that allow for a complex and pleasant user experience.  The album page and the player bar are two examples of solutions created in my BlocJams app, which have the ability to allow a user to search through a list of songs from an album and play and control each song in each album.  More examples of code from BlocJams as well as other examples Ruby on Rails, AngularJS, and jQuery based apps can be found on my Github page at https://github.com/melanconz.
