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

### Day 13: July 1, 2019 7:41pm to 8:25pm
***Today's progress** 
Today I created a higher or lower game in Android Studio. Used Random class to generate a random number when the app launches.

Created a method that takes the user input when a button is clicked and converts the String to an int. Then I used If statement to take the int object and compare it to the random number that is generated. The app will tell the user higher or lower based on which statement is true. If the number is correct, it tells the user “That’s right! Try again!” and added the Random number code to generate a new number so the user can play again. 

Went one step further and created a method called makeToast that takes a String object as its parameters and will display a message to the screen. So when the makeToast function is called, it will display the appropriate message.

This was super fun and it was great to see how to further simplify code by creating the makeToast function. I didn't see it right away that it was possible, but with time I think I will get better at simplifying my code. 

### Day 14 & 15: July 3, 2019 4:00pm to 6:42pm
***Today's progress**
Worked with loops and classes. Created a number shapes app that is able to tell whether a number is triangular, sqaure, or both. 
Added other little snippets of code. Uploaded numberShapes to my repositories.

public class Loops {
    
    public static void main(String[] args){
        
        //counter variable that counts up from 1 to 10
        int x = 1;
        
        while(x <= 5 ) {
            
            System.out.println(2 * x);
            
            x++;
        }
        
        //for loop to print even numbers up to 10
        for (int y = 1; y <= 5; y++) {
            
            System.out.println(y * 2);
        }
        
        
    }
}

//for loop to print even numbers down from 10
        for (int y = 5; y > 0; y--) {
            
            System.out.println(y * 2);
        }


//display the first 10 numbers divisible by three
        int i = 1;
        
        while(i <= 30) {
            if(i%3 == 0) {
            System.out.println(i + " ");
            }
            i++;
        }
//first 10 numbers divisible by three
for (int i = 3; i <= 30; i= i + 3) {
            System.out.println(i);
        }

//display the first 10 triangular numbers
        
        int x = 1;
        int triangularNumber = 1;
        
        while (x <= 10) {
            
            System.out.println(triangularNumber);
            
            x++;
            
            triangularNumber = triangularNumber + x;
        }


//create an array holding family members' names
        String[] familyMembers = {"Nathan", "Sophia", "Elyse", "Dahlia"};
        
        //For each loop to loop through whole array
        //For variable name get it from familyMembers array
        for (String name : familyMembers) {
            
            System.out.println(name);
        }

//create an array holding family members' names
//declare data type of variables in the list <String> and after ArrayList
        List<String> familyMembers = new ArrayList<String>();
        
        familyMembers.add("Nathan");
        familyMembers.add("Elyse");
        familyMembers.add("Sophia");
        familyMembers.add("Dahlia");
        
        //For each loop to loop through whole array
        //For variable name get it from familyMembers array
        for (String name : familyMembers) {
            
            System.out.println(name);
        }
        

Classes:

public class Classes {
    public static void main(String[] args){
        
        class User {
            
           public int score;
           
           //method to return true or false whether user won the game
           //by having 100 points or more
           public boolean hasWon() {
               
               if (score >= 200) {
                   return true;
               } else {
                   return false;
               }
               
           }
            
        }
        
        //create instance/object of User type
        User bob = new User();
        
        bob.score = 10;
        
        //run hasWon method on bob
        System.out.println(bob.hasWon());
    }
}


public class Numbers {
    public static void main(String[] args){
        
        class Number {
            
            int number;
            
            public boolean isPositive(){
                if(number > 0) {
                    return true;
                } else {
                    return false;
                }
            }
        }
        
        //create new object of type Number
        Number myNumber = new Number();
        
        //set number to 7
        myNumber.number = 7;
        
        //testint to see if the number is positive
        //need parenthesis because it is a method
        if (myNumber.isPositive()) {
            
            System.out.println(myNumber.number + " is positive.");
            
        } else {
            
            System.out.println(myNumber.number + " is not positive.");
            
        }   
    }
}

### Day 16: July 4, 2019 
***Today's progress** 

Cross-Fading animation:
Created johnny photo that takes up the entire screen. Set onClick to the fade method.
//what you want to change and how long you want it to happen
//alpha value is how transparent the image is = 0 is invisible
//be clear the number is a float by putting an f after the value
//2000 is milliseconds
johnny.animate().alpha(0f).setDuration(2000);

Brought in a second image view and changed width and height to match parent. Set the onClick to be fade1. Created a new method to do the reverse so I can click on the image to go back and forth.

public void fade(View view) {

        ImageView johnny = (ImageView) findViewById(R.id.johnny);

        //Y is vertical axis and move by certain number of pixels
        //going to move him off the screen
        johnny.animate().translationXBy(2000f).setDuration(2000);

        //ImageView zimandgir = (ImageView) findViewById(R.id.zimandgir);
        //zimandgir.animate().alpha(1f).setDuration(2000);
        //zimandgir.bringToFront();

    }

TranslationX:

//move off the left side of the screen, use negative pixel
johnny.animate().translationXBy(-2000f).setDuration(2000);

Negative TranslationX:
//use animation to move a photo on screen and use alpha to set the transparency when the application is run
@Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        ImageView johnny = (ImageView) findViewById(R.id.johnny);

        //set off screen to the left,
        johnny.setTranslationX(-2000f);
    }
}

//but still using the fade method to bring the animation in from the left
        johnny.animate().translationXBy(2000f).setDuration(2000);
(-2000 when it is clicked to bring it in and 2000f translationX to send it off the screen)

//rotation to turn the animation upside down
        johnny.animate().rotation(180f).setDuration(2000);

scaleX:
//shrink down to have its size
        johnny.animate().scaleX(0.5f).scaleY(0.5f).setDuration(2000);

### Day 17: July 9, 2019 7:00pm to 8:00pm
***Today's progress** 
Make sure your pictures are in the drawables folder. Make sure they are a good size. 
If you get an error RuntimeException Canvas: trying to draw to large (mem size) bitmap, then your pictures are too large.
Created images in paint of my boyfriend and stepdaughter and saved as png. Saved to desktop and added them to drawables folder.
Had to resize the images to 100x120 to use and copy paste them into the drawable folder instead of deleting them and overwrote them

Updates: help – whats new in android studio

Got my game and board set up. Changed the bottom margin to move the board down. Had to manually enter the layouts to center them inside the board. Changed the grid layout to 3x3 in the xml. 

Had to do a lot of research to find out why I was getting that error. Stackoverflow helped me find my answers. 

Got the animation working, just can’t get the rotation to work. 

### Day 18: July 11, 2019 7:00pm to 8:00pm
***Today's progress** 
Worked with SQL and NoSQL queries and data storage creations. Queries:

//create person table
create table person( 
person_ID INT(50) NOT NULL AUTO_INCREMENT,
lastName varchar(50) not null,
firstName varchar(50) not null, 
relationship varchar(255),
PRIMARY KEY (person_ID)
);

//create phone table
create table phone(
phone_number int(10) not null,
phone_type varchar(20), 
person_ID int(50) not null,
primary key (phone_number)
);

//insert data into person
insert into person (lastName, firstName, relationship) 
values 
('Smith', 'John', 'Father'),
('Smith', 'Sandy', 'Mother'),
('Summerson', 'Nathan', 'Boyfriend'),
('Segebart', 'Elyse', 'Girlfriend'),
('Gill', 'Finn', 'Cousin')
;

//insert data into phone
insert into phone(phone_number, phone_number2, person_ID, phone_type)
values
(5154785901, 5154785902, 1, 'cell'),
(5153224567, 5153224987, 2, 'work'),
(5151114900, 5151113456, 3, 'home'),
(5155559000, 5156652341, 4, 'cell'),
(5159991532, 5159991234, 5, 'work');

//run a join on one person
select * from person 
inner join phone 
on person.person_id = phone.person_id
where person.person_ID = 1;

//create person documents
db.person.insert({
"_id": personId,
"last_name" : "Segebart",
"first_name" : "Hannah",
"relationship" : "Sister"
});

//create phone documents

db.phone.insert({
person_id : personId,
phone : {
phone_type : "Cell",
phone_number : "987-765-5432"
}}); 

//create person documents embedded
db.person.insert({
"last_name" : "Smith",
"first_name" : "Anne",
"relationship" : "colleague",
"phone" : [
{ "phone_type" : "Business", "phone_number" : "111-222-3333" },
{ "phone_type" : "Home", "phone_number" : "222-333-4444" },
{ "phone_type" : "Cell", "phone_number" : "444-555-6666" }
]
});

//embedded

db.person.insert({
last_name: "Segebart",
first_name: "Hannah",
relationship: "Sister",
phone: [
{phone_type: "Business", "phone_number": "987-765-5432"},
{phone_type: "Home", "phone_number": "987-654-3210"},
{phone_type: "Cell", "phone_number": "123-444-5555"}
]});

### Started ROUND 1 ###
### Day 0: December 26, 2019
#####

**Today's Progress**:
Worked on Java with Code Gym CC. Completed several levels including problems to find the min of two numbers, the min of three numbers, and the min of 4 numbers that uses the min(a,b) function. 
/* 
Minimum of three numbers

*/
public class Solution {
    public static int min(int a, int b, int c) {
        int n = 0;
        if(a <= b && a <= c){
            n = a;
        } else if (b <= a && b<= c){
            n = b;
        } else if (c <= a && c <= b){
            n = c;
        } else {
            System.out.println("We don't have a min. Why not?");
        }
        return n;
    }

    public static void main(String[] args) throws Exception {
        System.out.println(min(1, 2, 3));
        System.out.println(min(-1, -2, -3));
        System.out.println(min(3, 5, 3));
        System.out.println(min(5, 5, 10));
    }
    
Min of four numbers: 
/* 
Minimum of four numbers
For this problem I struggled with how to incorporate the min(a,b) function. With the three, I was just making comparisons
and could use logical operators. This is essentially the same type of pattern with ab ac ad but I am using the min function 
to compare if the min of the two is equal to a, then b, then c, then d. I assigned the values to the variable n so I could return
it when comparisons were finished.
*/
public class Solution {
    public static int min(int a, int b, int c, int d) {
        int n = 0;
        if (min(a,b) == a && min(a,c) == a && min(a,d) == a) {
            n = a;
        } else if (min(b,a) == b && min(b,c) == b && min(b,d) == b) {
            n = b;
        } else if (min(c,a) == c && min(c,b) == c && min(c,d) == c) {
            n = c;
        } else if (min(d,a) == d && min(d,b) == d && min(d,c) == d) {
            n = d;
        }
        return n;
    }

    public static int min(int a, int b) {
        if(a < b) {
            return a;
        } else {
            return b;
        }
    }

    public static void main(String[] args) throws Exception {
        System.out.println(min(-20, -10));
        System.out.println(min(-20, -10, -30, -40));
        System.out.println(min(-20, -10, -30, 40));
        System.out.println(min(-40, -10, -30, 40));
    }
}

### Day 1: December 27, 2019
#####

**Today's Progress**:
Continued playing CodeGymCC to learn Java. Worked through a factorial return program where I had to return the product of the numbers 1-10. Another program to display the sum of 5 numbers on each line with the next line adding the next number to it. 

Also, I had to use a class's properties to create 12 different objects and use the name attribute to name them all using dot notation and the setter for name. 

Solved another challenge with how many liters are needed to fill a pool. I had to research how many liters were in a cubic foot. I think I am becoming better at reading the code and understanding what is happening between the methods. I am getting back in the groove of coding. This is some basics understanding that I think I had a few gaps in. However, I am surprising myself with how much I have retained when I had to pull the factorial information out of my brain and still remembered the equation for it.

   System.out.println(convertToSeconds(20)); <-- this is really important to me right now because I just remembered it for the first time that I can do this when I need a method to return something and it is void and shouldn't display anything. Yay!

