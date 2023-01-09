# Students-Report-Management-System
A student record management software is a tool
that tracks and records regular activities of the
students in institutes including attendance,
exam performance, and their behavior. The
software can be accessed by students, teachers,
admin and parents with a role-based login. It
collects all the student data along with their
personal information which can be easily
searched and retrieved later on. The software
stores years of data online on a cloud platform.

OBJECTIVE
A student report management system
helps you keep and maintain multiple
records effortlessly. The tool automates
data tracking and record-keeping related
to various academic aspects such as
performance, attendance, documents,
admission, fees, and disciplinary
records.The purpose of the project is to
build an application program to reduce
the manual work for managing the
Profiles, Courses, Student, Logins etc.
We can say that projects like these have
digitalized record keeping and made it
easier and convenient.

PROJECT WORK
Over the recent years, the performance and
efficiency of the education industry have been
enhanced by using the Student Management
System. This tool has productively taken over
the workload of the admin department with its
well-organized, easy, and reliable online
school management software. The project
works by taking details of different students
and storing it which can be accessed ,
viewed ,edited and deleted later on. We can
also search records of any particular student.
It saves the hassle of keeping records of
students on paper , hence saves a lot of
paperwork.

Basic Fundamentals with Code Explanation
Linked List :-
Linked List can be defined as the collection of nodes that are
randomly stored in memory.

There are four types of linked list :-
1) Singly Linked List
2) Doubly Linked List
3) Circular Linked List
4) Circular Doubly Linked Lists


Singly Linked List :-
It is the most common type of linked list among all. Here,
each node has a data and a pointer to the next node.Node in
Singly Linked List is represented as :-
struct Node {
int data;
struct Node *next;

Circular Linked List:-
A circular linked list is a variation of a linked list
in which the last element is linked back to the first
element. This forms a circular loop.
A circular linked list can be either singly linked or
doubly linked. In singly linked list, next pointer of
the last item points to the first item. In the doubly
linked list, prev pointer of the first item points to
the last item as well.

Doubly Circular Linked Lists:-
A doubly circular linked list is a mixture of a
doubly linked list and a circular linked list. Like
the doubly linked list, it has an extra pointer
called the previous pointer, and similar to the
circular linked list, its last node points at the head
node. This type of linked list is the bidirectional
list. So, you can traverse it in both directions.




Here, in our project we are mostly working with singly
linked lists.
So, let‘s take a look at the basic operations that we
have performed on singly linked list in our project.
Basic Operations on Singly Linked Lists :-
1) Insertion
2) Deletion
3) Searching
Insertion :-
Linked List gives us this freedom to insert a record
anywhere without
much modification. Here we can add a record at the
beginning, at the
end and also after a current record.
1. Insert at the beginning :-
Insertion at the beginning requires four steps to do:-
Allocate memory for a new node.
Take the data from the user and store it.
Point next pointer of newly created node to head node.
Change head to point to recently created node.
Program :-
struct node* newNode;
newNode = malloc(sizeof(struct node));
newNode->data = 1;
newNode->next = head;
head = newNode;
2. Insert at the End :-
Insertion at the end requires four steps to do:-
Allocate memory for new node.
Take the data from the user and store it.
Traverse to last node.
Change next of last node to recently created node.
Program:-
struct node *newNode;
newNode = malloc(sizeof(struct node));
newNode->data = 1;
newNode->next = NULL;
struct node *temp = head;
while(temp->next != NULL){
temp = temp->next;
}
temp->next = newNode;
3. Insert at the Middle
}}
Allocate memory for new node
Take the data from the user and store it. Traverse to node
just before the required position of new node.
Change next pointers to include new node in between.
Program :-
struct node *newNode;
newNode = malloc(sizeof(struct node)); newNode->data
= 4;
struct node *temp = head;
for(int i=2; i < position; i++) {
if(temp->next != NULL) {
temp = temp->next;
newNode->next = temp->next;
temp->next = newNode;
Deletion:-
Just like insertion, we can also delete a record from
beginning, end and any other location without much
modification.
1. Deletion at beginning :-
To delete a node at the beginning:-
1) Make a temporary pointer and point it to the head of the
linked list.
2) Change the head pointer to point to the next node of the
linked list.
3) Free the first node with the help of temporary pointer.
Program:-
struct node* temp = head;
head = head->next;
delete temp;
2.To delete a node at the end:-
1) Traverse to the second last element of the linked list.
2) Make a temporary pointer and point it to the next node of the
linked list.
3) Change the next pointer of the second last node to NULL.
4) Delete the last node, with the help of temporary pointer.
Program:-
struct node* temp = head;
while(temp->next->next !=NULL){
temp = temp->next;
}
struct node *nextNode = temp->next;
temp->next = NULL;
delete nextNode;
Delete at any Position:-
}}
Traverse to node before the node to be deleted.
Make a temporary pointer and point it to the next node
of the
linked list.
Change next pointers to exclude the node from the
chain.
Delete the node with the help of temporary pointer.
Program :-
for(int i=2; i< position; i++) {
if(temp->next!=NULL) {
temp = temp->next;
struct node *nextNode = temp->next;
temp->next = temp->next->next;
delete nextNode;
Searching :-
We can search for a particular record inside a linked
list using a
loop :-
Make head as the current node.
Run a loop until the current node is NULL.
In each iteration, check if the key of the node is
equal to the
record you are looking for. If it the key matches the
record,
return true otherwise return false.
Program :-
struct node *current = head;
while (current != NULL) {
if (current->data == key)
return true;
current = current->next;
}
return false;


FUTURE SCOPE
The project has a very vast scope in future. The
Project can be updated in near future as and when
requirement for the same arises, as it is very
flexible in terms of expansion. With the proposed
software of Student Report System ready and fully
functional the user is now able to manage and
hence run the entire work in a much better,
accurate and error free manner.In the future the
students can also be able to upload or download
notes.
A few more minor tweaks here an there for making
the application more visually appealing and will
have statistics, tracking and analytics.The whole
project can be made available as an android app
for far more ease of use and mobility.

Screenshots:-
Below are the screenshots of the output of the
various functions provided by the student record
management system:


                                Create Record:
![image](https://user-images.githubusercontent.com/77992826/211372939-3775ac3f-e4aa-4bde-9542-067ab4328d40.png)


Show Record:
![image](https://user-images.githubusercontent.com/77992826/211373243-d2ae383f-bb9e-490b-b51d-3409169f460f.png)


Search Record:
![image](https://user-images.githubusercontent.com/77992826/211373275-0f9bf6bb-675d-4284-9703-fa9ab7d5ff32.png)



Delete Record:
![image](https://user-images.githubusercontent.com/77992826/211373338-742b378a-4e31-43f0-bdf3-a27ead8a55dd.png)


Exit From Program:
![image](https://user-images.githubusercontent.com/77992826/211373445-beb66fa4-12a1-44ad-900e-3e22df2ca75c.png)


FUTURE SCOPE
The project has a very vast scope in future. The
Project can be updated in near future as and when
requirement for the same arises, as it is very
flexible in terms of expansion. With the proposed
software of Student Report System ready and fully
functional the user is now able to manage and
hence run the entire work in a much better,
accurate and error free manner.In the future the
students can also be able to upload or download
notes.
A few more minor tweaks here an there for making
the application more visually appealing and will
have statistics, tracking and analytics.The whole
project can be made available as an android app
for far more ease of use and mobility.



CONCLUSION:-
It was a wonderful and learning experience for us while
working on this project. Student report management
system make faculty jobs more accessible by giving
them easy place to find and sort information. This
system allows teachers and students engagement.
So, we can hope that this will create a scenario that
makes the lives of administration and teacher easier.
