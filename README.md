# Array-and-String-Methods
List of popular string and array methods - includes their time complexity, and various examples on how these methods can be implemented


Please research the following methods:

Give a short description of what the method does, how it works, it's time complexity, and give three examples of it in action!


slice (1, 4) -slice(start, end - not including the end) this method removes a chunk of an array - like a swiss army knife. 
array.slice(1,4) will remove everything from index 1 to 3. The last one is never included. 


Pop - this array method removes the last element in the array
Let array = [1,2,3,5,6,7,8]
array.pop()  // you will have the following array:  [1,2,3,5,6,7]

Shift - this method removes an element from the beginning of an array
Let array = [1,2,3,5,6,7,8]
Array.shift()  // returns [2,3,5,6,7,8]

Push - this method adds an element from the end of an array:
Let array = [1,2,3,4,5,6,7]
array.push(8)
Return array // this returns a new array like the following: [1,2,3,4,5,6,7, 8]

Unshift - this method adds a new element at the beginning of your array
Let array =  [1,2,3,5,6,7,8]
array.unshift(22) // will return the following array:  [22, 1,2,3,5,6,7,8]

Includes - array method that will determine if array includes something. Will return true or false 

Let array =  [1,2,3,5,6,7,8]
arr.includes(8) // should return true
arr.includes(“brown”) // should return false 


indexOf -  array method that determines the index of a given element

Let array = [1,2,3,4,”purple”, 10, 13]

Example: array.indexOf(“purple”) // will return 4



Map - an array method that creates a new array based on the conditions involved in the function that iterates over each element 
New array will be the same size as old array
Map of US - for each state I want the capitals of each state 
For each element you transform it into something
Let arr = [0,1,2,3,4,5,6,7,8,9]
Objective: increase each one by one
arr.map(element)
=. Functions have an implicit return 
Let newArray = array.map(element => element + 3
Return newArray // will
 return [3,4,5,6,7,8,9,10,11,12,13]
Let newArray = array.map(element => `${element} Dogs`)
Let newArray = array.map(element => element + “Dogs”)



Filter - array method that will filter out elements in your array - potentially removing elements  from the array. It creates a new array with all the elements that pass the test implemented by the function applied 
New array will be the same size or smaller 
Example:
Let words = [“yes”, “no”, “maybe”, “so”, “khorally”];
Let updatedWords = words.filter(element.length > 6
// expected output will be Array [“khorally”] 

forEach - this is a lot like map, it iterates over an array and applies a function to each element. Will not create a new array. 

Example:
Let array1 = [‘a’, ‘b’, ‘c’, ‘d’, ‘e’];
array1.forEach(element => console.log(element));
// this will output each element in the console. 
array1.forEach(element => element + “person”);
// will output the word “person” after each element


Sort(a,b) - this method will sort your array
The default sort order is ascending
Example: let months = [‘march’, ‘april’, ‘may’, ‘june’, ‘july’]
months.sort()
// this will sort the months in alphabetical order 
Let array2 = [1,20,3,4,10000, 25]
console.log(array2.sort());
The output will be [1, 10000, 20, 25, 3, 4]
The time and space complexity of the sort cannot be guaranteed as it depends on the implementation.

Reduce - an array method that creates a new array
Executes a reducer function that you provide on each element of the array - results in a single output value 
Let array3 = [1,2,3,5]
Let reducerFunction = (accumulator, currentValue = > accumulator + currenValue;
console.log(array3.reduce(reducer))
// expected output will be 11
conso.log(array1.reduce(reducer, 5));
// expected output would be 16


Every  - an array method that tests whether all elements in the array pass the test of the function applied to it. This returns a boolean value 

Example: let passesTheTest = (currentValue) => currentValue < 40;
Let array4 = [1,39, 30, 10, 13]
console.log(array4.every(passTheTest));
// this will return true because everything is below 40 


7/ 12

please research the following string methods:



Concat - string method where strings get put together 
Examples:
Let str1 = “hi”;
Let str2= “there”;
 Return str1.concat(‘ ‘, str2);
// output will be: “hit there”

Let str3 = “be”
Let str4 = “resilient”

Return str3.concat(‘ !’, str4)
// should return be! resilient 


Slice - extracts a part of a string and returns extracted parts in a new string 
First parameter is necessary, the last one determines where the extraction ends. If no last parameter is given, it will print out everything from the first parameter
Example: 
Let string = “beautiful day”
string.slice(0, 9)
// returns “beautiful”

Let string2 = “Khorally Pierre”
string.slice(0, 5)
// returns “khoral”


Let string3 = “Khorally Pierre”
string.slice(10)
// returns “pierre”


toLowerCase - changes everything to lower case
Example :
Let string1 = “Give Me My Money!”
string1.toLowerCase()
Returns “give me my money!”

Let string2 = “GIVE ME MY MONEY!”
string2.toLowerCase()
Returns “give me my money!”

toUpperCase - method that turns string to upper case
Example:

Let string10 = “I’m a Snob and I Talk Like This”
string10.toUpperCase()
// returns “I’M A SNOB AND I TALK LIKE THIS”


Includes-string method that determines whether or not a string includes something, returns true or false 

Example: 
Let string = “I like pancakes”
string.includes(“pancakes”)
// this should return true 

Let string = “I like pancakes”
string.includes(“cake”)
// this should return false 

Let string = “Leon is great”
string.includes(“is”)
// this should return true

** you can also test which position that word is located in the string:
string.includes(searchstring, position) 


Split - method that divides a string into smaller strings, converting the string into an array of strings
Example: 
Let string = “the brown fox ate my dog”
string.split(“ ”) // the space between the quotation marks indicate that words will become their own strings.
string.split(“”) - no space between quotation marks mean each letter would  become a string

Let word = string.split(“ ”)
console.log(word[2]) // this would return “fox”


indexOf - this method returns the index of a chosen element
Example:
Let sentence = “blanket forts are cool”
sentence.indexOf(“forts”) // this returns 7

Let sentence2 = “beds are soft and comfy”
sentence.indexOf(“comfy”) // this returns 14

Let sentence = “be resilient always!”
sentence.indexOf(“be”) // this returns 0

charAt - method that returns a new string consisting of the single UTF-16 code unit 
charCodeAt - string method  that returns an integer that represents the UTF-16 code at the given index 


Replace -  string method used to replace one element with one of your choosing. First parameter is what youre replacing, second is what youre replacing it with 
Example 1:
Let song = “Do you really love me, do you love me”
song.replace(“love”, “hate)

Return song // should return “do you really hate me, do you love me ”
// willonly change the first occurrence 

Example 2:

Let song = “my Red car was painted red because I really like red”
song.replace (/red/gi, “orange”)
// will return  “my orange car was painted orange because I really like orange”
//  gi syntax changes all occurrences, even those capitalized

Example 3:

Let song = “meeseeks are called Mr. Blue and are blue annoyingly blue creatures”
song.replace (/blue/g, “pink”)
// will return “meeseeks are called Mr. Blue and are pink annoyingly pink creatures”
//  gi syntax changes all occurrences but disregards capitalized ones

Search - string method that's used to find a specific string - returns integer representing the location of the string being searched for 
Example: 
Let blanket = “brown purple and yellow”
blanket.search(“p”)

// this returns 6 

Trim - string method that removes blank spaces from strings from the beginning and from the end 
Example:

Let str = “          Beyonce can't be messed with         ”
console.log(str.trim())
// this returns “Beyonce can't be messed with” 


Substr - this method extracts part of a string and returns the portion of the string based on start index and end index. Includes the end index in the extraction

Example:
Const str = “inside world”
Return str.substr(1,2);
// this returns “ns” 


Match - method that retrieves the result of matching a string against a regular expression

Example1: 

Let sentence = "The rain in SPAIN stays mainly in the plain"; 
Let matchedLetters = sentence.match(/ain/gi); 
// returns all occurrences of “ain” from the sentence 

Example 2:
Let sentence2 = “I went to getti to eat spaghetti, but I ran into letti”
Let matchedLetters = sentence2.match(etti/gi);
Returns all occurrences of “etti” 

Repeat - string method that creates and returns a new string that contains a number of copies of the string which it was called, gets combined together 

Example 1: 
Let chorus = “because I\’m happy.”;
chorus.repeat(27); 
Returns “because I\’m happy. because I\’m happy. because I\’m happy. because I\’m happy. because I\’m happy.” - will print 27 times 

Example 2:
Let bob = “squidward”; 
bob.repeat(3)
// Returns “squidward. squidward. Squidward.”

Example 3:
Let emotion = “laugh”; 
emotion.repeat(3)
// Returns “laugh laugh laugh”

