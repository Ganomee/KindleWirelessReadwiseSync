# KindleWirelessReadwiseSync
A simple website that allows users to access and upload clippings.txt from a kindle to the readwise api using the browser


# How to use
1. copy the HTML file into your kindle documents folder, and create an AccessToken.txt in your documents folder and fill it with your Readwise access token.
2. Open the experimental browser and enter 
"""
file:///mnt/us/documents/ReadWiseSync.html
"""

3. Profit

4. Bookmark it for 1 click access the next time around

## Why does this work
0.5) the kindle (experimental) browser allows you to navigate and view any displayable file on the system using direct links, thus enabling you to run js from local files by opening local html files.

1.) The kindle browser uses a weird browser implementation, that has misconfigured cors policy that allows reading file contents of other local files given an XHTML request. This way we can pipe it into js, and sent it to (any) server.
