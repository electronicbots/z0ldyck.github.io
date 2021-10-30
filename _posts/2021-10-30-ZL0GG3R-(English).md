---
title: ZL0GG3R (English)
author: Z0ldyck
date: 2021-08-25 18:32:00 -0500
categories: [Blogging, Tutorial]
tags: [Applocker, CLM]
---

# Agenda:

- **Introduction**
- **Installation**
- **User Guide**
- **What’s Next?**


# Introduction:

Hello everyone, before going over our new application, let me just give you the background of this project. ZL0gg3r was part of my College Research Project. The project was just to create a simple Keylogger which is easy to create with Python, but I decided to challenge myself and create it with C# as I started using it recently. I mentioned the Key Logger idea to one of my friends, and he told me, why not make it even more than just a Keylogger. Which is the reason why we created this tool. So we are going to add more features that will make it go beyond a typical Keylogger.


We started with just the basics, which was just creating the Key Logger, then we moved to creating the Application and adding some simple features to it. While we were creating the Application, new ideas and features always came to our mind, but we didn’t want to shift the release of it until we finished the whole program. So we decided to release this Beta version, and the new feature will be added monthly to it. You can check what new features we are going to add, or you can even suggest to us new ideas, that can make the program even better.



# Installation:

I just wanted to let you know before asking us questions on Twitter or Github please follow this guide and make sure everything is as mentioned in this documentation. The Key Logger is currently using FTP to transfer files from the victim machine, check the “What’s Next?” section to see what other transfer features we will be adding.

## ZL0GG3R:

You can clone the whole repo and build the program using Visual Studio or you can use the Pre-Built one by downloading the zip file. I would suggest using the pre-built one, as it was configured by us. I also want to mention that you may need to modify some of the code to work on your Windows.

Open the program in Visual Studio and then open “Form2.cs” from the right panel. Go to line 53 and make note of the CSC version number. You may need to change that path to the one your computer has.



After that just right-click on the Project name and hit “Build”. You should then be all set.
In the same directory, you should be able to notice a file called “keylogger.cs”. Open this file and go to line 64. Modify the IP Address to match yours. Save it and close, then you should be all set to start using ZL0GG3R.

## FTP Server:

You are not limited to what FTP Client you are using, we might build an FTP Client just for this project later. This guide will help you install and run the Windows FTP Server.


In the Search Bar lookup for “Turn Windows features on or off” and open it. You should see something similar to this:




Go down and expand “Internet Information Services” so you can check the “FTP Server” option. Make sure all the options are selected, check the image below:



You will also need to Check “Web Management Tools”. Then hit OK. Then the installation should start. After that, using the Search Bar lookup “Internet Information Services (IIS) Manager” and open it. Expand the left side menu and right-click on “Sites”, then click on “Add FTP Site…”. You can now type the site name and the physical path. I would suggest creating a directory for the FTP Server inside the ZLogger path.





In the next window you can leave everything as it is, but make sure to select “No SSL”, and you can then hit Next. In the Authentication window select “Basic” and then for the “Allow access to” section, you can set it to “Specific users” and write the username there. Make sure to checkmark the Read and Write permissions. If you hit Finish you should be all set. You can copy a file to the physical path and try to connect to the FTP server using File Explorer.




## Web Server:

We will be also using the IIS Web server, you can choose something else, but make sure you modify the program code. Because It is not that hard to configure the server, you can use the following documentation on how to set it up and start running it:

Install and Setup a Website in IIS on Windows 10

Make sure to set the root directory of the Web Server to the directory called “WebSrv” which is found in the directory of the application.


# User Guide:

Before reading this section make sure you did the installation correctly. We are working on making the program more user-friendly, and creating a better theme. You can see below the current program main page.







Let’s start first in the Generate section where you will be inputting your data, and generating the keylogger exe file.



When you finish just hit “Generate” and an exe file will be located in the root directory of the program.


The last section is the “Log Files” where you can choose the path where all the log files are located and open them inside the program.






## Detectable?

I know people will be using Virus Total to scan the Keylogger, so it is not going to take that long to be detected by the AVs. Our main objective is not to keep the Keylogger undetectable, but we will try our best to keep it undetected. By the time of writing this article, there were only one AV was able to detect it:



We will be also posting another article about Anti Virus evasion methods.


# What’s Next?

So the program may look very basic at the moment, but we are working on adding the new features and testing them out before releasing them, so that will take some time. You can read below what are the features we are adding.


For log files transferring:

- Through Email
- HTTP
- Discord
- Slack
- Telegram
- (Other methods that will not be mentioned currently.)


The Application itself:

- Taking screenshots
- Voice recording
- Voice recording to Text
- USB
- Reading a plugged-in USB content
- Video Recording
- New Theme (based on the community)
- (Other ideas that will not be mentioned currently.)


If you have other things you think the program is missing let us know on Twitter, you can find us here: