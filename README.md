Gio - Chat - 
The Chat Board that no one Asked for
=================
  Live Site - https://gio-chat.web.app/
  
  Gio-Chat is an online messageboard app. The app is designed for anyone with a Google account to use with ease! Share'
  messages, photos, and memories, all in one chat board!
  
  This site is built in HTML, utilizing CSS stylesheets, and Javascript functionality.
  The site's UI was designed by Google's Material Design Lite Stylesheets, and is hosted by 
  Firebase's web servers. The site also utilizes Firebase's databases for message storage.
  Gio-Chat uses Google's authentication API for login and user data.
  
  On this site, users can:
  * View the chat board's messages, with or without using a Google Account
  * Log in with a Google account to add messages to the board
  * Use Google account to also upload images
  * Toggle a Dark-Mode feature which limits battery consumption and eye strain
  * Get a live character count for their messages - as to not overflow the message limit.
  
  
  
  Features to be Implemented in the future:
  * Multiple Channels
  * Private DMs
  * Customizable Themes


Project Outline
------------

### ← README.md 

That's this file, which you are currently reading :)

### ← index.html 

This is the main file that hosts all of the main elements. It gets manipulated by adding the messages onto it during runtime.
The MDL Stylesheets are referenced here, as well as the class declarations for all MDL elements/colors.

### ← main.css

This file handles the styling that isn't provided by Google's MDL CSS Framework.

### ← main.js

This code handles the bulk of the work, interfacing with a firebase backend to deploy the website on a firebase server.
The JS in this code handles the loading of previous messages, by reading the contents of Firebase's database and using it to fill out a message template. These templates are then inserted into an element which houses all of the messages, providing the user a scroll ability to navigate sent messages.
The JS also parses strings in the text field into JSON files with user data and message data, which gets sent to the database via Firebase API. There is also a functioning image-selector, which prompts the user to choose an image from their hard drive, and upload it to the site as a message object. 

Besides core functionality, the JS file also provides the user with a text-counter mechanic that prevents the user to lose their typed message if it exceeds firebase's limit of 300 characters. This gives a real-time update to the user's character count, and will prevent sending messages above them.
Another highlight of this project is the dark mode trigger, which changes the color scheme of the website by altering the selected MDL colors of the on-screen elements. The toggle functionality ensures that the user can switch to dark mode whenevever they see fit, at just a click of a switch.

## Assets
All Colors are imported from the Google Material Design Lite Stylesheets.


## Credits
This tutorial was adapted from Google Codelab. 
Code development and extras by Giovanni Q. @ GioEpic123
Guidance and Mentorship provided by Snap Engineering Academy 2020

Hosted live by Firebase - https://gio-chat.web.app/
-------------------

