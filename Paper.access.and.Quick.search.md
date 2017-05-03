# Quick Access to web resources
> Written by Abel Vertesy, 21 April 2017

<br>  
A. Papers  
B. Proteins, genes, etc.   

<br><br><br><br>
## a) 1-click paper access using javascript [bookmarklet](https://en.wikipedia.org/wiki/Bookmarklet) to reach the library's subscription. 
Description for Mozilla Firefox, might be possible in other browsers. Based on the one-liner script by E. Izquierdo, a former student in the AvanO lab.

### Requirements

- [SOLIS-ID and Password](https://www.uu.nl/en/organisation/information-and-technology-services-its/solis-id-and-password) for UU library. 
- Firefox, or other modern browsers.
- Optionally: Bookmark Shortcut Keys add-on


### 1. Create a new bookmark & save it to the `Bookmark Toolbar`

Easiest to save any website, e.g.: [snag.gy](https://snag.gy/) or [smallpdf.com](https://smallpdf.com/compress-pdf)

![bookmark](https://snag.gy/UgWduM.jpg)
    
    
### 2. Right click on the bookmark's icon in the toolbar, then select `properties` and paste (replace) the following line into the `location` field

`javascript:location.href%20=%20window.location.protocol%20+%20%22//%22%20+%20window.location.host%20+%20%22.proxy.library.uu.nl%22%20+%20window.location.pathname;`


![edit](https://snag.gy/cgKrn3.jpg)

The code means in simpler terms: `javascript:location.href = window.location.protocol + // + window.location.host + .proxy.library.uu.nl + window.location.pathname;`

Read more on  [bookmarklets here](https://en.wikipedia.org/wiki/Bookmarklet). 

### 3. Drag-and-drop to the left most position of the  `Bookmark Toolbar`
![](https://snag.gy/TzFtwH.jpg)
   
### 4. Install Firefox add-on `Bookmark Shortcut Keys`
![](https://snag.gy/YAfWon.jpg)

 - CHROME VERSION: Install chrome add-on named: [Shortkeys](https://chrome.google.com/webstore/detail/shortkeys-custom-keyboard/logpjaacgmcbpdkdchjiaagddngobkck).
- Once installed right-click the icon of Shortkeys and select options & setup as below (Note: if you saved the Bookmark under a different name this may be different).
- You can change the keyboard command as you wish.

![link](https://snag.gy/z4jrWP.jpg)


### 5. Visit a [paper](http://www.sciencedirect.com/science/article/pii/S1097276509006418)

### 6. Hit `CTRL+1`

*Or `CTRL+2` if you put the bookmark in the second position in the bookmark toolbar, etc.*  
Let Firefox remember your `Solis-id` and password.

### Limitations:

-  For most Elsevier journals you need to go to the **ScienceDirect** site.
-  Disable `HTTPS everywhere` on nature.com
  
### Alternatives

- There is an experimental [browser plugin from UU](https://www.uu.nl/universiteitsbibliotheek/literatuur-zoeken/online-toegang/uu-easy-access-browserextensie-experiment).
-  Alternatively you might find the paper on [http://sci-hub.cc/](http://sci-hub.cc/). Read more at [Wikipedia](https://en.wikipedia.org/wiki/Sci-Hub).

<br><br><br><br><br><br>
  
-----------------------------------

## b) Quick, pre-specified search with keywords
Concept by Koos Rooijers from the Kind lab.

### 1. Setup the search & save the bookmark to the `Bookmark Toolbar`

Try [Polycomb protein EED in Uniprot for mice](http://www.uniprot.org/uniprot/?query=actb+AND+organism%3A%22Mus+musculus+%28Mouse%29+%5B10090%5D%22&sort=score)

   
      
### 2. Right click on the bookmark's icon, then select `properties` and change the following:

1. Replace your original search query `EED` with `%s`

	Original location: `http://www.uniprot.org/uniprot/?query=EED+AND+organism%3A%22Mus+musculus+%28Mouse%29+%5B10090%5D%22&sort=score`
     
	Replaced Location:   `http://www.uniprot.org/uniprot/?query=%s+AND+organism%3A%22Mus+musculus+%28Mouse%29+%5B10090%5D%22&sort=score`

2.  Set a keyword e.g. `upm`

![link](https://snag.gy/2ndkEB.jpg)

### 3. Type `upm Rad51` in the address bar to test

![link](https://snag.gy/kuzgpc.jpg)

→ You will be redirected to a Uniprot search for mice proteins. You can do it with other additional filters and websites too.



