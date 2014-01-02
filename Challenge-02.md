From the Lynda.com video series “Foundations of Programming: Object-Oriented
Design”, watch each (short) video and answer the correlating questions:


Section 0: Introduction
=======================
[0.1] What to expect from this course (3:06)
--------------------------------------------
What is the intended purpose and potential advantage of learning object oriented
design?

Object oriented design is a methodology to creating an application that helps with your pre-coding analysis and the actual construction of your coding so that it runs cleaner, has less issues and can be flexible enough to accommodate updates and adaptations.

[0.2] Exploring object-oriented analysis, design, and development (1:41)
------------------------------------------------------------------------
Why might it be advantageous to analyze and design before beginning programming?

The analysis and design stage of programming is essential to building an application. Without first understanding what needs to be done and planning the steps and necessary pieces of your application, the building part of object-oriented programming will surely be slower with more mistakes and less successful in the end.

[0.3] Reviewing software development methodologies (4:08)
---------------------------------------------------------
What is the difference between a "waterfall" and an "agile" approach to
development? What is an iteration and how do we to use them to build software?

A waterfall approach to development works in stages where each step is fully completed before beginning the next step. An agile approach is more flexible, allowing for new requirements, fresh ideas and unforeseen problems to be a possibility and to revisit previous steps while still completing other parts of the application. An iteration is a cycle of the object-orientation process where a new requirement is added, analyzed, considered and built into the previously created program. 


Section 1: Core Concepts
========================
[1.1] Why we use object-orientation (2:42)
------------------------------------------
What are the various types of programming languages and in which domain is each
used?

Early in programming, procedural languages were used in mainframes until programs became more lengthy and complicated. Object-oriented languages were created to make programs run more efficiently. There are some other specific types of OO languages used for specialized functions, but most of these language types are used for practical, mainstream applications.


[1.2] What is an object? (5:22)
-------------------------------
Describe in your own words the three properties of a computing object.

A computing object has characteristics or attributes that give the object its uniqueness. Also, a computing object is self-contained or has an identity separate from other objects even if the object is created by the same group of code and shares the same attributes. Finally, computer objects have behaviors or can perform specific tasks aligned to that object not unlike how a noun can carry out a specific verb.


[1.3] What is a class? (4:43)
-----------------------------
Explain how classes are analogous to blueprints. Include the relationship
between a class and an object. Can you think of how the analogy breaks down?

Like a blueprint, classes are detailed descriptions of an object that gives it its overall characteristics and behaviors. In OO programming, the class gives all of these characteristics and behaviors to an object while creating an instance of that object. This instantiation is where a class breaks away from the utilization of a blueprint.  


[1.4] What is abstraction? (2:45)
---------------------------------
When a developer uses the term “abstraction” what are they describing?

A developer uses abstraction to focus on the essentials of an object rather than the specific attributes. Abstraction also ignores the irrelevant characteristics that do not apply to the object in question.


[1.5] What is encapsulation? (3:45)
-----------------------------------
What does encapsulation prevent? What does it enable?

Encapsulation prevents data from being available to different parts of the application. This enables protection of the data from inside the object while reducing the dependence throughout the program to minimize changes and making for smoother operation.


[1.6] What is inheritance? (3:35)
---------------------------------
Describe the inheritance relationship between classes. When would this
relationship be advantageous to establish?

When a subclass inherits from another superclass, it takes all of the methods and attributes from the superclass while being able to create its own attributes separate from the superclass. When a change is made in the superclass, it also applies to the subclasses without needing to update multiple objects.


[1.7] What is polymorphism? (3:22)
----------------------------------
What is the basic idea behind polymorphism? How can it make the classes we
create more flexible?

Polymorphism means that inherited attributes from the superclass by a subclass can be adapted or overridden to suit the needs of the new subclass. It makes them more flexible by being able to adapt an attribute or method automatically based on the object type.


Section 2: Object-Oriented Analysis and Design
==============================================
[2.1] Understanding the object-oriented analysis and design processes (4:13)
----------------------------------------------------------------------------
What are the steps of analysis that come before writing code for an application?
Why do you think these steps make writing the code easier?

Before starting to build an application, a team must gather requirements and describe the application and its utilization based on the discovered information. Next comes identifying the main classes and describing the interactions based on the requirements. Finally everything comes together in a class diagram that is constantly revised and adapting based on changing needs and issues that were not considered previously. 

These steps help code writing by giving the process forethought and consideration, then gradually building a visual framework that can be utilized and adapted as the application goes through new iterations.


[2.2] Defining requirements (6:09)
----------------------------------
What should you have after you've completed the first phase of defining your
requirements?

After completing the first phase of defining your requirements, there should be the minimum amount needed to give the application its function and state its usability and acceptable level of reliability which is a basis for the agile approach to OO programming.


[2.3] Introduction to the Unified Modeling Language (UML) (1:54)
----------------------------------------------------------------
What is UML? Why Is it useful to visualize your application before coding it?

UML, or unified modeling language, is a graphic method used for drawing diagrams of a system used in object oriented programming. It is useful to the development process to have a general sketched layout of your application that can be easily manipulated and updated as needed.


Section 3: Utilizing Use Cases
==============================
[3.1] Understanding use cases (6:11)
------------------------------------
Write a use case for creating an event on your phone's calendar.

Title: Create a new event in the calendar
Actor: User (who is creating the event)
Scenario: 	1. User opens application.
		2. User touches the “plus sign” in the upper right hand corner
		3. User enters Title (if desired)
		4. User enters Location (if desired)
		5. User toggles all-day switch (if desired)
		6. User updates the start date and time as needed
		7. User updates the end date and time as needed
		8. User chooses a repeat selection (if desired)
		9. User adds invitees to the event (if desired)
		10. User chooses an event alert selection (if desired)
		11. User selects an alternative calendar (if desired)
		12. User chooses a “Show As” selection (if desired)
		13. User enters a URL link (if desired)
		14. User enters Notes for event (if desired)
		15. User touches Done to complete the new event.
		

[3.2] Identifying the actors (4:16)
-----------------------------------
Can you think of a use case for a mobile application in which the actor is not
the user of the mobile device?

Using the example above, an invitee to the event would be an actor based on the user inviting them to a new event. 


[3.3] Identifying the scenarios (5:07)
--------------------------------------
Write another use case for a mobile device user interacting with a calendar
application. This time include a couple extensions when crafting your scenario.

Title: Create a new event in the calendar
Actor: User (who is creating the event)
Scenario: 	1. User opens application.
		2. User touches the “plus sign” in the upper right hand corner
		3. User enters Title (if desired)
		4. User enters Location (if desired)
		5. User toggles all-day switch (if desired)
		6. User updates the start date and time as needed
		7. User updates the end date and time as needed
		8. User chooses a repeat selection (if desired)
		9. User adds invitees to the event (if desired)
		10. User chooses an event alert selection (if desired)
		11. User selects an alternative calendar (if desired)
		12. User chooses a “Show As” selection (if desired)
		13. User enters a URL link (if desired)
		14. User enters Notes for event (if desired)
		
		Extension: Complete and save event
		15a. User touches Done to complete the new event.

		Extension: Cancel event
		15b. User touches Cancel to cancel the new event.


[3.4] Diagramming use cases (4:18)
----------------------------------
Do a google image search for "use case diagram." Notice how many variations
there are. What do they all generally have in common?

Although there are different styles of use case diagrams, there are generally ellipses representing use cases and stick figures representing users. The use cases are connected to each other and users by lines and/or arrows representing the available interactions.


[3.5] Employing user stories (3:43)
-----------------------------------
Write 5 user stories to describe a mobile user interacting with his or her maps
application.

1. As a user, I want to enter my home address so I can get directions based on it.
2. As a user, I want to save an address so I can refer to it quickly and simply.
3. As a user, I want to be able to see traffic on the map so I can avoid it.
4. As a user, I want to know the estimated amount of time my trip will take so I can plan accordingly.
5. As a user, I want to be able to see public transportation stations so I can find them easily.


Section 4: Domain Modeling (Modeling the App)
=============================================
[4.1] Creating a conceptual model (1:59)
----------------------------------------
What’s your favorite color?

Blue! No, yellow! Augggh!

[4.2] Identifying the classes (2:27)
------------------------------------
Identify the classes in the use case you constructed for a user interacting with
his or her calendar application in chapter 3.

Objects: User, Event, Calendar, Date (all others are attributes or methods)


[4.3] Identifying class relationships (2:38)
--------------------------------------------
Identify the relationships among the classes you found above. Create a
conceptual model where you diagram these relationships and then upload a picture
of your model below.

I created a link to this Google Doc. I hope this is good enough? 

https://docs.google.com/drawings/d/1Om8a-Q4P9UiNln-Dvu7wGh85kP5X2tzhujBpRxWgjlo/edit?usp=sharing


[4.4] Identifying class responsibilities (6:43)
-----------------------------------------------
Identify the responsibilities of the classes you found above. List them here.

Event responsibilities: Display Title, Display Location, Get All-Day switch, Display Start Date, Display Start Time, Display End Date, Display End Time, Get Repeat Setting, Display Calendar Used, Get Event Alert, Display Invitees, Display Show As Status, Display URL Link, Display Notes

Calendar responsibilities: Display Date, Display Event, Display Name

Date responsibilities: Display Event, Display Time


[4.5] Using CRC cards (2:49)
----------------------------
If you’d like, try creating CRC cards for the model you made above. There's no
need to respond here, just try it out and see if you like this form of
organization.

I would like to try using a UML program or freeware with the recommendation of those who know more than I do.


Section 5: Creating Classes
===========================
[5.1] Creating class diagrams (6:11)
------------------------------------
Construct Class Diagrams for the classes you imagine exist in a twitter app, a
maps app, a calendar app, or any other app you would like to make. Do you find
that it is easier to come up with the attributes or with the behaviors? Why do
you think that is?

Class Name: Event
Attributes: title: String, location: String, allDay: Boolean, startDate: Date, startTime: Time, endDate: Date, endTime: Time, eventRepeat: Char?, eventAlert: Alert?, invitee: String, showAs: Boolean, linkURL: String, notes: String
Operations: getName():String, getLocation():String, setAllDay(Boolean), getStartDate():Date, setStartDate(Date), getStartTime():Time, setStartTime(Time), getRepeat():char, getCalendar():Calendar, getAlert():Alert, setAlert(Alert), getInvitees():String, getShowAs(Boolean), getLink():String, getNotes():String, displayEvent(),

Class Name: Calendar
Attributes: Name: String, Date: Date, Event: Event
Operations: getDate():Date, getEvent():Event, displayCalendar()

Class Name: Date
Attributes: Event: Event, Time: Time, Calendar: Calendar
Operations: getEvent():Event, getCalendar(): Calendar, getTime():Time, displayDate()

It is seemingly easier to create attributes right now as they can be more easily visualized as objects. Operations are more varied based on their action rather than their tangible aspect. 



[5.2] Converting class diagrams to code (4:57)
----------------------------------------------
How might the separation of interface and implementation in Objective-C be an
advantage when working with class diagrams?

Separating the interface and implementation in Objective-C shows the interface as what exists or an attribute and the implementation as what is being done or the operation. 

[5.3] Exploring object lifetime (5:55)
--------------------------------------
What are the constructors and destructors in Objective-C? Why do we use them?

In Objective-C, they key words alloc and init are used to create and construct an object rather than the new keyword. We use these keywords to instantiate and allocate memory for the object. To construct an object, we would need to create a method that gives a value to the outstanding variables needed for the object. The destructor keyword is dealloc to dispose of the object, making the memory available again. 


[5.4] Using static or shared members (5:22)
-------------------------------------------
Like the interest rate example in the video, give three additional examples of
data that would be the same for all instances of a class.

Examples of static or shared variables are: 
 - When you begin a video game and your new played starts with the same attributes every time. (ex. hit points, gold pieces)
 - When you start to compose a “tweet” on Twitter and the counter begins at 140 characters before typing.
 - When a customer is using a coupon value code for their account (ex. $10 toward any purchase over $50)


Section 6: Inheritance and Composition
======================================
6.1 Identifying inheritance situations (6:49)
---------------------------------------------
Describe in your own words what inheritance is and how it is useful when
constructing classes.

Inheritance is using the Object Oriented concept of a superclass that will have shared attributes that can be used by its subclasses. Also, a subclass can override those attributes inherited from the superclass so that it can be adapted for better usability.


[6.2] Using inheritance (2:43)
------------------------------
Referring to the apps on your phone, come up with three examples where you
believe methods are being inherited from superclasses and called by subclasses.

- In shopping applications, Product would be a superclass and all different types of products (Music, Book, Toy, Electronic) would inherit the generic attribute of Product.
- In the Tumblr application, a generic superclass Post can have different subclasses, namely Text, Photo, Quote, Link, Chat or Video.
- In the Phone application, there are many types of Phone Numbers making it the superclass. Some subclasses are Home, Work, iPhone, Fax and Cell. 
