# PixelFox
a simple startpage for Firefox with some pixelart.

(scroll down for instructions)

1. Startpage without search box
![FF in Debian-openbox](/scrot1.png)

2. Startpage with search box(alt)
![FF in Debian-openbox1](/scrot2.png)


## Instructions:

Place both chrome and startpage(or startpage_alt) in .mozilla/firefox/PROFILE/ to use them. You can get the location of your PROFILE dir in about:profiles. Set the startpage for Home in preferences and restart.


* the chrome dir contains 2 types of files.


1. userChrome.css and userContent.css for the UI and the default homepage respectively.

2. userChrome.xml and userChrome.js for setting the New tab page to a custom page.



If you are using FF 69+ you need to enable it first:
about:config > toolkit.legacyUserProfileCustomizations.stylesheets > true


* For the startpage:
To enable the newtab startpage functionality open userChrome.js and then change  const mypage = "file:///home/debasis/.mozilla/firefox/sawjo289.default-esr/startpage/index.html";
Put the path of your index.html in the quotation.


### Note:

* startpage dir contains the page without searchbox.

* startpage_alt dir contains the page with searchbox.

Copy any one.

Also, you can uncomment the commnted lines in /startpage_alt/style.css to get some shadow effects.



Thats it. Enjoy.
