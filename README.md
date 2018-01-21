# SSAD 2018 - Ajax Exercise 1

## Clone the Exercise Remote Repository

```
$ cd /xampp/htdocs
$ git clone <GitHubRepository_URL>
$ cd ssad2018-ajax-ex1
$ ls or dir
$ git status

```


## Part 1

1.	Open the HTML file [artists.html](http://localhost/ajax-ex1/artists.html)

1.	Thoroughly examine the code in the HTML, JavaScript and PHP files.  Make sure you understand the code.

1.	Update the code so the artist_id of each artist is shown as the first column in the HTML table shown.

1.	Commit these changes to your remote repository by using the following Git Bash commands:

	```
	$ git status
	$ git add .
	$ git commit -m "Part 1"
	$ git push origin master

	```



## Part 2

1.	Run the PHP program [albums.php](http://localhost/ajax-ex1/albums.php?artist_id=1).  Notice how it is passed an argument called ``artist_id`` and a value - this returns the album names for artist id 1.  In the address bar of your browser change the value of ``artist_id`` to 2 or 3 or 4 to see albums for other artists.

1.	Provide the missing code in the ``albums.js`` function ``showData()`` to display the output shown below:

	![alt text](images/albums_html.png "Albums")

1.	Modify line 15 in ``albums.js`` so we get an Ajax request that gets album data for artist id 2 like this:

	```
	xmlhttp.open("GET", "albums.php?artist_id=2", true);  
	```

	Examine the program ``albums.php`` carefully.  Particularly, lines 4 & 8.

	Hopefully, you can see how a PHP program can be passed a specific value and in turn it will return data specific to that value. i.e.  we request data for a particular artist id and we get data for that artist id.  This is done alot in Ajax programming. 


1.	Commit these changes to your remote repository by using the following Git Bash commands:

	```
	$ git status
	$ git add .
	$ git commit -m "Part 2 - 1"
	$ git push origin master

	```

1.	Uncomment the HTML button code from ``albums.html`` to reveal a button.  Refresh to see it.

1.	Let's use the button to trigger the Ajax request.  Update the code in ``albums.js`` for the window onload event.  The code should look like this now:

	```javascript
	window.onload=function(){
	   document.getElementById('button').onclick=function(){
	      getAjaxData();
	   }
	}

	```

	Clicking the button now should trigger the Ajax request.  Again, this is done alot in Ajax programming.

1.	Commit these changes to your remote repository by using the following Git Bash commands:

	```git
	$ git status
	$ git add .
	$ git commit -m "Part 2 - 2"
	$ git push origin master

	```


## Part 3




