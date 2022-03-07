Watch this video to understand what to do in this exercise block [link](https://www.youtube.com/watch?v=zGpplZj4zY0&feature=youtu.be)

#### Getting To Know String Methods

Go to this [link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) and look for the name of method to learn about it.

**Write in your own way of understanding (don't copy paste)**

Only if you are done with step 1 you should go ahead.

1. Practice it by yourself in console (4-5 times to understand)
2. Data types of parameters
3. Return value type
4. Write three examples
5. In your own words and one sentence explain what this method does.

Example:

1. `charAt`

   - Parameter: (index) defaults to 0 - (number data type)
   - Return: character at specific index in the string (string data type)
   - Example:
     ```js
     let name = 'Arya Stark';
     name.charAt(2); //"y"
     let sentance = 'A quick brown fox jumped over a lazy dog';
     sentance(4); // "i"
     let houseName = 'Starks';
     houseName.charAt(0); // "S"
     ```
   - `charAt` accepts a index (number data type) and return the character on that index in the string.

2. `toUpperCase`
   - Parameter: (empty)  - (string data type)
   - Return: new string converted into the uppercase (string data type)
   - Example:
     ```js
     let name = 'John Snow';
     name.toUpperCase(); //"JOHN SNOW"
     let sentance = 'Lion is coming to road';
     sentance.toUpperCase(); // "LION IS COMING TO ROAD"
     let houseName = 'Lever';
     houseName.toUpperCase(); // "LEVER"
     ```
   - `toUpperCase` accepts a empty parameter (string data type) and return the string converted into the uppercase.

3. `toLowerCase`
   - Parameter: (empty)  - (string data type)
   - Return: new string converted into the uppercase (string data type)
   - Example:
     ```js
     let name = 'John Snow';
     name.toUpperCase(); //"john snow"
     let sentance = 'Lion is coming to road';
     sentance.toUpperCase(); // "lion is coming to road"
     let houseName = 'Lever';
     houseName.toUpperCase(); // "lever"
     ```
   - `toUpperCase` accepts a empty parameter (string data type) and return the string converted into the lowercase.

4. `trim`
   - Parameter: (empty)  - (string data type)
   - Return: new string removed the whitespaces from start and end (string data type)
   - Example:
     ```js
     let name = '            John Snow               ';
     name.trim(); //"John Snow"
     let sentance = 'Lion is coming to road                    ';
     sentance.trim(); // "Lion is coming to road"
     let houseName = '                       Lever';
     houseName.trim(); // "Lever"
     ```
   - `trim` accepts a empty parameter (string data type) and return the new string removed the whitespaces from start and end.

5. `trimEnd`
   - Parameter: (empty)  - (string data type)
   - Return: new string removed the whitespaces from end (string data type)
   - Example:
     ```js
     let name = 'John Snow               ';
     name.trimEnd(); //"John Snow"
     let sentance = 'Lion is coming to road                    ';
     sentance.trimEnd(); // "Lion is coming to road"
     let houseName = 'Lever                     ';
     houseName.trimEnd(); // "Lever"
     ```
   - `trimEnd` accepts a empty parameter (string data type) and return the new string removed the whitespaces from end.

6. `trimStart`
   - Parameter: (empty)  - (string data type)
   - Return: new string removed the whitespaces from start (string data type)
   - Example:
     ```js
     let name = '      John Snow';
     name.trimStart(); //"John Snow"
     let sentance = '          Lion is coming to road';
     sentance.trimStart(); // "Lion is coming to road"
     let houseName = '     Lever';
     houseName.trimStart(); // "Lever"
     ```
   - `trimStart` accepts a empty parameter (string data type) and return the new string removed the whitespaces from start.
7. `concat`
   - Parameter: (string)One or more strings to concatenate - (string data type)
   - Return: A new string containing the combined text of the strings provided. (string data type)
   - Example:
     ```js
     let firstName = 'John';
     let lastName = 'Snow';
     firstName.concat(' ', lastName); //'John Snow'
     let sentance = 'Lion is coming to road';
     let sentance2 = 'the king';
     sentance.concat(' ',sentence2); // "Lion is coming to road the king"
     let houseName = 'Lever';
     houseName.concat(',',sentance2); // 'Lever,the king'
     ```
   - `concat` accepts a one or more strings (string data type) and return the new string containing the combined text. 

8. `endsWith`
   - Parameter: (string)The characters to be searched for at the end of string - (string data type)
   - Return: true.if the given characters are found at the end of the string; otherwise, false. (string data type)
   - Example:
     ```js
     let firstName = 'John';
     firstName.endsWith('n'); //true
     let sentance = 'Lion is coming to road';
     sentence.endsWith('road'); // true
     let houseName = 'Lever';
     houseName.endsWith('!'); // false
     ```
   - `endsWith` The characters to be searched for at the end of string(string data type) and return true.if the given characters are found at the end of the string; otherwise, false. 

9. `includes`
- Parameter: A string to be searched for within(position) optional - (string data type)
   - Return: true if the search string is found anywhere within the given string; otherwise, false if not.(string data type)
   - Example:
     ```js
     let firstName = 'John';
     firstName.includes('J'); //true
     let sentance = 'Lion is coming to road';
     sentence.includes('coming'); // true
     let houseName = 'Lever';
     houseName.includes(''); // true
     ```
   - `includes` to be searched for within strings (string data type) and return true if the search string is found anywhere within the given string; otherwise, false if not.

10. `indexOf`
- Parameter: a substring to search for, searches the entire calling string(position) optional - (string data type)
   - Return: The index of the first occurrence of search of String found, or -1 if not found.(string data type)
   - Example:
     ```js
     let firstName = 'John';
     firstName.indexOf('h'); //2
     let sentance = 'Lion is coming to road';
     sentance.indexOf('road'); // 18
     let houseName = 'Lever';
     houseName.indexOf(''); // 0
     ```
   - `indexOf` to be searched for within strings (string data type) and return The index of the first occurrence of search of String found, or -1 if not found.
11. `lastIndexOf`
- Parameter: a substring to search for, searches the entire calling string(position) optional - (string data type)
   - Return: The index of the last occurrence of search of String found, or -1 if not found.(string data type)
   - Example:
     ```js
     let firstName = 'John';
     firstName.lastIndexOf('n'); //3
     let sentance = 'Lion is coming to road';
     sentance.lastIndexOf('is'); // 5
     let houseName = 'Lever';
     houseName.lastIndexOf('e'); // -1
     ```
   - `lastIndexOf` to be searched for within strings (string data type) and return The index of the last occurrence of search of String found, or -1 if not found.

12. `padEnd`
- Parameter: The length of the resulting string once the current str has been padded. (length)(padstring) optional - (string data type)
   - Return: A String of the specified Length with the padString applied at the end of the current str.(string data type)
   - Example:
     ```js
     let firstName = 'John Snow is fighter';
     firstName.padEnd('30','.'); //'John Snow is fighter..........'
     let sentance = 'Lion is coming to road slowly';
     sentance.padEnd('35','!'); // 'Lion is coming to road slowly!!!!!!'
     let houseName = 'Lever';
     houseName.padEnd('10','#'); // 'Lever#####'
     ```
   - `padEnd` the length of the resulting strings (string data type) and return String of the specified Length with the padString applied at the end of the current str.

13. `padStart`
- Parameter: The length of the resulting string once the current str has been padded. (length)(padstring) optional - (string data type)
   - Return: A String of the specified Length with the padString applied at from the start of the current str.(string data type)
   - Example:
     ```js
     let firstName = 'John Snow is fighter';
     firstName.padStart('22','.'); //'..John Snow is fighter'
     let sentance = 'Lion is coming to road slowly';
     sentance.padStart('50','$'); // '$$$$$$$$$$$$$$$$$$$$$Lion is coming to road slowly'
     let houseName = 'Lever';
     houseName.padStart('15','#'); //'##########Lever'
     ```
   - `padStart` the length of the resulting strings (string data type) and return String of the specified Length with the padString applied from the start of the current str.

14. `repeat`
- Parameter: (count)indicating the number of times to repeat the string.(string data type)
   - Return: A new string containing the specified number of copies of the given string.(string data type)
   - Example:
     ```js
     let firstName = 'John Snow is fighter';
     firstName.repeat(5); //'John Snow is fighterJohn Snow is fighterJohn Snow is fighterJohn Snow is fighterJohn Snow is fighter'
     let sentance = 'Lion is coming to road slowly';
     sentance.repeat("Lion",2); //'Lion is coming to road slowlyLion is coming to road slowly'
     let houseName = 'Lever';
     houseName.repeat(9); //'LeverLeverLeverLeverLeverLeverLeverLeverLever'
     ```
   - `repeat` indicating the number of times to repeat the string(string data type) and return A new string containing the specified number of copies of the given string.

15. `replace`
- Parameter: (objet or literal)A RegExp object or literal. The match or matches are replaced with newSubstr or the value returned by the specified function.(substring)(string data type)
   - Return: A new string, with some or all matches of a pattern replaced by a replacement.(string data type)
   - Example:
     ```js
     let firstName = 'John Snow is fighter';
     firstName.replace("fighter","teacher"); //'John Snow is teacher'
     let sentance = 'Lion is coming to road slowly';
     sentance.replace("Lion","Spider"); //'Spider is coming to road slowly'
     let houseName = 'Leversmash';
     houseName.replace("smash","pool"); //'Leverpool'
     ```
   - `replace` The match or matches are replaced with newSubstr(string data type) and return A new string, with some or all matches of a pattern replaced by a replacement.

16. `slice`
- Parameter: (beginIndex)The zero-based index at which to begin extraction.(endIndex) Optional.(substring)(string data type)
   - Return: A new string containing the extracted section of the string.(string data type)
   - Example:
     ```js
     let firstName = 'John Snow is fighter';
     firstName.slice(0,12); //'John Snow is'
     let sentance = 'Lion is coming to road slowly';
     sentance.slice(8,30); //'coming to road slowly'
     let houseName = 'Leversmash';
     houseName.slice(5,10); //'smash'
     ```
   - `slice` The zero-based index at which to begin extraction(string data type) and return A new string containing the extracted section of the string.

17. `split`
- Parameter: (separator)The pattern describing where each split should occur. The separator can be a simple string or it can be a regular expression.(limit) Optional.A non-negative integer specifying a limit on the number of substrings.(string data type)
   - Return: An Array of strings, split at each point where the separator occurs in the given string.(string data type)
   - Example:
     ```js
     let firstName = 'John Snow is fighter';
     firstName.split(' '); //(4) ['John', 'Snow', 'is', 'fighter']
     let sentance = 'Lion is coming to road slowly';
     sentance.split(' '); //(6) ['Lion', 'is', 'coming', 'to', 'road', 'slowly']
     let houseName = 'Leversmash';
     houseName.split(''); //(10) ['L', 'e', 'v', 'e', 'r', 's', 'm', 'a', 's', 'h']
     ```
   - `split` The pattern describing where each split should occur.(string data type) and return An Array of strings, split at each point where the separator occurs in the given string.

18. `substring`
- Parameter: (indexStart)The index of the first character to include in the returned substring.(indexEnd)optional(string data type)
   - Return: A new string containing the specified part of the given string.(string data type)
   - Example:
     ```js
     let firstName = 'John Snow is fighter';
     firstName.substring(0,15); //'John Snow is fi'
     let sentance = 'Lion is coming to road slowly';
     sentance.substring(5,20); //'is coming to ro'
     let houseName = 'Leversmash';
     houseName.substring(0,5); //'Lever'
     ```
   - `substring` The pattern describing where each split should occur.(string data type) and return An Array of strings, split at each point where the separator occurs in the given string.

