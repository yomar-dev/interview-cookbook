# Interview Cookbook

This repository will house several code snippets and useful resources for Data Structures, Algorithms and Object-Oriented Concepts.

    Feel free to contribute to this repository and make a pull request!

## Java

>#### Sorting Algorithms
* [BubbleSort](/java/sort/BubbleSort.java)
* [InsertionSort](/java/sort/InsertSort.java)
* [SelectionSort](/java/sort/SelectionSort.java)
* [QuickSort](/java/sort/QuickSort.java)
* [MergeSort](/java/sort/MergeSort.java)

>#### Searching Algorithms
* [BinarySearch](/java/search/BinarySearch.java)
* [RotatedBinarySearch](/java/search/RotatedBinarySearch.java)
* [TernarySearch](/java/search/TernarySearch.java)
  
>### String Programs
* [Reverse String](/java/strings/ReverseString.java)
* [Palindrone String](/java/strings/PalindroneStrings.java)
* [Regular Expression](/java/strings/RegularExpression.java)
* [Remove Duplicates](/java/strings/RemoveDuplicates.java)
* [Remove White Spaces](/java/strings/RemoveWhiteSpaces.java)
* [String Segmentation](/java/strings/StringSegmentation.java)
* [Next Highest Permutation Of A String](/java/strings/NextHighestPermutation.java)
* [Anagram](/java/strings/Anagram.java)

## JavaScript(ECMAScript 2015)  

### Data Structures :  

>#### Arrays
* [Kadane's Algorithm](/javascript/DataStructures/Arrays/kadaneAlgorithm.js)
* [Missing numbers in a sequence](/javascript/DataStructures/Arrays/MissingNumber.js)
* [Sub-array sum equals k](/javascript/DataStructures/Arrays/SubArraysWithGivenSum.js)
* [largest Sub-array with contiguous 0's and 1's](/javascript/DataStructures/Arrays/LargestSubArrayWith0and1s.js)

### Algorithms :  

>#### Sorting Algorithms
* [BubbleSort](/javascript/sort/BubbleSort.js)
* [InsertionSort](/javascript/sort/InsertionSort.js)
* [SelectionSort](/javascript/sort/SelectionSort.js)
* [QuickSort](/javascript/sort/QuickSort.js)
* [MergeSort](/javascript/sort/MergeSort.js)

>#### Searching Algorithms
* [BinarySearch](/javascript/search/BinarySearch.js)
* [BinarySearchTree](/javascript/search/BinarySearchTree.js)  

>#### Greedy Algorithms  
* [GreedyKnapsack](/javascript/GreedyAlgorithms/GreedyKnapsack.js)

>#### Maps & Filters in ES6

**Maps :**  
 - A map is an object that lets us store key-value pairs where both the keys and the values can be objects, primitive values, or a combination of both of these.  

 - *Description* - The `map()` method creates a new array with the results of calling a provided function on every element in the calling array.  
```
 const numbers = [3,6,9,12];
 const newNumbers = numbers.map(num => num/3);
```
Here,we are just going over the values in ‘numbers’ array, halving them and creating a brand new array with the new values `[1,2,3,4]`.  

 - *Creating a map* - The below code snippet creates an empty map student with no key-value pairs.  
```
 const students = new Map();
 console.log(students);
```
```
 Map{}
```
 We can add key-values to a map by using the `.set()` method.  
```
 const students = new Map();  
 students.set('adithya@gmail.com',{  
    'firstName': 'Adithya',  
    'lastName':'NR',  
    'course':'Udacity React Nanodegree'  
 });  
 students.set('bapspatil@gmail.com',{  
    'firstName': 'Bapusaheb',  
    'lastName':'Patil',  
    'course':'Udacity Android Nanodegree'  
 });  
 console.log(students);  
```
```
 Map{'adithya@gmail.com' => Object{...},'bapspatil@gmail.com' => Object{...}}
```
The `.set()` method takes two arguments - the key,which is used to reference the second argument,the value.  

- *Removing* a key-value pair using the `.delete()` method.  
```
 students.delete('adithya@gmail.com');
 console.log(students);
```
```
 Map{'bapspatil@gmail.com' => Object{firstName:'Bapusaheb',lastName:'Patil',course:'Udacity Android Nanodegree'}}
```

- We can use the `.clear()` method to remove all key-value pairs from the Map.  
```
 students.clear();
 console.log(students);
```
```
 Map{}
```

**Filter :**  

The `filter()` method creates a new array with all elements that pass the test implemented by the provided function.  
```
 const names = ['Adithya','Aditya','Arjun','Abhishek','Bapusaheb'];
 const peopleWithShortNames = names.filter(name => name.length < 8);  

 //Output - peopleWithShortNames = ['Adithya','Aditya','Arjun']
```
Just like map, ‘filter’ is nothing special. It’s going over values in ‘words’ array checking which values pass the test, in this case which name has length lesser than 8 characters and then returns a new array with those names.  


## Interview Questions

>#### HTML5
**Q** : What is the purpose of the *DocType* in HTML5?  
**A** : The *DocType* element specifies the HTML version to the browser. It usually appears in the first line of code of an HTML page. Unlike the earlier versions/standards of HTML, DocType has got a simplified format in HTML5. 

**Q** : What are the various media tags introduced in HTML5?  
**A** : 
* `<audio>` – It specifies sound content.
* `<video>` – It links to a video.
* `<source>` – This tag specified the source of video and audio links.
* `<embed>` – It acts as a container for external applications.
* `<track>` – This element defines tracks for video and audio.  

**Q** : What is *SVG*?   
**A** : *SVG* which stands for Scalable Vector Graphics as recommended by the W3C is used to display vector graphics across the web.All elements and attributes of SVG support animation and use XML format.They provide high quality and responsive graphics.  

**Q** : What is a canvas?  
**A** : Canvas is an HTML5 element which can draw graphics on the fly with the help of JavaScript. The `<canvas>` element can only contain graphics. It supports a number of methods for drawing paths, boxes, circles, text, and images.  

**Q** : How do set an image as a draggable element?  
**A** : To set an image as draggable, initialize the draggable attribute with true.  
``` 
    <img draggable="true" src="...">
```  

**Q** : What is web storage in HTML?  
**A** : HTML5 brought this new ability to store web pages within the browser cache. This web storage is not only faster than the cookies but secured too. It is capable of storing a large amount of data without compromising the performance of the website.  

**Q** : What Is The Difference Between LocalStorage And SessionStorage Objects?  
**A** :  
* The `<localStorage>` object doesn’t have an expiry for the stored data whereas the `<sessionStorage>` object keeps it only for a single session.  
* The `<localStorage>` object doesn’t have a provision to delete the data upon closing of browser window whereas the `<sessionStorage>` object clears it simultaneously with the window closing down.  

>#### CSS3

**Q** : How does CSS3 support the Responsive Web Designing?  
**A** : Media Queries ;-)

**Q** : What are the different types of CSS?  
**A** : 
* *Embedded* – It adds the CSS styles using the `<style>` attribute inside the HTML file.  
* *Inline* – It adds the CSS to the HTML elements. (ie: ```<h1 style="text-align=center;font-size:36px;">Hola!</h1>```)
* *Linked/External* – It adds an external CSS file to the HTML document via the `<link>` tag.  

**Q** : How does an ID selector differ from a class selector?  
**A** : An ID Selector finds and modifies the style to only a single UNIQUE element whereas a class selector may apply to any number of HTML elements.An ID Selector is given higher priority over a class selector.  

**Q** : How do you implement a rounded border?  
**A** : By using the `border-radius` property.

**Q** : What is webkit in CSS3?  
**A** : Webkit is a core software component which is responsible for rendering HTML and CSS in browsers like Safari and Chrome. There are other similar rendering engines like Gecko for Mozilla, Presto for Opera, and Edge for IE.  
To enable Webkit on a web page, it requires prefixing the <-webkit> keyword with CSS values.  
```
.className {
    -webkit-box-shadow: 0px 0px 5px 0px #ffffff;
    box-shadow: 0px 0px 5px 0px #ffffff;
}
```

**Q** : What are *transitions* in CSS?  
**A** : CSS3 transitions help to create easy and fast animation effects. They not only give us control to change the value of a property but also let it proceed slowly for the given duration.  
```
transition, transition-delay, transition-duration, transition-property, and transition-timing-function.
```

**Q** : What are Media Queries?  
**A** : Media queries are one of the latest features of CSS3 used to define responsive styles for devices of different screen sizes.  
They are the powerful CSS tool which makes it easy to create responsive design for tablets, desktop, mobiles devices. They can help adjusting the Height, Width, Viewport, Orientation and Resolution.  
```
@media screen and (min-width: 480px) {
    body {
        background-color: #ffffff;
    }
}
```

**Q** : What are Pseudo-classes in CSS?  
**A** : A Pseudo-Class is a CSS technique to set the style when the element changes its state.  
i.e : Editing the style upon mouse hover event,Set the style when an element is on focus or Apply different styles for visited/unvisited links.  
  
```
selector:pseudo-class {
    property:value;
}
```

**Q** : Explain the working of z-index?  
**A** : The z-index is a CSS property which defines the stack order of web elements. Higher order elements will appear before any lower order element.  
```
Note – The z-index only applies to the positioned elements. For example, position:absolute, position:relative, or position:fixed.
    div {
        position: absolute;
        left: 10px;
        top: 10px;
        z-index: -1;
    }
```





### Contributors
>[Adithya NR](https://adithyabhat.com)  
[Arjun MD](https://www.linkedin.com/in/arjun-devappa-a6085114a/)  
[Aditya Kothari](https://www.linkedin.com/in/aditya-kothari-919b02131/)  
[Ankush Lakkanna](https://www.linkedin.com/in/ankush-lakkanna-275aa8149/)  
[Abhishek Iyer](https://github.com/Abhishekiyer97)  
[Bapusaheb Patil](https://bapspatil.com)
