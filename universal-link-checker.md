# Universal link checker

This is probably *very very* niche idea but still. Just today I was troubleshooting some issues with [Universal links](https://developer.apple.com/ios/universal-links/) in one app which turned out were caused by missing and in other case improperly formatted apple-app-association file which is JSON file you can put on your site to enable Universal links.

If you have one site then the check is quick but if you have multiple sites it quickly adds up, especially if you need to construct the URL yourself and check them in your browser.

So finally the app idea. I think this would work better as a web service where you could create an account, add domains and it would periodically check them for valid association files. It could even sent a email warning.
App would be quicker and could use background tasks to do the checking and then sent notification in case something is wrong. 

Other features could include advanced JSON parsing which would do code highlighting and possibly allow to paste concrete URL to validate that these association rules cover and it should work.