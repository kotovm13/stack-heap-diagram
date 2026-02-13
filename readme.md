Self-evaluation
For this task, I created a Stack–Heap diagram that represents the execution of the given Java program at the deepest point of the call stack (inside the shrink() method). I chose this moment because it shows all active stack frames at once, which makes it easier to demonstrate method call order and all local variables.
Depiction of local variables and local references
All primitive local variables and local references are shown in the stack memory segment.
In main():
args
name
list
times
In fill():
collection
str
times
shrunk
i
In shrink():
str
newLength
chars
i
Primitive variables such as times, newLength, and i are represented as values. Reference variables correctly point to objects in the heap. Therefore, all required local variables are depicted.
Score: 4 / 4
Depiction of method calls and stack order
The diagram clearly shows the correct order of method calls in the stack. The stack is represented from top to bottom as:
shrink()
fill()
main()
This reflects the actual execution flow of the program, where main() calls fill(), and fill() calls shrink(). The stack frame order is correct and demonstrates proper understanding of how the JVM manages method calls.
Score: 3 / 3
Depiction of heap objects and links
All relevant objects are shown in the heap memory segment. These include:
String objects ("Kevin", "KevinKevin")
char[] created in shrink()
ArrayList object
Internal Object[] of the ArrayList
String[] args
All stack references correctly point to their corresponding heap objects. The internal relationship between ArrayList and its internal Object[] is also shown. This demonstrates correct understanding of object allocation and reference linking in JVM memory.
Score: 4 / 4
Final score
Local variables and references: 4
Method call order: 3
Heap objects and linking: 4
Total: 10 / 10
