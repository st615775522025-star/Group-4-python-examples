# Group-4-python-examples
#2. STACK (LIFO)
class Stack:
    def __init__(self):
        self.stack = []

    def push(self, x):
        self.stack.append(x)

    def pop(self):
        if not self.is_empty():
            return self.stack.pop()
        return "Stack is empty"

    def peek(self):
        return self.stack[-1] if not self.is_empty() else None

    def is_empty(self):
        return len(self.stack) == 0


# Example
s = Stack()
s.push(5)
s.push(10)
print(s.pop())   # 10
print(s.peek())  # 5
