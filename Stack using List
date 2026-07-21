class StackDS:
    def __init__(self):
        self.stack = []

    def is_empty(self):
        if len(self.stack) == 0:
            print("Stack is Empty")
        else:
            print("Stack is Not Empty")

    def push(self, data):
        self.stack.append(data)

    def pop(self):
        if len(self.stack) == 0:
            print("No Element to delete")
        else:
            print("Deleted:", self.stack.pop())

    def peek(self):
        if len(self.stack) == 0:
            print("Stack is Underflow")
        else:
            print("Top Element:", self.stack[-1])

    def display(self):
        print("Stack:", self.stack)


obj = StackDS()

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

    ch = input("\nEnter 'exit' to stop or 'continue' to proceed: ").lower()

    if ch == "exit":
        print("Program Ended")
        break



        
