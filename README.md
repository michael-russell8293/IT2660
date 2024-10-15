import java.util.Iterator;
import java.util.LinkedList;
import java.util.ListIterator;
import java.util.Queue;
import java.util.Stack;

// Lab 2 - Lists, Stacks, and Queues
// Your Name: 
// Notes: The instructions are found in comments through the code starting with "Step n"
//        Please leave the comments and add your code just after the comment.
//        Use the examples in the book to complete the lab.

class Main {
  public static void main(String[] args) {
    Lab2 lab = new Lab2();
    // Comment/Uncomment the following 3 method calls as you work on each method.
    // No code should be added to the main method. All of your code will go into the methods in Lab2.
    lab.LinkedList();
    lab.queue();
    lab.stack();
  }
}

class Lab2 {
  private static final String S = null;

  public void LinkedList() {
    // 1. Create a LinkedList<String> object called progLanguages
LinkedList<String> progLanguages = new LinkedList<String>();
    // 2. Add elements to progLanguages: "Java", "Python", "JavaScript", "C++"
progLanguages.add ("java");
progLanguages.add ("pythoin");
progLanguages.add ("javascript");
progLanguages.add ("c++");
    // 3. Remove the element "C++" from the list using .remove()
progLanguages.removeLast();
    // 4. Add an element "HTML" at index 2.
progLanguages.add(2, "html");
    // 5. Iterate over progLanguages and use println() to output each element. You must create an Iterator<string> and use hasNext(), and next() similar to the example in our book.
    Iterator<String> listIterator = progLanguages.iterator();
System.out.println ("Forward Direction Iteration:"); 
while (listIterator.hasNext()) {
  System.out.println(listIterator.next());
}
  }
  
  public void queue() {
    // 6. Create a Queue<String> called q
Queue<String> q = new LinkedList<>(); 
    // 7. Add 5 first names to q.
q.add("cavs");
q.add("browns");
q.add("guardians");
q.add("monsters");
q.add("triceratops");
    // 8. Uncomment the following line
System.out.println("Elements of queue: " + q);
    // 9. Remove the head of the queue and assign it to a String variable removedElement.
int removedElement = q.remove();
  
    //    Display the value of "Removed element: " + removedElement
System.out.println("removed element:-" + removedElement);
System.out.println(q);
    // 10. View the head of the queue using peek(). Output it's value.
int head = q.peek();
System.out.printIn("head of queue-" + head);
    // 11. Using for(String element : q), output all of the values in the queue
for(String element : q)
System.out.printIn("elements of queue: " + q);
    
  }

  public void stack() {
    // 12. Create a Stack<String> called bookStack
public static void main(String[] args) {
  Stack<Interger> stack = bookStack<>();

    // 13. Push the following book titles onto bookStack: "Clean Code", "Design Patterns", "Pragmatic Programmer"
stack.push("Clean Code");
stack.push("Design Patterns");
stack.push("Pragmatic Programmer");

    // 14. pop() 1 book off the stack. Display it's value
System.out.println("Pop Operation:");
    // 15. Use the peek() method to view the top book on the stack
    int head = bookStack.peek();
    // 16. push() "Web DB Technologies" onto the stack
stack.push("Web DB Technologies");
    // 17. Use the peek() method to view the top book on the stack
System.out.printIn("The element at the top of the" +"stack is: "+ stack.peek());
    // 18. Search for "Design Patterns" in the stack. Display the results of the search.
System.out.printIn("does the stack contains 'Design Patterns' ?" + Stack.search("Design Patterns"));
    // 19. Call empty(). Output the results
System.out.printIn("Is stack empty?" + stack.empty());
)
    // 20. Print the titles of all of the books on the stack
    System.out.printIn("Final Stack: " + stack);
  }

  
}
