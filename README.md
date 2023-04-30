Download Link: https://assignmentchef.com/product/solved-homework-12-complex-guis
<br>
<strong>Goals:</strong>

<ul>

 <li>Learn how to apply the MVC paradigm</li>

 <li>Learn how to handle events</li>

 <li>Learn how to add functionality to Swing components</li>

</ul>




<strong>Introduction: </strong>

While working in the terminal for an eternity may be appealing to some, most users would like to interact with a graphical user interface, or GUI. GUIs, nowadays, can be found anywhere and everywhere — on our laptops, on our phones, at fast food locations, et cetera. They have made, and continue to make, computers easier to use for everyone.

The Java Programming Language offers built-in libraries to create graphical user interfaces, in the form of AWT and Swing, with Swing being the newer of the two. One of the nice things about these libraries is that they are cross-platform. If you create an application on your Mac, the same application can run seamlessly on your friend’s Windows machine. <strong> </strong>

<strong>Description </strong>

An IntelliJ project has been provided for you as skeleton code and is accessible from the course webpage. This project contains classes and methods that have already been declared for you. All you need to do is add implementations where you find TODO comments in <strong>AddController</strong>​, ​<strong>EditController</strong>​, ​<strong>DeleteController</strong>​, and ​<strong>SearchController</strong>​. When you would like to run the application, you may do so by clicking the green arrow in the MessageBoardRunner class — this is where main() is declared. If you have any issues with setting this up in IntelliJ, please post on Campuswire.

This application is similar to a Twitter feed or message board. Rather than have a user go through a terminal and manually organize a list of text files or messages, we are designing a GUI to allow a user to easily add, delete, edit, and search for tweets. Each tweet will have a unique numeric ID (1, 2, … 17). Our GUI will include four tabs corresponding to the classes in bold above. Your task is to implement each of the methods described below. Starter code is available on Blackboard, and you should not begin working until you have downloaded and read through it.

For a better understanding of the Model View Controller (MVC) paradigm, you can read about it ​<u><a href="https://medium.freecodecamp.org/model-view-controller-mvc-explained-through-ordering-drinks-at-the-bar-efcba6255053">here</a>​</u><a href="https://medium.freecodecamp.org/model-view-controller-mvc-explained-through-ordering-drinks-at-the-bar-efcba6255053">.</a> Note that the CS180 team does not condone underage drinking ;).







<h1>AddController.java</h1>

<ol>

 <li><strong>public AddController(): </strong>Implement the constructor method for this class. This should​ throw an IllegalArgumentException if either argument is null. This is where you will add the functionality of the buttons. If you get stuck, try doing some googling for how Swing components use “ActionListeners”.</li>

</ol>




<ol start="2">

 <li><strong>private void getAddButtonSemantics(): </strong>This method gets called when the user​ presses ‘Add Tweet’ button, it checks the tweet ID, and if it is not numeric or negative, it displays an error message (The specified ID is not a valid number!), and moves the cursor to this text field in the form. If the ID is valid, it proceeds to adding this tweet to the tweetList, and then displays either a successful message if successfully posted, or an error message otherwise. Reminder that Tweet ID’s must also be unique.</li>

</ol>




<ol start="3">

 <li><strong>public void getClearButtonSemantics(): </strong>This method is called to clear the fields in a​ panel of all text and put the cursor back on the ID field.</li>

</ol>

<h1>EditController.java</h1>

<ol>

 <li><strong>public EditController(): </strong>Follow the same instructions for the AddController instructor,​ but instead of adding a tweet to our tweetList, we will edit the contents of an existing tweet.</li>

</ol>




<ol start="2">

 <li><strong>private void getEditButtonSemantics(): </strong>This method gets called when the user​ presses ‘Edit Tweet’ button, it checks the tweet ID, and if it is does not exist, it displays an error message (A message with the given ID does not exist!). If the ID exists, it proceeds to editing this tweet, reading the new body entered by the user, updating it and then displays a successful message for the user. If the edited text is left empty, show a message that suggests the user delete the Tweet instead. If the Tweet is successfully edited, display a message dialog accordingly.</li>

</ol>




<ol start="3">

 <li><strong>private void getClearButtonSemantics():</strong> Clear the fields in the panel and reset the​ cursor to the body text field.</li>

</ol>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong>             </strong>

<h1>DeleteController.java</h1>

<ol>

 <li><strong>public DeleteController():</strong>​ Follow the same instructions per the two previous constructor methods. Rather than adding or editing a tweet to our tweetList, we will be removing a tweet based on the ID input.</li>

</ol>




<ol start="2">

 <li><strong>private void getDeleteButtonSemantics(): </strong>​This method gets called when the user presses ‘Delete Tweet’ button, it checks the tweet ID, and if it is does not exist, it displays an error message (A message with the given ID does not exist!). If the ID exists, it proceeds to deleting this tweet, and then displays a success message for the user. It also clears all fields in this form. You can assume there will be no null input.</li>

</ol>




<ol start="3">

 <li><strong>public void getClearButtonSemantics(): </strong>​This method is called to clear the fields in a panel of all text and put the cursor back on the ID field.</li>

</ol>

<h1>SearchController.java</h1>

<strong>*</strong>​You may create additional methods within SearchController in order to complete this task

<ol>

 <li><strong>public SearchController(): </strong>​Follow the same instructions per the other constructors.</li>

</ol>




<ol start="2">

 <li><strong>private void getSearchButtonSemantics():</strong>​ Similar to the other semantic methods, write this method in order to search for a given tweet by using a search phrase. You can assume the phrase used to search will always be a valid String and will not be null. By pressing the ‘Search’ button, a list should show up in the ​<strong>IDTextArea</strong>​, separating each Tweet ID that contained the search phrase to a new line. You should check to see if the search phrase is empty and display an error message accordingly.</li>

</ol>

<strong>Submission </strong>

Items required for Submission via Blackboard:

<ul>

 <li><strong>Resubmit all files provided in the skeleton code. </strong></li>

 <li><strong>GRADING IS MANUAL FOR THIS ASSIGNMENT! </strong></li>

</ul>