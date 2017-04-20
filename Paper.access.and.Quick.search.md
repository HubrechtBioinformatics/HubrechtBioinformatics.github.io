# Quick Access to web resources

A. Papers
B. Proteins, genes, etc.

## a) 1-click paper access using javascript [bookmarklet](https://en.wikipedia.org/wiki/Bookmarklet). 
Description for Mozilla Firefox, might be possible in other browsers. Based on the one-liner script by E. Izquierdo, a former student in the AvanO lab.

### 1. Create a new bookmark & save it to the `Bookmark Toolbar`

Easiest to save any website, e.g.: [snag.gy](https://snag.gy/) or [smallpdf.com](https://smallpdf.com/compress-pdf)

![bookmark](https://snag.gy/UgWduM.jpg)
    
    
### 2. Drag-and-drop to the left most position of the  `Bookmark Toolbar`
![](https://snag.gy/TzFtwH.jpg)

      
      
### 3. Right click on the bookmark's icon, then select `properties` and paste (replace) the following line into the `location` field

`javascript:location.href%20=%20window.location.protocol%20+%20%22//%22%20+%20window.location.host%20+%20%22.proxy.library.uu.nl%22%20+%20window.location.pathname;`


![edit](https://snag.gy/cgKrn3.jpg)

The code means in simpler terms: `javascript:location.href = window.location.protocol + // + window.location.host + .proxy.library.uu.nl + window.location.pathname;`

Read more on  [bookmarklets here](https://en.wikipedia.org/wiki/Bookmarklet). 
  
   
### 4. Install Firefox add-on `Bookmark Shortcut Keys`
![](https://snag.gy/YAfWon.jpg)

### 5. Visit a [paper](http://www.sciencedirect.com/science/article/pii/S1097276509006418)

### 6. Hit `CTRL+1`

*Or `CTRL+2` if you put the bookmark in the second position in the bookmark toolbar, etc.*  
Let Firefox remember your `Solis-id` and password.

### Limitations:

-  For most Elsevier journals you need to go to the **ScienceDirect** site.
-  Disable `HTTPS everywhere` on nature.com
-  Alternatively you might find the paper on [http://sci-hub.cc/](http://sci-hub.cc/). Read more at [Wikipedia](https://en.wikipedia.org/wiki/Sci-Hub).
  
<br><br><br><br><br><br>
  
-----------------------------------

## b) Quick, pre-specified search with keywords
Idea by Koos Roojers at the Kind lab.

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