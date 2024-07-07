INDEX.HTML:
This project requires creating three files in a directory: index.html, index.js, and style.css. The HTML file is pretty short. In the head, I linked the file to the stylesheet, and gave it a title:
In the body, I inserted an <h1> tag for the header, and created a few divs. The first div surrounds the input bar and button. The second div is where new items added to the to-do list will go. In the input div, I created an <input> element, giving it necessary class, type, and placeholder, as well as a <button> with the class addButton.
At the bottom of the body, I linked to the JavaScript file.

STYLE.CSS:
The video that I followed used a lot of CSS, and as I don't have much experience with it, I largely followed along with their code.
There were, however, things I added that I thought improved the functionality of the program, or removed because I felt they were unnecessary or not in my personal style.
For this part of the code-along, I will include the CSS block-by-block, and say generally what that block does.
The body block targets the entirety of the body. These few lines are a good place to put style that will remain uniform for the program, such as background color and font.

SCRIPT.JS
The logic of this application can all by found in index.js. At the top of this file, I declared a few variables globally that will be necessary to use later on Then, I created a class called Item.
Inside the class I have a constructor, which takes in itemName. Inside the constructor, I called on an instance method called createDiv and pass in the itemName. 
Still inside the Item class, I created an instance method, createDiv, passing in itemName. This method first creates a variable called input which is an input, and is given the value of the inputName, a class of item_input, a type of text, and disabled is set to true. 
The text property disabled affects whether the field can be clicked on and altered. This is important for the editing function which will be implemented later on.
