#Workshop - Using the Dev Tools

In this exercise we will be using the dev tools in Google chrome. Although there are excellent dev tools also available in Firefox and Safari, we have chosen to use Chrome due to its ease of use and clarity of information.

##A GET request to a URL
* Visit http://www.ebuyer.com
* Open the network tab and look for the request named 'www.ebuyer.com'
* Can you find the response status code of this request?  200 
  * What does is the meaning of this status code? Request was fulfilled
  * List some resources you could use to look up the meaning of other status codes you may come across.
  * https://www.w3.org/Protocols/HTTP/HTRESP.html
  *https://en.wikipedia.org/wiki/List_of_HTTP_status_codes
* What language is listed as acceptable in the request headers? en-GB,en-US
  * what is the purpose of this header? Why might this information be useful?
  * The request header also contains the type, version and capabilities of the browser that is making the request so that server returns compatible data.Upon receipt of the request header, the server will return an HTTP response header to the client that is attached to the file(s) being sent. As the language on our computer is set to English the resuest is asking the response to be in english so it is compatiable.
* Name a URL that is listed in the content-security-policy.  https://secure.pay4later.com
  * what is this list of URLs for? It is the list of URL's that the website trusts data from or marks as unsafe.
* What was the total response time of the request? 196.23ms
* Look for meta data in the HTML response - what is the "description" tag for? General website contents to describe website

##POSTing form data
* Visit https://online.lloydsbank.co.uk/personal/logon
* Open the network tab of your dev tools
* Enter a fake name and password (not a password you normally use)
* Open the 'primaryLogin' request
  * Can your pair partner find what fake password you entered on the site? Yes 
  * What can you infer from this about the behaviour of forms on websites? That info entered into forms isnt secure
  * frmLogin:strCustomerLogin_userID:Jollyjon
  frmLogin:strCustomerLogin_pwd:rtwewerwr

