# Questions & Answers

### 1. call, apply and bind method in 
```JavaScript
/* call method */
let name1 = {
    firstname: 'Akshay',
    lastname: 'Saini',
}

let name2 = {
    firstname: 'Sachin',
    lastname: 'Tendulkar',
}

let printFullName = function (hometown) {
    console.log(this.firstname+ ' '+ this.lastname + ' from ' + hometown)
}

printFullName.call(name1, 'Ahmedabad'); // call method
printFullName.call(name2, 'Channai'); // call method

printFullName.apply(name1, ['Mumbai']) // apply method

// bind method
let printMyName = printFullName(name1, 'Mumbai');
console.log(printMyName);
printMyName();
```
* In call method we pass arguments individually using comma separated and In apply method we will pass second argument as an array list

* The bind method looks exactly the same as call method but the only difference is that instead of directly call method, the bind method bind the method with object and return value.

* call method invoke function directly.

* apply same exacly the call method the only difference is that we can use array as an argument.

* Bind method does not directly invoke the method but gives you the copy of that exactly same method invoke later. 

### 2. explain CSS position
* There are five values of position property
    * static
    * relative
    * absolute
    * fixed
    * sticky
* **Static** is the default value of element. Left, right, top, bottom and z-index do not affect with this element.
* **Relative** is the normal flow of document. Left, right, top, bottom, z-index properties affect with this position
* **Absolute** element with position absolute are positioned relative to their parent elements. One thing to note is that an element with absolute is positioned relative to closest positioned ancestor. If closest parent element is not positioned with relative then child element with absolute position is not relatively absolute with parent element.
* **Fixed** Fixed position elements are similar to absolutely positioned elements. they are always positioned relative to the *html* tag element.
* **Sticky** position: sticky is a mix of position: relative and position: fixed. It acts like a relatively positioned element until a certain scroll point and then it acts like a fixed element. 

### 3. What is < !DOCTYPE>? Is it necessary to use in HTML5?
The < !DOCTYPE> is an instruction to the web browser about what version of HTML the page is written in. It is not case sensitive. This declaration must be very first thing in the document.

### 4. What is use of sessionStorage Object in HTML?
The sessionStorage object stores the data for one session. The data is deleted when the user closes the browser window
```JavaScript
sessionStorage.blogName=”OnlineInterviewQuestions”;
document.write(sessionStorage.name);
```
https://medium.com/@dineshmarathe2/html5-css3-interview-questions-answers-e729a37aa33c