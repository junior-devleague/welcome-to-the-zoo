# welcome-to-the-zoo

Welcome to the Zoo! Look around and pet our collection of exotic animals.

## Objective

Use **JavaScript Objects** to represent zoo animals, **Object Methods** to generate text in the console, and **Dot notation** to correctly access object properties. On click of a button, generate the correct zoo animal name, image, and description in the animal container.

## Prerequisites

To complete this project, students should have the following:
* Basic understanding of HTML structures and attributes.
* Basic understanding of JavaScript and DOM.

## Concepts

JS | Description
---|-------------
JS | **J** ava **S** cript used to create the function of web pages.
Object | Variables that can contain many values.
Method | Function associated with an object.
Dot notation | Access an object's property using object.property

Remember that objects are variables that can store many values within them. Take a look at the general structure of an object which we've stored in a variable called animal.

``` JavaScript
var animal = {
  name: "Crocodile",
  age: 2,
  isWild: true,
  babies: ["Cindycroc", "Bobbycroc", "Janeycroc"],
  makeNoise: function() {
    console.log("RAAAWR");
  }
}
```

Notice that this object stored in animal contains a string, number, boolean, array, and function! All types of values can be stored within an object.

How do we access these values from our object? We can use a DOT between the variable name and the property name (dot notation):

``` javscript
console.log(animal.age) // Prints 2
```

How do we call a function? Usually we would use the functionName and parenthesis as in: functionName()

How do we call a function associated with an object (method)?

``` javascript
console.log(animal.makeNoise()); // Prints "RAAAWR" to the console.
```

*What gets printed to the console if we instead do animal.makeNoise? Try it!*

## Your Challenge

### Part I

To complete Part I, fulfill the following requirements:

1. Set up your project file structure through the command line.
2. Create the following:
* HTML file
* JS file
* CSS file
3. Link all of your files correctly.

### Part II Create the Zoo in HTML

To complete Part II, fulfill the following requirements:

1. In your HTML file, create the following with the correct parent child relationships as indicated with indentation.
* ```div``` with ```id``` of "container"
  * ```div``` with ```id``` of "animal-container"
    * ```h1``` with ```id``` of "animal-name" and text "Welcome to the Zoo!"
    * ```img``` with ```id``` of "animal-image"
    * ```p``` with ```id``` of "animal-description" and text "Click on the animal to view more information."
  * ```div``` with ```id``` of "zoo-container"
    * ```button``` with ```id``` of "button1" and text of an animal you can find at the zoo.
    * ```button``` with ```id``` of "button2" and text of an animal you can find at the zoo.
    * ```button``` with ```id``` of "button3" and text of an animal you can find at the zoo.

### Part III Zoo Styes in CSS

To complete Part III, fulfill the following requirements in your CSS:

1. Target the ```id``` of "container".
* Set the height to the full view height.
* Set the width to the full view width.
* Activate flexbox.
* Center the items HORIZONTALLY using flexbox.
* Center the items VERTICALLY using flexbox.
* Set the direction of items to COLUMN using flexbox.

2. Target the ```id``` of "animal-container".
* Activate flexbox.
* Center the items HORIZONTALLY using flexbox.
* Center the items VERTICALLY using flexbox.
* Set the direction of items to COLUMN using flexbox.

3. Target the ```img``` element.
* Set the width to 300px.
* Set the height to 200px.

### Part IV Make the Zoo Alive in JS

To complete Part IV, fulfill the following requirements in your JS:

1. Create a ```variable``` called animalImageContainer that will store your animal image by id (id is "animal-image").
2. Create a ```variable``` called animalNameContainer that will store your animal name container by id (id is "animal-name").
3. Create a ```variable``` called animalDescriptionContainer that will store your animal description by id (id is "animal-description").
4. Create a ```variable``` called button1 that will store your 1st button by id (id is "button1").
5. Create a ```variable``` called button2 that will store your 2nd button by id (id is "button2").
6. Create a ```variable``` called button3 that will store your 3rd button by id (id is "button3").
7. Create a ```variable``` called animal1 that will store an object with the following properties:
  * name: String (ex. "Fiji banded iguana")
  * image: String (ex. Copy Image Address from online picture ->  'http://reptilepark.com.au/wp-content/uploads/2015/12/iguana_fijian_banded-1030x686.jpg')
  * description: String (ex. "The fiji banded iguana is...")
  * makeNoise: function that will print to the console the sound that the animal would make (ex. console.log("RAWR!"))

8. Create a ```variable``` called animal2 that will store an object with the following properties:
  * name: String
  * image: String
  * description: String
  * makeNoise: function

9. Create a ```variable``` called animal3 that will store an object with the following properties:
  * name: String
  * image: String
  * description: String
  * makeNoise: function

10. Create an ```onclick function``` on your button1 that will do the following. Look at the code comments in this example:

``` javascript

button1.onclick = function() {
  // Change the image to the 1st animal's image
  animalImageContainer.src =
  // Change the name to the 1st animal's name
  animalNameContainer.innerHTML =
  // Change the description to the 1st animal's description
  animalDescriptionContainer.innerHTML =
}

```
11. Create an ```onclick function``` on your button2 that will do the same thing as the above function but for the 2nd animal.

12. Create an ```onclick function``` on your button3 that will do the same thing as the above function but for the 3rd animal.

13. Create a ```variable``` called currentAnimal. Do not set this equal to anything yet.

14. Go back to each of your onclick functions. Set the value of the currentAnimal variable to the current animal object (animal1, animal2, or animal3). So, when the 1st button is clicked, the currentAnimal should be set to animal1!

15. Create an ```onclick function``` on your animalImageContainer. When this image is clicked, do the following:
  * Call the makeNoise function on the currentAnimal! Resource: https://www.w3schools.com/js/js_object_methods.asp

## Stretch Goals

1. Add a property to your zoo animals called isEndangered. Look the animal up to see if they are endangered and set the value to true or false accordingly. If the image of an animal that is endangered is clicked, play a growling sound!
