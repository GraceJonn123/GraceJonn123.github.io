---
layout: post
title: How to fix the META-INF situation.
---

#META-INF

###What is META-INF?

Metadata are "data that provide information about other data". Two types of metadata exist: structural metadata and descriptive metadata. 
**Structural metadata** are data about the containers of data. 
**Descriptive metadata** use individual instances of application data or the data content.

In Java, you often see a META-INF folder containing some meta files. 
Have you ever asked yourself what the purpose of this folder is and what can be put in there? Well i think i could answer that roughly.

The META-INF folder is the home fort the MANIFEST.MF file. This file contains meta data about the contents of the JAR. 
For example, there is an entry called Main-Class that specifies the name of the Java class with the static main() for executable JAR files.


You can also place static resources in there.

In example:

__META-INF/resources/button.jpg__ and get them in web3.0-container via __http://localhost/myapp/button.jpg__

Anyway, if you ever get an error of this manner;


Error:duplicate files during packaging of APK E:\Code\iDoc\app\build\outputs\apk\app-debug-unaligned.apk

    Path in archive: META-INF/license.txt
    
    Origin 1: E:\Code\iDoc\app\libs\spring-core-3.1.0.RELEASE.jar
    
    Origin 2: E:\Code\iDoc\app\libs\spring-web-3.1.0.RELEASE.jar
    
    
You can ignore those files in your build.gradle:

    android {
    
      packagingOptions {
      
        exclude 'META-INF/license.txt'
        
      }
      
    }
    
    
probably the issue is that the packaging options for the META-INF are lacking.

Add this to your gradle file.



packagingOptions{

        exclude 'META-INF/DEPENDENCIES'
        
        exclude 'META-INF/NOTICE'
        
        exclude 'META-INF/LICENSE'
        
        exclude 'META-INF/LICENSE.txt'
        
        exclude 'META-INF/NOTICE.txt'
    }
    
    
And voila! Run gradle again and there you have it. You fixed a META-INF bug.
