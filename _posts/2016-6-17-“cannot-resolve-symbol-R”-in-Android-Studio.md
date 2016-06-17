---
layout: post
title: “cannot resolve symbol R” in Android Studio
---

#### Ever had this issue? R. cannot be resolved..

In many instances in all of my classes where I reference R.id.something, 
the R is in red and it says "cannot resolve symbol R". Also whenever there is R.layout.something 
it is underlined in red and says "cannot resolve method setContentView(?)". The project always builds fine. 
It is annoying to see this all the time. 

So i took it upon myself to write this, so you will not have to wander like i did.
1. Try a simple 'gradlew clean' and 'gradlew build'. That is, clean project then build it, then voila.

2. In the latest versions of Android Studio, at least for some people, the following works:

    "Tools" -> "Android" -> "Sync Project with Gradle Files"

3. Also you could make sure in your AndroidManifest.xml the package name is correct. 

4. Close and reopen project

    Sometimes as simple as it looks, this may solve your issue.


Alright, good luck with your 'R' issue. 

Ciao.


![Ya heard](http://clipartsign.com/upload/2016/04/04/good-luck-on-luck-quotes-good-luck-quotes-and-clipart.jpg)
