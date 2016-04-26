#Workshop - Using the Dev Tools

In this exercise we will be using the dev tools in Google chrome. Although there are excellent dev tools also available in Firefox and Safari, we have chosen to use Chrome due to its ease of use and clarity of information.

##A GET request to a URL
* Visit http://www.ebuyer.com
* Open the network tab and look for the request named 'www.ebuyer.com'
* Can you find the response status code of this request?
  * What does is the meaning of this status code?
  * List some resources you could use to look up the meaning of other status codes you may come across.
* What language is listed as acceptable in the request headers?
  * what is the purpose of this header? Why might this information be useful?
* Name a URL that is listed in the content-security-policy.
  * what is this list of URLs for?
* What was the total response time of the request?
* Look for meta data in the HTML response - what is the "description" tag for?

##POSTing form data
* Visit https://online.lloydsbank.co.uk/personal/logon
* Open the network tab of your dev tools
* Enter a fake name and password (not a password you normally use)
* Open the 'primaryLogin' request
  * Can your pair partner find what fake password you entered on the site?
  * What can you infer from this about the behaviour of forms on websites?

Resource for checking status codes : http://httpstatuses.com
acceptable languages : en-GB,en-US;q=0.8,en;q=0.6 number is acceptable weight
purpose of this header : Its a request from the client to send back the information in the required format because thats how we like it
Name a URL that is listed in the content-security-policy. : www.google-analytics.com, heartukdeals.com

what is this list of URLs for : The new Content-Security-Policy HTTP response header helps you reduce XSS risks on modern browsers by declaring what dynamic resources are allowed to load via a HTTP Header.(in other words, places we are friends with?)

The new Content-Security-Policy HTTP response header helps you reduce XSS risks on modern browsers by declaring what dynamic resources are allowed to load via a HTTP Header. 523.75ms

Look for meta data in the HTML response - what is the "description" tag for? : A meta description is an HTML and XHTML element that describes your page to search engines (addwords for search engines?)

Open the 'primaryLogin' request : yes we can find the password its in the headeres tab under form data
                                : theres probaly some extra security going on, maybe not very safe? theres an extra level of encryption between client and server?

by max and amy