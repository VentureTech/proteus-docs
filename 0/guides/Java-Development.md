---
title: Java Development
---

# Overview
This unit introduces advanced Java features and idioms, Linux basics, and some good software engineering practices.  Use the given references, plus any others you find, to learn about the topics mentioned here.  *Explore the first part of each section fully (up to "Other References"), and peruse the Other References sections as needed.*  There is *much* information available about Java and software engineering; focus especially (but not only) on the information you need to complete the exercises at the end.

# Environment
While you could theoretically develop Java applications on any platform, you will find it helpful to use the same environment as other VentureTech engineers.

We run Linux as a virtual *guest* operating system within another *host* OS, usually Windows.  We use [VMWare] (http://www.vmware.com/) to do this.  Nearly all of your development will be done in the guest Linux OS. 

Set up your virtual development environment using one of our images and instructions.
Once you have opened the image, you may want to do the Unix Primer below, then come back and finish setting up the virtual development environment.
[Virtual Development Machine Setup] (https://docs.google.com/a/vipasolutions.com/document/d/1-Wvp1A9p3qeetbEblxh0DOWgvzkyQ7qLfwhFu25s3Yo/edit?usp=sharing)

Follow this primer and do the tasks in it to learn the basics of working in Linux.
[Unix Primer] (http://cs.iupui.edu/~droberts/n311/resources/unixprimer.htm)
(Note: Linux is Unix-like enough that most Unix information will apply.)

You may use any IDE, but other engineers at VentureTech currently use IntelliJ IDEA, so that will probably be the best option.

## Other References

* [Linux Tutorial] (http://www.tldp.org/LDP/gs/node5.html)
* [Unix for Beginners] (http://www.ee.surrey.ac.uk/Teaching/Unix/)
* [IntelliJ Documentation] (http://www.jetbrains.com/idea/documentation/)

# Java

[Oracle's site] (http://docs.oracle.com/javase/tutorial/index.html) has a wealth of first-party documentation on Java.  
Many of these "trails" cover topics that will not be relevant to Proteus development, like GUIs, Sound, and RMI.  We recommend you focus on the "Trails Covering the Basics" and the trails listed below.

* [Polymorphism] (http://docs.oracle.com/javase/tutorial/java/IandI/index.html)
* [Generics] (http://docs.oracle.com/javase/tutorial/java/generics/)
* [Annotations] (http://docs.oracle.com/javase/tutorial/java/annotations/)
* [Reflection] (http://docs.oracle.com/javase/tutorial/reflect/index.html)

## Other References

If a particular concept is not clear to you as explained in the standard Java tutorials, or you want to explore it from a different angle, try some of these.  You can also just search the web; most of these concepts have been presented a number of times.

* [free-programming-books list] (https://github.com/vhf/free-programming-books/blob/master/free-programming-books.md)
* [IBM DeveloperWorks Library] (http://www.ibm.com/developerworks/java/library/)
* [TutorialsPoint] (http://www.tutorialspoint.com/javaexamples/)
* [Data Structures and Algorithms with Object-Oriented Design Patterns in Java] (http://www.brpreiss.com/books/opus5/html/page9.html)
* [Think Java] (http://greenteapress.com/thinkapjava/html/index.html)
* [Introduction to Programming Using Java, Sixth Edition] (http://math.hws.edu/javanotes/)
* [Learning Java] (http://chimera.labs.oreilly.com/books/1234000001805/index.html)
* [Introduction to Programming in Java] (http://introcs.cs.princeton.edu/java/home/)




---------------------------------
Software Engineering
This topic will require you to think critically about the articles you read.  Writing software always involves judgment calls about the best way to approach a problem.  Often the “best” approach has some disadvantages compared to other approaches, but it is “best” because its advantages match up the best to solve the problem at hand.  Part of good engineering is learning to see, understand, and predict these tradeoffs.  The references provided in this section are about judgment and rules of thumb; not every “rule” will apply 100% of the time.  Still, it is important to learn from other programmers’ experiences as best we can.  For example:

“Beware instanceof operator”
http://javapractices.com/topic/TopicAction.do?Id=31

In this article, the author describes (only) the disadvantages of using instanceof.  But the language designers included instanceof for a reason: there are appropriate uses of it.  A good engineer learns to distinguish necessary and questionable uses of instanceof.  Learn to read critically any article about software engineering or architecture.
Key Topics
API Contracts
Method preconditions, postconditions, and invariants should be clearly documented.  Where appropriate, they should be enforced.  The earlier you discover an error, the easier it will be to debug.
Design by Contract  http://javapractices.com/topic/TopicAction.do?Id=194
Preconditions, Postconditions, and Class Invariants  http://docs.oracle.com/cd/E19683-01/806-7930/assert-13/index.html
Use javadoc liberally http://www.javapractices.com/topic/TopicAction.do?Id=60
How to Design a Good API http://lcsd05.cs.tamu.edu/slides/keynote.pdf 
Exception Handling
Exceptions  http://docs.oracle.com/javase/tutorial/essential/exceptions/
Avoid empty catch blocks  http://javapractices.com/topic/TopicAction.do?Id=16
Pass all pertinent data to exceptions  http://javapractices.com/topic/TopicAction.do?Id=130
Abstraction Tradeoffs
Deciding the proper level of abstraction for a piece of software is difficult.  Which elements should be hard-coded, and which should be parameters?  Too many hard-coded elements leads to inflexible code, while too many parameters leads to convoluted and difficult-to-understand code.  But inflexible code might be acceptable for a one-off (throwaway) piece, while more parameters might be necessary for a reusable API.  Duplicated code is usually bad for maintenance in a reusable library, but it might be more clear than an abstraction in a simple application script.

As you read these articles, notice how there is some tension between “Don’t Repeat Yourself” and “Use Before Reuse”.  
Don’t Repeat Yourself   http://programmer.97things.oreilly.com/wiki/index.php/Don't_Repeat_Yourself
Simplicity before generality, use before reuse http://97things.oreilly.com/wiki/index.php/Simplicity_before_generality,_use_before_reuse

Other References
Again: Beware of one-sided architecture or design articles.  Every “design pattern” has good and poor use cases. Sometimes the increase in complexity when using a pattern outweighs the benefits it would provide.  Read these critically.

Java Practices  http://javapractices.com
This is a useful site, but not every section is relevant.  In particular, you probably want to skip Servlets, JSPs, Swing, and Threads.

Effective Java:  Get a copy of this book from your mentor or manager.

97 Things Every Programmer Should Know
http://programmer.97things.oreilly.com/
http://programmer.97things.oreilly.com/wiki/index.php/Contributions_Appearing_in_the_Book

Martin Fowler on Software Design  http://martinfowler.com/design.html
Like other good software architects, Martin Fowler is skilled in discerning and explaining the costs and benefits of design patterns.

Java Design Patterns  http://www.javaworld.com/columns/jw-java-design-patterns-index.html
Java Design Patterns At a Glance  http://www.javacamp.org/designPattern/
Exercises
The exercises in this section are for command-line, text-based programs (not web applications).

Identify more resources
List 3 links to articles about Java development and software engineering that you found helpful.  Use different articles than the ones in this document.  Summarize each, with pros and cons (elements you liked, did not like, or disagreed with), in a few sentences.


Polymorphism
For this exercise, create a text-only Reverse Polish notation (postfix notation) calculator, similar to:
http://www.meta-calculator.com/learning-lab/reverse-polish-notation-calculator.php  
Additional information in Wikipedia:  http://en.wikipedia.org/wiki/Reverse_Polish_notation

Your calculator will wait for the user to enter a line of text and split it into tokens delimited by whitespace.  Tokens may be floating point numbers or operator strings.  Numbers are pushed onto a Stack<Double>, and operators work on elements at the top of the stack.  When the user enters a blank line, the program terminates.

For example, the user enters:
2 5 + 3 *
And the output is “21” (that is, (2 + 5) * 3).  

Implement these operators:
Binary:  +  -  *  /  
Unary:  sin  cos  tan  sqrt

The key of this exercise is this requirement: Use polymorphism to separate operator implementation from the core program.  Create an interface with a method that takes a Stack<Double> and performs some operation on it.  Then implement the interface once for each operator.  The code that accepts user input should find the correct operator implementation (from some collection of available operations) and delegate to it.  Do not use a giant switch or if-else block. 


Generics
Use type parameters (generics) for this exercise.  The method signatures are the key feature of the exercise.
Write a method last(...) that takes a list of arbitrary objects and returns the last element.  These calls should compile:
String a = last(new ArrayList<String>());
Integer b = last(new ArrayList<Integer>());
Object c = last(new ArrayList<String>());
But not these:
String d = last(new ArrayList<Integer>());
String e = last(new ArrayList<Object>());

Write a method append(...) that takes an object x and a list y, and returns a new list that appends x to the end of y.  These should compile:
append(new String(), new ArrayList<String>());
append(new String(), new ArrayList<Object>());
But not these:
append(Integer.valueOf(0), new ArrayList<String>());
append(new Object(), new ArrayList<String>()); // can’t have objects polluting our List<String>


Add type parameters to the method signatures of “sum” and “appendOne” so that the methods and invocations compile except for the commented calls.  Note that Integer and Double both extend Number.
public static double sum(List list) {  // Add type parameter to List
    double sum = 0;
    for(Number n : list){
        sum += n.doubleValue();
    }
    return sum;
}

public static void appendOne(List list) {  // Add type parameter to List
    list.add(1);
}
    
public static void main(String[] args) {
    sum(new ArrayList<Integer>());
    sum(new ArrayList<Double>());
    //sum(new ArrayList<Object>());  // should fail to compile
    appendOne(new ArrayList<Integer>());
    appendOne(new ArrayList<Object>());
    //appendOne(new ArrayList<Double>()); // should fail to compile
}


Reflection & Annotations
Write a method annotation @Test.  (The Oracle Annotations trail describes how to do this.  For this exercises, you will also need to explore “ Annotations That Apply to Other Annotations” section of the trail.)  Write a method that takes an arbitrary object and finds zero-argument methods on that object with the annotation @Test and executes them.
For an object of the following class, your method should print “foo”.

class MyClass {
     @Test void foo() { System.out.println(“foo”); }
     void bar() { System.out.println(“bar”); }
}


API Contracts
Add Javadoc to your calculator program.
What is wrong with the Javadoc in the following methods?  Rewrite the Javadoc, correcting any errors.

/**
 * Divides two numbers.
 * @param a dividend
 * @param b divisor
 * @return quotient
 */
int divide(int a, int b) 
{
    return a / b;
}


/**
 * Computes the Fibonacci series.  For n >= 2, calls itself twice (on n-1 and n-2).
 * @param n a number
 * @return the nth Fibonnaci number
 */
int fibonacci(int n)
{
    if(n < 0) 
        System.err.println(“Invalid n: “ + n);
    if(n < 2) 
        return n 
    else 
        return fibonacci(n-1) + fibonacci(n-2);    
}

Exception Handling
Add exception handling to your program for the following cases:
User enters a token that is neither a number nor an operator
An operation fails due to invalid arguments
What is wrong with the code in the following methods?  Assume the Javadoc is correct.  Rewrite the code to match the Javadoc and correct any problems.


/**
 * Reads a file into a buffer.
 * @param file the file
 * @param buf character array that must be large enough to hold the file contents
 */ 
void read(File file, char[] buf) 
{
    try
    {
        FileReader input = new FileReader(file);
        input.read(buf);
    }
    catch(Exception ex)
    {
    }
}


// Note especially the stated precondition.
/**
 * Converts a String to an int and adds one.  Assumes the argument is parseable.
 * @param s a String that must be parseable as an int
 * @return (the int value of s) plus one
 */
int getValueAndIncrement(String s)
{
    try
    {
        return Integer.valueOf(s) + 1;
    }
    catch(NumberFormatException ex)
    {
        _logger.info(“Error parsing number: “ + s);
        return -1;
    }
} 


Abstraction Tradeoffs

This exercise requires you to think about the approach to a problem without writing any code.

Suppose you recently did some work for a client that involved reading CSV files and processing them, outputting the rows in a certain order. For this project, you wrote all the code yourself. A new project also requires you to read CSV files and process them, outputting the rows in a certain order, but the ordering is different and the set of columns is different.  The file format for the new project is different also; some of the data are escaped.  The new project is small and needs to be done as quickly as possible.

a.  How would you implement this second project, assuming time is short and you don't know whether or not you'll be asked to do similar future projects?  Would you use a particular design pattern, reuse code, or write code from scratch?  Describe your approach in a few sentences.
b.  What if you have a little more time, and you know you'll need to process more files in the future the same way, but with different columns and different specification for how to order the output?  Would your approach be the same, or how would it be different?
