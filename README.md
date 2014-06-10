BypassCORS-PHP
==============

This will bypass Cross-Origin Resource Sharing block policy in PHP Javascript web applications by using cURL with the same domain referer in headers

###Install
Move the get.php to somewhere publically-accessible on your server.
This file requires cURL. If you do not have cURL installed, enter this on Linux server:
```sudo apt-get install php5-curl && sudo service apache2 restart```

###Use
JavaScript: Create a jQuery GET request to where the get.php page is located and append the url to fetch. For an example, also copy the example.html file to your server and if needed modify the get.php path location.

```
$.get("get.php/"+"http://example.com",function(data){
	alert(data);

})
```

PHP: Copy the getURL() function from the get.php file into your php file and use it by passing it the desired URL.




