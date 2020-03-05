# PixelFox
a simple startpage for Firefox with some pixelart.
![FF in Debian-openbox](/scrot1.png)

## Instructions:

Place both chrome and startpage in .mozilla/firefox/PROFILE/ to use them. You can get the location of your PROFILE dir in about:profiles. Set the startpage for Home in preferences and restart.


* the chrome dir contains 3 types of files.


1. userChrome.css and userContent.css for the UI and the default homepage respectively.

2. userChrome.xml and userChrome.js for setting the New tab page to a custom page.

3. scrollbars.css, scrollbars.xml and scrollbars.js is a slim scrollbar which looks great. Tested on FF 69. I couldnt make the scrollbars work in later versions.


If you are using FF 69+ you need to enable it first:
about:config > toolkit.legacyUserProfileCustomizations.stylesheets > true


* For the startpage:
To enable the newtab startpage functionality open userChrome.js and then change  const mypage = "file:///home/debasis/.mozilla/firefox/sawjo289.default-esr/startpage/index.html";
Put the path of your index.html in the quotation.

Thats it. Enjoy.
