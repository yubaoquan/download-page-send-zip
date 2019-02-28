# download-page-send-zip
Download the web page with all resources, and make all results into a zip, and send it to some mailbox


## Steps to achieve this

1. you want to browse a web page https://github.com/a-very-exciting-project, but your environment forbid you to open that url.
2. - on a server which can request that page, run `wget -pkE -P target page_url`, to download the page into a folder named `target` -
2. In order to download *dynamic* web page, you have to use a headless browser to get the rendered webpage, and then download it with all the resources.
3. run `zip -rm target.zip target`, so folder `target` become a zip file `target.zip`
4. send the target.zip to mailbox. This step whether using linux command line tool, or use npm package? Let me see...
