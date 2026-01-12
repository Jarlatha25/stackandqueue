# stackandqueue

class Stack:
    def __init__(self):
        self.items = []

    def push(self, item):
        self.items.append(item)

    def pop(self):
        return self.items.pop() if self.items else None

    def peek(self):
        return self.items[-1] if self.items else None

    def display(self):
        print("Stack:", self.items)
print("--- Stack ---")
stack = Stack()
stack.push(10)
stack.push(20)
stack.push(30)
stack.display()
print("Pop:", stack.pop())
stack.display()
print("Peek:", stack.peek())

class Queue:
    def __init__(self):
        self.items = []

    def enqueue(self, item):
        self.items.append(item)

    def dequeue(self):
        return self.items.pop(0) if self.items else None

    def display(self):
        print("Queue:", self.items)

print("\n--- Queue ---")
queue = Queue()
queue.enqueue(10)
queue.enqueue(20)
queue.enqueue(30)
queue.display()
print("Dequeue:", queue.dequeue())
queue.display()
 

OUTPUT:
--- Stack ---
Stack: [10, 20, 30]
Pop: 30
Stack: [10, 20]
Peek: 20

--- Queue ---
Queue: [10, 20, 30]
Dequeue: 10
Queue: [20, 30]

