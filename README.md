# Stack implementation using list

stack = []

# Push operation
def push():
    element = int(input("Enter element to push: "))
    stack.append(element)
    print("Stack:", stack)

# Pop operation
def pop():
    if len(stack) == 0:
        print("Stack is empty")
    else:
        removed = stack.pop()
        print("Removed element:", removed)
        print("Stack:", stack)

# Display stack
def display():
    print("Stack elements:", stack)


while True:
    print("\n1.Push  2.Pop  3.Display  4.Exit")
    choice = int(input("Enter choice: "))

    if choice == 1:
        push()
    elif choice == 2:
        pop()
    elif choice == 3:
        display()
    elif choice == 4:
        break
    else:
        print("Invalid choice")# Data-structure-practical-program34
