Challenge 3: Get Your Hands Dirty
=================================
Next up, find the Lynda.com video series entitled: “Objective-C Essential
Training”. Watch each video in the following list and answer the corresponding
question.

Section 1: Getting Started
==========================
[1.1] Installing the tools (4:42)
---------------------------------
You should already have Xcode installed, but you will need to register as an
Apple Developer.

Do you like cats?

I actually have one, so the answer is yes by default.


[1.2] Creating your first application (11:28)
---------------------------------------------
Create your first application using the same steps Simon describes in the video.
Familiarize yourself with the Xcode environment, specifically notice how it can
be manipulated to display different helper tools and how it will attempt to fill
in your code as you type it.

No issues with starting apps here.



[1.3] Updates to this course (3:31)
-----------------------------------
Why do you think it's important to be aware of the idiosyncracies with older
versions of Objective-C and to keep up with new features as they are added?

Since Objective-C is a living language, updates to the libraries and the code both for simplicity and functionality are consistently occurring. Also, noticing the switch from the older "square bracket" style to the newer syntax is important for references to older code and other materials that will be used for learning.


Section 2: Objective-C Basics
=============================
[2.1] The Objective-C language (4:11)
-------------------------------------
How did Objective-C become the language to learn if you want to make apps for
the iPhone and iPad?

Instead of other languages which were influence by the original C language, Objective-C still uses C as its base language. The Objective-C part of C is actually built on top of original C when it was first utilized by NeXT in the late 1980s. Apple ended up absorbing NeXT and utilizing Objective-c for their future operating systems including for devices such as iPhone and iPad. 

[2.2] The structure of an Objective-C program (6:15)
----------------------------------------------------
Create a new project. Go to the menu option `Xcode`, `Preferences`,
`Text Editing` and make sure *Line Numbers* is checked in the section marked
"Show." Then add comments describing the purpose of each auto-generated line in
the main.m file. For example on Line 17 I would write: 

```
NSLog(@"Hello, World!");  // instructs the console to output: Hello, World!
```

Done and done.

[2.3] Compiling and running your code (8:37)
--------------------------------------------
Why might you build in one version of iOS but deploy in an older version?

You may want to test your application's functionality on older operating systems to ensure that it works properly for older devices or for users who do not update as frequently as they should.



Section 3: Program Flow
=======================
[3.1] Logging messages to the command line (6:07)
-------------------------------------------------
Following the example in the video, write a program that calculates and outputs
to the console the number of seconds in ten years. Copy and paste your code
here.

int main(int argc, const char * argv[])
{

    @autoreleasepool {
        
        // insert code here...
        int seconds = 60;
        int minutes = 60;
        int hours = 24;
        float days = 365.25;//leap year
        
        int secondsInTenYears = 10 * seconds * minutes * hours * days;
        
        NSLog(@"There are %i seconds in ten years.", secondsInTenYears);
        
    }
    return 0;
}


[3.2] Writing conditional code (7:01)
-------------------------------------
Using Objective-C, create an integer variable called "day" that represents the
days of the week. Write an if statement that checks whether "day" is a weekend
day. If the day is a weekend day then have your program print a message saying
"Have a nice weekend!" and if it's not, print a message saying "I hope you're
having a good week!"

@autoreleasepool {
        
        int day = 0;
        NSLog(@"Please state the day of the week with an integer.");
        NSLog(@"1 - Sunday");
        NSLog(@"2 - Monday");
        NSLog(@"3 - Tuesday");
        NSLog(@"4 - Wednesday");
        NSLog(@"5 - Thursday");
        NSLog(@"6 - Friday");
        NSLog(@"7 - Saturday");
        do {
            scanf("%i", &day);
            if (day == 1 || day == 7) {
                NSLog(@"Have a nice weekend!");
            } else if (day == 2 || day == 3 || day == 4 || day == 5 || day == 6 ) {
                NSLog(@"I hope you're having a good week!");
            } else {
                NSLog(@"You chose an invalid integer! Please choose again.");
            }
        } while (day < 1 || day > 7);
    }
    return 0;

[3.3] The switch statement (5:58)
---------------------------------
Create a variable called "hurricaneCategory" and a switch statement that prints
out a message describing a hurricane's category from 1-5.

@autoreleasepool {
        
        int hurricaneCategory = 0;
        NSLog(@"Please state the hurricane type (1-5).");
        
        do{
            scanf("%i", &hurricaneCategory);
            switch (hurricaneCategory) {
                case 1:
                    NSLog(@"Category 1 hurricane.");
                    break;
                case 2:
                    NSLog(@"Category 2 hurricane.");
                    break;
                case 3:
                    NSLog(@"Category 3 hurricane.");
                    break;
                case 4:
                    NSLog(@"Category 4 hurricane. Uh oh.");
                    break;
                case 5:
                    NSLog(@"Category 5 hurricane. We are screwed.");
                    break;
                default:
                    NSLog(@"You chose an invalid integer! Please choose again.");
            }
            
        } while (hurricaneCategory < 1 || hurricaneCategory > 5);
    }

[3.4] Code snippets (5:15)
--------------------------
Grab a code snippet, indent it to match the indent of your project, then add
comments to it, then select the entire snippet you just modified and save it as
your own code snippet. Time yourself and record how many seconds it takes you to
do all this.

It took me about 25 seconds. That was pretty sweet.


[3.5] Operators and expressions (11:08)
---------------------------------------
List the 6 types of operators described in this video. Provide their name, a
description of their meaning, and the syntax you would use to execute them. What
code snippet does the ternary operator replace?

Arithmetic operators are standard math operations that follow the same rules learned in basic math courses (ex. order of operations).
Comparison operations are used in conditional statements for returning a boolean answer (Yes or No). These act as gatekeepers for loops and other conditionals where if the operation returns a "Yes", the following code procedures are followed.
Modulus operators are used for finding the given remainder of a division operation. This is useful for math operations where division of integers does not return an integer quotient.
Increment/decrement operators will perform a unary operation to a value either adding or subtracting by one.
Prefix/Postfix operators are increment and decrement operators where the operations can be performed before or after the line of code is read.
Ternary operators are statements with three conditions. This can be used as a shortened conditional statement saving on lines of code.


[3.6] Loops (8:53)
------------------
Think of a scenario while using a mobile app that might require you to use a
"continue" statement in the middle of a loop.

If there was an array with a non-assigned variable for one of the index points, a continue statement may be used to skip over that empty variable.

[3.7] Functions (10:16)
-----------------------
What is a function? What is a function prototype? What are the purposes of each?
What are the rules for when and how you can call a function?

A function is a reusable section of code that can take parameters and can return a specific value type. A function prototype is a statement giving the generals about a function to notify the compiler that this function exists. Functions can only be called if they havve been already compiled or if a function prototype has been created before the function is called.


Section 4: Variables
====================
[4.1] Data types (7:06)
-----------------------
What are the primitive data types in Objective-C? Why did Apple add a set of
classes to handle other data types?

The primitive data types in Objective-C are:
int, double, float, char, BOOL. Apple created a set of classes, modifiers and composite data types that is part of the Objective-C framework that works off of the core primitive data types. 


[4.2] Working with numbers (9:33)
---------------------------------
Make a table of Objective-C primitive data types. Add numeric data types and
their properties to this table.

int:	 			4 bytes		−2,147,483,648 to +2,147,483,647
unsigned int:		4 bytes		0 to 4,294,967,295
long int (64-bit):	8 bytes		−9,223,372,036,854,775,808 to +9,223,372,036,854,775,807
short int: 			4 bytes		-32,767 to 32,768

float: 				4 bytes		
double:				8 bytes		Can handle a number twice the size of a float.

char:				1 byte		Any ASCII character
BOOL:				1 byte			YES or NO



[4.3] Working with characters (4:39)
------------------------------------
Add char and BOOL (the character data types) to your table created above.

**ANSWER ABOVE!**

[4.4] Variable scope (8:06)
---------------------------
Describe in your own words what the scope of a variable is in Objective-C

Variables are automatically local, meaning that they exist only within the statement block that they are defined in. To make a variable value available outside of a statement block, the variable must be defined as a global variable outside of the block or a copy must be made by a function or another variable.



[4.5] Enumerations (3:35)
-------------------------
What does the `enum` keyword allow you to do?

The keyword enum allows you to enumerate a strict set of values for selections needed for a program. Since the value is stored as an integer, it does the enumeration piece for you without the extraneous code.

[4.6] Using typedef (2:17)
--------------------------
When would you define your own data type versus using an enum?

If a enumerated variable was going have values that were going to be constantly updating and changing, then defining a data type using typedef would be recommended.

[4.7] Preprocessor directives (5:56)
------------------------------------
Describe the three common preprocessor directives, `#import`, `#define`, and
`#if DEBUG`. Come up with one example where you would use each.

The #import directive finds a library, class or some other grouping of code and makes it available to the application. This directive is essential when writing new classes for your application.

The #define directive will create a variable of an unchanging value to be utilized anywhere throughout the application. This directive is used for values that are set at the initialization of an application and will always start at that value.

The #if DEBUG chooses to run a specific block of code only when we are in debug scheme mode. This is helpful for writing diagnostic messages throughout the code that would only run when testing an application, but would not need to be removed upon release.


[4.8] Working with strings (7:52)
---------------------------------
Define the same string using both NSString and C-style string syntax. Describe
the purpose behind each part of your definition.

In traditional C, a String is really defined as an array of characters. (ex. char a[] = "hello";)

In Objective-C, a String is a prebuilt object that is created and defined using a pointer that allocates the necessary space for the needed characters. (ex. NSString * a = @"hello";)


Section 5: Classes
==================
[5.1] Introduction to object orientation (7:36)
-----------------------------------------------
Create an encapsulated (including generalized attributes and behavior)
description of a `MobileMakersParticipant` class. Instantiate a single object
representing yourself as a member of this class.

class MobileMakersParticipant
Attributes - firstName, lastName, address, phoneNumber, email, grade,
Behavior - pay(), turnInAssignment(), findGrade(), attendance()

MobileMakersParticipant *matthewVoracek [[MobileMakersParticipant alloc]init];

[person setLastName:Matthew];
[person setFirstName:Voracek];
[person setAddress:237 Forestway Drive];
[person setPhoneNumber:7736126284];
[person setEmail:mjvoracek@gmail.com];
[person setGrade:A+];


[5.2] Using objects and pointers (6:38)
---------------------------------------
What is the pointer’s role in instantiating an object from a class? How is a
pointer different than a primitive?

The pointer references to the memory address and allocates the necessary space needed for the new object. THis makes the act of allocating the memory needed more flexible and allows for changes to the object that are less taxing. Since primitive data types already have set memory allocation and strict parameters for what values can be given, the asterisk is not needed as a pointer.

[5.3] Messages and methods (6:44)
---------------------------------
What is the main difference between Objective-C’s messages and method calls in
other languages? How can this difference be seen as an advantage while
programming?

Objective-C uses square brackets instead of dot syntax to call methods to indicate to the complier that we are using that new language. Also each method call and parameter is stated explicitly within the the square brackets. This can be advantageous for developers so they can keep track of the method that is attached to each parameter. 

[5.4] Using existing classes in the foundation framework (8:40)
---------------------------------------------------------------
What's the difference between a class method and an instance method?

Instance methods are designed only to work on the specific instance of that class. Class methods are defined to work on the entire class rather than a specifc instantiation.

Try typing "NSD..." into your code window. Use the autofill feature and select a
single class name that starts with those three letters. Once the name has been
auto-completed, use the handy shortcut (Option + click) and investigate the
class whose name just got printed to the screen. Examine the task list for this
class. Do this a few more times until you're familiar with the process, or until
you've exhausted your curiosity, whichever comes last.


Section 6: Memory Management
============================
[6.1] What's new with memory management? (1:45)
-----------------------------------------------
Let it soak in. No questions for this one.

I am well soaked.


[6.2] Memory management in Objective-C (6:58)
---------------------------------------------
What is the relationship between a pointer to an object, a block of memory, and
the owning and releasing process. Can you come up with an analogy for this
relationship?

For any object, a pointer is the address to the block of memory that holds that object. The memory is then allocated, used, updated and released by the owner, creator of that object. An analogy for this could be making a reservation for a restaurant. Your space in that restaurant is "held" not unlike the memory space for a an object. When you arrive, are seated and order, you are utilizing your reservation not unlike an object uses methods. Paying the bill is your "release" from that reservation. If you leave without paying, then that reservation does not complete, not unlike a dangling pointer. If you never leave the restaurant, then other reservations cannot be filled which is like a memory leak. Kind of clunky, but it was the best I could come up with right now. 

[6.3] Object creation (7:31)
----------------------------
What does the new method do when used to create an object instance of a class?
Why do we avoid using this method? How long is an object's lifetime?

The new method when used to create an object instance is a class method, not an instance method. If the new method was used to create an object, then you would not have the various init methods that are often available when creating an object. The lifetime of an object is either for the lifetime of the program or until the object is released. 


[6.4] Using autorelease pools (5:14)
------------------------------------
How does the autorelease pool work? How and when can you use it deliberately?

The autorelease pool is an active list that contains all of the objects created by the application. As a convenient tool, it can hold all of the created objects until the keyword 'drain' is used to empty the pool. It is best used when instantiating and returning an object. An autorelease would assure that the release of this object will occur at a necessary point in the future.


[6.5] Apple autoreleased objects (3:39)
---------------------------------------
What does ARC stand for? Why is it important to remember this?

ARC stands for Automatic Reference Counting, which is a way of keeping track of objects and goes through the job of automatically releasing them from our program at the most necessary points. This is important and ultimately helpful so that iOS developers do not need to write release calls any longer. In fact, XCode will not allow you to write a release code when in ARC mode.

[6.6] Introduction to Automatic Reference Counting (ARC) (4:43)
---------------------------------------------------------------
What does ARC save us from having to do? How does it keep us from having to make
this extra effort?

ARC helps in that iOS developers do not need to write release calls any longer. In fact, XCode will not allow you to write a release code when in ARC mode. Instead it writes the code out for us upon compilation. 

[6.7] What ARC manages (2:42)
-----------------------------
What are the differences between ARC and garbage collection? What makes these
differences advantageous?

ARC runs at compile-time and finds the release points accordingly rather than garbage collection which performs its duities during runtime. This helps by not having to run in the background of an application and untimately saving on processing. 

[6.8] The rules of ARC (4:20)
-----------------------------
Why can you not release or dealloc memory when working with ARC?

Because ARC automatically does this and any code performing these methods will cause immediate errors. SO, basically, stay out of the way.


Section 7: Custom Classes
=========================
[7.1] Creating your own classes (14:01)
---------------------------------------
What are the two different sections used to create a class? What do they hold
and what files are they placed in?

The interface file is a general listing of the basic attributes and operations of a given class. The implementation file of a class is where the code is held for the actual performance of the listed methods and other properties available to the calling application.
    
**Challenge!** Create a Tweet class for a twitter style app.

[7.2] Defining methods (8:36)
-----------------------------
**Challenge!** Define what should get passed in and what should get returned by
each of your methods in your Tweet class above.

I definitely prefer the openness and anonymity of Twitter to the restrained rehash of cat videos that happens on Facebook.

[7.3] Defining properties (7:21)
--------------------------------
How did Objective-C programmers handle instance variables before 2012? How are
they handled now? What got easier and what got obscured?

Before recent updates to Objective-C, instance variables of classes were declared in braces under the class and written with getter and setter accessor methods that performed the duties of either setting a variable's value and getting it when needed. Now, these methods and declarations are handled by an @property methods eliminating the extra work of writing code. The @property makes the whole act simpler while the complier does this work unseen. 

[7.4] Defining initializers (12:30)
-----------------------------------
What are initializers and why do we need to use them? Describe a situations when
you can rely on the standard `init` method and when you have to create your own
custom initializer.

When creating an Object in Objective-C, first space needs to be allocated and given a pointer to that space. Next, initialization is needed to set the apporpriate type of each instance variable and given a meaningful value.

In situations where the instance variables of a class are never standard, then the init method given with the creation of any object is suitable. However, if we need the variance between different set values of your instance variables, then custom made initializers that are suited to the various needs of the application are necessary. 

[7.5] Using dealloc (5:33)
--------------------------
Why can we have a dealloc method in a class when using ARC, but we can't call
dealloc manually oursevles when using ARC?

When using ARC we can not call dealloc because that method is controlled by ARC and finds the appropriate time to release that memory at compile time. If initialization is holding onto something that needs to be dealt with before the object is deallocated, then a dealloc method can be wriiten.


Section 8: Collections
======================
[8.1] Working with C-style arrays (7:12)
----------------------------------------
What are the three constraints when using C-style arrays? Create a C-style array
that holds the days of the week.

There are no bounds checking by the complier, so array calls written for space that has not been proerly allocated with result in no errors from the complier. Also, the size of the array is fixed upon creation so no members can be added or removed. Finally, an array can only by of one type.

NSString * daysOfTheWeek[] = {@"Sunday", @"Monday", @"Tuesday", @"Wednesday", @"Thursday", @"Friday", @"Saturday"};

[8.2] Working with Objective-C array objects (8:00)
---------------------------------------------------
What is the difference between a mutable and an immutable array?

NSArray is immutable, or unchangable, meaning that objects cannot be added or tremoved from the array. To create a mutable array, we can use the NSMutableArray class.

**Challenge!**
Create an immutable array containing the days of the week. Create a mutable
array that contains the days of the week that you will be at Mobile Makers. Add
the days of the week from the immutable array to the mutable array.

NSArray * daysOfTheWeek = [NSArray arrayWithObjects:@"Sunday", @"Monday", @"Tuesday", @"Wednesday", @"Thursday", @"Friday", @"Saturday", nil];

NSMutableArray * mobileMakersSchedule = [NSMutableArray arrayWithObjects:daysOfTheWeek[1], daysOfTheWeek[2],daysOfTheWeek[3], daysOfTheWeek[4],daysOfTheWeek[5], nil];

[8.3] Using dictionaries (5:55)
-------------------------------
Create a dictionary that lists five or more events in your life and the
accompanying year (or date if you want to get fancy) of the event.

NSDictionary *lifeEvents = [NSDictionary dictionaryWithObjectsAndKeys:
            @"graduated high school.", @"June 1989",
            @"moved to London.", @"September 1996",
            @"got married.", @"July 1999",
            @"had a baby.", @"March 2007",
            @"became an iOS developer.", @"March 2014",
            nil];
        

[8.4] Fast enumeration (3:27)
-----------------------------
Use fast enumeration to log the timeline of the life events you described above
to the console.

for (NSDate * year in lifeEvents){
            NSLog(@"%@ was when I %@",year,[lifeEvents objectForKey:year]);

Section 9: File Management
==========================
[9.1] Introduction to file management in Objective-C (6:44)
-----------------------------------------------------------
What can you do with files using the methods you are aware of that are available
in Objective C’s Foundation class?

Using the methods available in the FileManager class, files can be accessed, read, saved, removed, found by its directories, access its attributes and checked for its existence.

[9.2] Working with paths and URLs (7:17)
----------------------------------------
What are the three parts of a URL? What are the advantages to using NSURL?

The three parts of a URL address is the scheme, domain and path. The NSURL class can catch errors, usable across classes and runs faster than a String object.

[9.3] Reading and writing strings (4:38)
----------------------------------------
What would be a reason you would want to write a string to disk instead of just
keeping it memory?

Just a guess, but if a String is quite long it would take up a lot of space needed to run the application. Keeping a String in a separate file would only make it in use while being accessed. 

[9.4] Archiving objects (12:41)
-------------------------------
Why would you want to archive an object instead of writing the data to disk
using the techniques discussed previously?

Archiving objects is a quicker and more convenient method of taking variables of different types and encoding them so that are organized and can be be decoded and accessed easily.


Section 10 - More Complex Classes
=================================
[10.1] Inheritance and NSObject (8:13)
--------------------------------------
How can you determine what methods you're inheriting from a super class? How do
you overide a method inherited from a super class?

When performing option-click on the class name, the class reference can be researched for the available methods for that class. To override the given method of a super class, a reference key word super may be utilized in the class implementation. For all overrides, the new method is written using the same signature as what is used in the super class then adding new code ready to be utilized.

[10.2] Extending classes with categories (6:31)
-----------------------------------------------
What is the difference between a category and an inheritance? What are the
limitations of using a category?

Instead of creating a new sub class that inherits from an established super class, using categories will create methods as if the super class had these methods from the start. The limitations on categories are that new instance variables cannot be added to them.

[10.3] Defining protocols (5:14)
--------------------------------
How are protocols useful?

Protocols can be useful in finding a general interaction between objects that has the desired method needed without the formality of creating an inheritance.

[10.4] Dynamic typing (11:33)
-----------------------------
What are the advantages and disadvantages to dynamic typing?

Dynamic typing works for situations where the application is receiving object information from an unknown source and needs to accept the incoming data without knowing the internal workings of that data. When that data is needed for that application, dynamic typing uses polymorphism to get the general object methods without needing to know more than the object name. THe disadvantages to ddynamic typing is the lack of knowledge of what is involved in the incoming data, so it does not allow for the compile time assurance checking that goes with static typing. 

