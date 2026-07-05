# Singly Linked List

class Node:
    def __init__(self, data):
        self.data = data
        self.next = None


class SLL:
    def __init__(self):
        self.head = None

    def insertNode(self, data):
        node = Node(data)

        if self.head is None:
            self.head = node
        else:
            temp = self.head
            while temp.next:
                temp = temp.next
            temp.next = node

    def display(self):
        temp = self.head
        while temp:
            print(temp.data, end="->")
            temp = temp.next


ob = SLL()

ob.insertNode(10)
ob.insertNode(20)
ob.insertNode(30)
ob.insertNode(40)
ob.insertNode(50)

print("""
1. INSERTION AT BEGINNING
2. INSERTION AT END
3. INSERTION AT ANY POSITION
4. DELETION AT BEGINNING
5. DELETION AT END
6. DELETION AT ANY POSITION
""")

choice = int(input("Enter Your Choice: "))

match choice:

    case 1:
        newnode = Node(5)

        if ob.head is None:
            ob.head = newnode
        else:
            newnode.next = ob.head
            ob.head = newnode

        ob.display()

    case 2:
        newnode = Node(55)

        if ob.head is None:
            ob.head = newnode
        else:
            temp = ob.head
            while temp.next is not None:
                temp = temp.next
            temp.next = newnode

        ob.display()

    case 3:
        newnode = Node(25)
        pos = int(input("Enter your position you want to insert: "))

        if ob.head is None:
            ob.head = newnode

        elif pos == 1:
            newnode.next = ob.head
            ob.head = newnode

        else:
            temp = ob.head
            for i in range(1, pos - 1):
                temp = temp.next

            newnode.next = temp.next
            temp.next = newnode

        ob.display()

    case 4:
        if ob.head is None:
            print("No element to delete")
        else:
            ob.head = ob.head.next

        ob.display()

    case 5:
        if ob.head is None:
            print("No element to delete")
        else:
            temp = ob.head
            while temp.next.next is not None:
                temp = temp.next

            temp.next = None

        ob.display()

    case 6:
        if ob.head is None:
            print("No element to delete")
        else:
            ob.display()

            key = int(input("\nEnter Key You Want Delete: "))

            if key == 10:
                ob.head = ob.head.next
            else:
                temp = ob.head
                prev = None

                while temp.data != key:
                    prev = temp
                    temp = temp.next

                prev.next = temp.next

            ob.display()

    case _:
        print("Invalid Choice")
