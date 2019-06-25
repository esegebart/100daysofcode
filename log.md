# 100 Days Of Code - Log

### Day 0: May 6, 2019
#####

**Today's Progress**: Went over the basics of classes again. Created a separate class from main, created fields that describe the state of the object with the private access modifier, and created two basic getter and setters that would get the model of the car from main and print it out and set the model of the car. Went over the "this" keyword and that when you put the dot to attach it to it, it shows locks for private or not, an m for method and f for field or p for parameter. That way you know if you are describing the parameter that is passed into the method or accessing the field through the modifier. Classes are real world objects, with fields that describe the state of them, and methods to make it do something.

**Thoughts:** I remember a lot of this, but it was really nice to go over again the modifiers, the this keyword, and learned a new trick that intellij helps us with using the little m, p, and f to know what you are accepting. I feel good about class basics.

**Link to work:** 

### Day 1: May 7, 2019

**Today's Progress**: Had a list of requirements for two classes. Created Person class and Simple Calculator class. Wrote all the methods myself, used this keyword correctly, used conditional statements and logic operators, knew to make a boolean method, had to add in the data type of some objects I created and the data type of a few methods, but I did not make the mistake after I made it once. Used test code to validate my methods and they all passed! 

### Day 2: June 20, 2019
**Today's Progress**: Got my Android Studio updated and demo projects downloaded. Videos weren't working so I sent in a support ticket. But I am ready to rock and roll when they are!

### Day 3 & 4: June 22, 2019 7:30am to 11:30am
***Today's Progress**: What I learned:
In order for the Gradle Build Failed, add Google Maven repository error to go away, go to Project Gradle build, under Allprojects>Repositories add: google() and sync.

To get relative layout to work with placing components on the relative layout from palette.. go to the top top of the view editor, to the leftish, there is a little magnet icon, turn on/off autoconnect to prevent it from magnetizing to the top left.
Make sure its in relative layout or it wont open on your screen well.

1 dp is roughly 1/60th of an inch. So 160dp is roughly 1” on any android screen.
Dp for everything except text, sp for text size. Scale Independent pixel. 

Click on an attribute to edit it. I used background, selected the color, changed the text size using dp, changed the text color, and gravity to center the text inside of the textView, use padding to set the box 
 
Buttons:
Under properties, type in the function into the onClick property. When button is clicked, clickFunction will run.
View is anything that appears on the screen. Button is a type of view.
Log.i(string tag, string msg) : 
 
Using Genymotion: You must start the device first using the Genymotion Icon at the top. Setting it up you must link the location of the Genymotion file in the Project structure. After that you can run the project by clicking Run.
Asking for user name and password:
TextField an ID and getting info from it 
 
Create an onClick function for the button.
Create the variables, typecast them to EditText because its trying to find a View, the typecast will work around this. R for resources, id is the id in the xml
Log.i will have what will show up. It was changed to show Username and Password and then getText to String to display it in the Log.

### Day 5: June 22, 2019 6:45pm to 7:15pm
***Today's Progress**: What I learned:
Learned about Toast and how to take what the user enters and display it in a pop-up message at the bottom of the screen. It's called toast because it pops up at the bottom of the screen for a short period of time like toast "pops up". Made a small toast program and pulled it all together to set up an onClick function with a button and a plain text field. Created and edit text field and typecasted it. Used toast to concatenate “Hi there, “ + enterYourName.getText().toString() to greet the person that just entered their name. 

### Day 6 & 7: June 25, 2019 5:30 to 6:03pm
***Today's progress**:
Created an application that takes two photos uploaded to the drawable folder. Added a button called New Cat and when clicked, will display a photo of a different cat. First tested that my button worked by using the Log.i to display a message to the log to ensure that my button was clicked. Created the onClick function called "clickCat". Worked very similar to the EditText, only used ImageView and typecasted the findView to ImageView. The second part was to use

image.setImageResource(R.drawable.cat2);

to set the image to the second photo upon being clicked.

