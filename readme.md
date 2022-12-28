# learning js
1. JavaScript Can Change HTML Content
- JavaScript accepts both double and single quotes
```
<p id="demo">JavaScript can change HTML content.</p>

<button type="button" onclick="document.getElementById('demo').innerHTML = 'Hello JavaScript!'">Click Me!</button>
```

2. JavaScript Can Change HTML Attribute Values
```
<button onclick="document.getElementById('myImage').src='pic_bulbon.gif'">Turn on the light</button>

<img id="myImage" src="pic_bulboff.gif" style="width:100px">

<button onclick="document.getElementById('myImage').src='pic_bulboff.gif'">Turn off the light</button>
```
3. JavaScript Can Change HTML Styles (CSS)
```
<p id="demo">JavaScript can change the style of an HTML element.</p>

<button type="button" onclick="document.getElementById('demo').style.fontSize='35px'">Click Me!</button>
```

4. JavaScript Can Hide HTML Elements
```
<p id="demo">JavaScript can hide HTML elements.</p>

<button type="button" onclick="document.getElementById('demo').style.display='none'">Click Me!</button>
```

5. JavaScript Can Show HTML Elements
```
<p id="demo" style="display:none">Hello JavaScript!</p>

<button type="button" onclick="document.getElementById('demo').style.display='block'">Click Me!</button>
```
# JavaScript Where To
> The <script> Tag <br>
In HTML, JavaScript code is inserted between <script> and </script> tags.

```
<p id="demo"></p>

<script>
document.getElementById("demo").innerHTML = "My First JavaScript";
</script>
```
# js function
A JavaScript function is a block of JavaScript code, that can be executed when "called" for.
<br>
**You can place any number of scripts in an HTML document.**
<br>
**Scripts can be placed in the <body>, or in the <head> section of an HTML page, or in both.**
1. JavaScript in <head>
> In this example, a JavaScript function is placed in the <head> section of an HTML page.

```
<html>
<head>
<script>
function myFunction() {
  document.getElementById("demo").innerHTML = "Paragraph changed.";
}
</script>
</head>
<body>
<h2>Demo JavaScript in Head</h2>

<p id="demo">A Paragraph</p>
<button type="button" onclick="myFunction()">Try it</button>

</body>
```
2. js in body
```
<p id="demo">A Paragraph</p>

<button type="button" onclick="myFunction()">Try it</button>

<script>
function myFunction() {
  document.getElementById("demo").innerHTML = "Paragraph changed.";
}
</script>
```
3. External JavaScript Advantages
- It separates HTML and code
- It makes HTML and JavaScript easier to read and maintain
- Cached JavaScript files can speed up page loads


- An external script can be referenced in 3 different ways:

  - With a full URL (a full web address)
    - ex: ```<script src="https://www.w3schools.com/js/myScript.js"></script>```
  - With a file path (like /js/)
    - ex: ``` <script src="/js/myScript.js"></script>```
  - Without any path
    - ex: ``` <script src="myScript.js"></script>```

-----------------------------------------------------------------------------------------
# js output
JavaScript can "display" data in different ways:

- Writing into an HTML element, using innerHTML.
<br>
  - **js use the document.getElementById(id)<br>
  - id =>html element innerHTML =>html content**
- Writing into the HTML output using document.write().
  - **Never call document.write after the document has finished loading. It will overwrite the whole document.**<br>
  - **Using document.write() after an HTML document is loaded, will delete all existing HTML**
- Writing into an alert box, using window.alert().
  - **alert your code**
  - **You can skip the window keyword.**
  - **window object is the global scope object**


- Writing into the browser console, using console.log().
  - For debugging purposes, you can call the console.log() method in the browser to display data.

---------------------------------------------------------------------------------------------
# js print
1. JavaScript does not have any print object or print methods.
2. The only exception is that you can call the window.print() method in the browser to print the content of the current window.
---------------------------------------------------------------------------------------------
computer program=>list of instruction <br>
programming instruction=>statements<br>
javascript=>list of programming statement<br>
**In HTML, JavaScript programs are executed by the web browser.**
---------------------------------------------------------------------------------------------
JavaScript's statements are composed of:

1. values
2. operators
3. expressions
4. keywords
5. comments
---------------------------------------------------------------------------------------------
very important point:<br>
1. **The statements are executed, one by one, in the same order as they are written.**
2. **Semicolons separate JavaScript statements.**
3. **JavaScript ignores multiple spaces.**
4. **For best readability, programmers often like to avoid code lines longer than 80 characters.**
5. JavaScript's statements can be grouped together in code blocks, inside curly brackets {...}.

``` 
function myFunction() {
  document.getElementById("demo1").innerHTML = "Hello Dolly!";
  document.getElementById("demo2").innerHTML = "How are you?";
}
```

JavaScript's statements often start with a keyword to identify the JavaScript action to be performed.
> var,let,const,if,switch,for,function,return,try

---------------------------------------------------------------------------------------------
# js syntax












