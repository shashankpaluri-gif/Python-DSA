class Node:
    def __init__(self,data):
        self.data=data
        self.next=None
        
class Stack:
    def __init__(self):
        self.top=None
    def is_empty(self):
        if self.top is None:
            print("Stack is Empty")
        else:
            print("Stack is Not Empty")
    def push(self,data):
        new=Node(data)
        new.next=self.top
        self.top=new
        
    def pop(self):
        if self.top is None:
            print("Stack is underflow ")
        else:
            temp=self.top
            self.top=self.top.next
            return temp.data
    def peek(self):
        if self.top is None:
            print("Stack is underflow")
        else:
            return self.top.data
    def display(self):
        if self.top is None:
            print("stack is underflow")
        else:
            temp=self.top
            while temp:
                print(temp.data,end="->")
                temp=temp.next
obj = Stack()

while True:
    print("\n------ STACK MENU ------")
    print("1.Is_Empty\n2.Push\n3.Pop\n4.Peek\n5.Display")
    
    choice = int(input("Enter your choice: "))

    match choice:
        case 1:
            obj.is_empty()

        case 2:
            data = int(input("Enter element: "))
            obj.push(data)

        case 3:
            obj.pop()

        case 4:
            obj.peek()

        case 5:
            obj.display()

        case _:
            print("Invalid Choice")

    ch = input("\nEnter 'yes' to stop or 'No' to proceed: ").lower()

    if ch == "No":
        print("Program Ended")
        break
