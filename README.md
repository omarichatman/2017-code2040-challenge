This is all my code for the 2016 Code2040 API challenege. 
I have written this in JavaScript using the WebStorm IDE. 

Step1: Register 

Objective:
This challenge was to POST an HTTP Request with 2 keys to a url that was given. 

Methods:
I used a jQuery $.post() method to send the HTTP request with keys (token) and (github).

Step2: Reverse a string 

Objective:
This challenge was to use POST then recieve a string from the URL. Collect that string, reverse it, then send it back to the validate URL using POST. 

Methods:
After my POST I used function(res) to collect the string I recieved. Created a function with parameter string. Then used .split(), .reverse() and .join() to reverse the string and return it. Then use POST to send the reversed sting to a validate URL. 

Step3: Needle in a haystack

Objective:
This challenge was to use POST then recieve an object from the URL with a string named needle and an array of strings named haystack. Look through the array of strings and return the index of the place the string needle was. Use POST to send it to a validate URL. 

Methods:
After my POST I created a fucntion with parameters, string and stringArray. Then used .indexOf() to check the string array(haystack) for the string(needle) and get the index value from that word in the array. 

Step4: Prefix 

Objective:
This challenge was to use POST then recieve an object from the URL with string named prefix and an array of strings. Look through the array of strings then create an array with all the words from the original array that dont have the prefix inside the string.  

Methods:
After my POST I created a fucntion with parameters, string and stringArray. Then used a for loop to loop through the array of strings. Created a variable to hold the strings I want to add to my new array. Then an if statement using .startsWith() to check if any of the string have the prefix I collected and if not use .push() to add that string to my new array. Use POST to send my new array to the validat link.

Step5: The Dating Game

Objective:
This challenge was to use POST then recieve an object from the URL with string named Datestamp and number named Interval. Datestamp is formatted in years, months, days  then a T after that hours, minutes, and seconds then a Z ( YY-MM-DDTHH:MM:SSZ ). Take the numbers from the datestamp and add the interval (in seconds) to the Datestamp and create the new date in the same format as the Datestamp. 

Methods:
After my POST I created a fucntion with parameters, datestamp and interval. JavaScript has very few key words that will help with dates except new Date(). So I used the custom JavaScript library momnet.js. mooment let me pass in the Datestamp in the correct format and I used moment().add() to add interval to datestamp. The used .toISOString() to convert .add() to the correct Datestamp format. Since .add() returns it with millisends I use .replace() to get rid of the milliseconds. The new Datestamp is now in the correct format I can save that value and use POST to send it to the validate link. 
