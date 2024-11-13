# linkedlist 
This repository contains a Python implementation of a singly linked list with basic operations such as inserting a node at the end and printing the list.
program to insert a node at the end of a linked list

class Node:
    def __init__(self,data):
        self.data = data
        self.next = None
class linkedlist:
    def __init__(self):
        self.head=None
        
    def insert_at_end(self,data):
        newnode=Node(data)
        if not self.head:
            self.head=newnode
            return
        current=self.head
        while current.next:
            current=current.next
        current.next=newnode
    def printlist(self):
        current=self.head
        while current:
            print(current.data,end= "->")
            current=current.next
        print(None)

ll = linkedlist()  
ll.insert_at_end(5)  
ll.insert_at_end(10)  
ll.insert_at_end(15)  
ll.printlist()  

 This will insert the values `5`, `10`, and `15` into the linked list and print the list.

Example Output

5 -> 10 -> 15 -> None

        
