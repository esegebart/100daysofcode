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

### Day 8 & 9: June 27, 2019 5:30 to 6:03pm
***Today's progress**:

Today I built currency converter application to take in Dollars and use toast to pop up the message in pounds. Even added the little squiggly pound sign to make it look more official. This was the end of the Android course section two. Next is the Java deep dive which I am really excited about. Some of the takeaways from the currency converter are using 

String.format("%.2f", poundAmount)

In this example, the String.format sets the decimal point to two places and accepts the variable it will be formatting as the second parameter. If you are wondering what the “%.2f” means, like I did, %f is the format specifier for float data type in the functions printf and scanf. This format specifier will display up to six digits after the decimal point, but using %.1f or %.2f will make the precision to the first or second digit.

I added in the currency photo from google and matched parent width. 

I had to take the EditText (which is a String) and create a new variable and parse it to a Double. I added the conversion and assigned it to the variable poundAmount.

Then I used toast to display the conversion to pounds at the bottom of the screen.

### Day 10: June 28, 2019 5:30 to 6:03pm
***Today's progress**:
Java deep dive. https://www.beta.browxy.com/?ref=browxy
It’s an editor you can use so you don’t have to compile everything everytime and you can save your program.
A class is like a template or what’s known as an object. 
If you had some characters that are a ghost in a game, you would create a ghost class and in it has code that defines the ghost: what it looks like, how it moves, how much damage is inflicted on it.
A class is a template to create an object.

Public is the access modifier. Available anywhere in our program. Void doesn’t return anything. Static (related to the ghost class): whether ghost is alive or dead. Each instance will have its own property whether it’s alive or dead.  *google what does static mean*
String[] array of strings. Args is a particular set of values you want to tell it. Not manually setting args when we are setting apps.

Main method is the chunk of code that is ran when the program starts. 

### Day 11: June 29, 2019 9:30am to 11:30am
***Today's Progress**:
Working with arrays. A primitive array cannot change datatype once it is created. 
Use list.length() to find the amount of items in your array. 
Use list.add() to add elements to the array.
Use list.remove() to remove elements from the array.

ListType can have elements added removed or changed.

        //Creating an array of prime numbers
        //Images from Instagram or list of user names
        int[] primeNumbers = {2, 3, 5, 7, 11, 13};
        
        //find out how many items in your array .length
        //cannot have elements added to them once it is created
        System.out.println(primeNumbers.length);
        
        
        //Can use it with any data type
        //create a new object of ArrayList
        List list = new ArrayList();
        
        list.add(2);
        list.add(3);
        list.add(5);
        
        list.remove(1);
        
        System.out.println(list.get(1));
        System.out.println(list.toString());

        //Create a list of three countries
        //Remove one country
        //Add another one
        
        List country = new ArrayList();
        
        country.add("Canada");
        country.add("Spain");
        country.add("France");
        
        
        country.remove(1);
        
        country.add("Germany");
        
        System.out.println(country.toString());


Hash Map. Have not worked with hashmaps before. Create an object of hashmap which has parameters of a Key and a Value. 

        //Maps is part of java util framework
        //Object of HashMap
        
        Map map = new HashMap();
       
       //Maps the value of father to rob
        map.put("Father", "Rob");
        map.put("Mother", "Kirsten");
        
        //Remove an item
        map.remove("Mother");
        
        //Use map.get and enter the key value father
        System.out.println(map.get("Father"));
        
        //Get the size of the map
        System.out.println(map.size());

//Exercise with if statements
int[] numbers = { 1, 2 };
     
     if (numbers[0] > numbers[1]) {
         System.out.println("The second number is bigger.");
     } else {
         System.out.println("The first number is smaller");
     }

### Day 12: June 30, 2019 7:00pm to 8:00pm
***Today's progress** 
Had to do a little bit of troubleshooting why my emulator didn't show up anymore. I had to enter the Path to the file with adb.exe to System Variables by selecting edit and add new path. Added the path and closed the environmental variables. Now I was able to use adb commands.
Opened the command prompt and and used “adb connect device_ip_address:5555”. The ip address taken from the genymotion device screen clicking on it in android studio. 
Got my button to work and display to the log screen. 




