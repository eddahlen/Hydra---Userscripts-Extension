# Hydra---Userscripts-Extension
A Safari userscript for iOS that opens Reddit links directly in the Hydra app using the hydra:// URL scheme.

This script is based on the original “Open Apollo App” userscript, modified to work with Hydra instead of Apollo.

What It Does

This userscript detects Reddit links and redirects them to Hydra.

It works on:

* Reddit pages
* Reddit media links
* Google search results
* Bing search results
* DuckDuckGo search results
* Yahoo search results
* Ecosia search results

When you tap a supported Reddit link, the script converts it into a Hydra link and opens it with:

hydra://

Example

A Reddit link like this:

https://www.reddit.com/r/example/comments/abc123/example_post/

will be opened as:

hydra://www.reddit.com/r/example/comments/abc123/example_post/

Installation on iOS

This script is intended to be used with the Userscripts Safari extension for iOS.

1. Install Userscripts

Install the Userscripts app from the App Store.

2. Enable the Safari Extension

Go to:

Settings → Apps → Safari → Extensions → Userscripts

Enable the extension and allow it to run on the websites you want, especially:

reddit.com
google.com
bing.com
duckduckgo.com
yahoo.com
ecosia.org

3. Set a Userscripts Directory

Open the Userscripts app and choose a folder for your scripts.

For example:

iCloud Drive/Userscripts

Your .user.js file needs to be saved directly inside this folder.

4. Add the Script

Save the script as:

Open Hydra App.user.js

Make sure the file name ends exactly with:

.user.js

It should not be:

Open Hydra App.user.js.txt

If you are on iOS, open the Files app, tap the three dots, choose View Options, and turn on Show All Extensions so you can confirm the real file name.

Recommended iOS Code Editors

If iOS keeps saving the file as a generic document or .txt file, use a plain-text/code editor such as:

* Runestone
* Kodex
* Textastic

Create the file in one of those apps, paste the script, and save it directly into your Userscripts directory as:

Open Hydra App.user.js

Troubleshooting

The script does not appear in Userscripts

Check that:

* The file is directly inside the selected Userscripts directory
* The file name ends with .user.js
* The file is not secretly ending in .txt
* The file is downloaded locally if stored in iCloud Drive
* Safari has been fully closed and reopened
* The Userscripts extension is enabled in Safari settings

The file says “Kind: Document” in iOS Files

This usually means iOS created it as a generic document instead of a JavaScript file.

The easiest fix is to recreate the file using a code editor like Runestone, Kodex, or Textastic, then save it again as:

Open Hydra App.user.js

Reddit links do not open Hydra

Make sure:

* The Hydra app is installed
* Hydra supports the hydra:// URL scheme
* The Userscripts extension is allowed to run on the website you are using
* The script is enabled in the Userscripts extension menu

Notes

This script skips Reddit search pages and only redirects supported Reddit links.

Search result links are handled through click listeners so that long-pressing links can still work normally.

Credits

Original script by AnthonyGress.

Modified version changes Apollo references and the apollo:// URL scheme to Hydra and hydra://.
