### Question 3: Implement a Generic Stack Data Structure

**Question:**

Create a generic `Stack` class in TypeScript that supports typical stack operations: `push`, `pop`, `peek`, and `isEmpty`. The stack should be able to store any type of elements.

**Class Specification:**

1. `push(element: T): void` - Adds an element to the top of the stack.
2. `pop(): T | undefined` - Removes and returns the top element from the stack. Returns `undefined` if the stack is empty.
3. `peek(): T | undefined` - Returns the top element without removing it. Returns `undefined` if the stack is empty.
4. `isEmpty(): boolean` - Returns `true` if the stack is empty, otherwise `false`.

Ensure your implementation uses TypeScript generics to handle different types and provide type safety.

**Example Usage:**

```typescript
class Stack<T> {
  // Implement the class here
}

const numberStack = new Stack<number>();
numberStack.push(1);
numberStack.push(2);
console.log(numberStack.pop()); // Output: 2
console.log(numberStack.peek()); // Output: 1
console.log(numberStack.isEmpty()); // Output: false

const stringStack = new Stack<string>();
stringStack.push("a");
stringStack.push("b");
console.log(stringStack.pop()); // Output: "b"
console.log(stringStack.peek()); // Output: "a"
console.log(stringStack.isEmpty()); // Output: false
```

**Constraints:**

- The class should be implemented in TypeScript.
- The stack should support elements of any type.
- The implementation should handle edge cases, such as popping from an empty stack.

---

This question requires a solid understanding of TypeScript generics, data structures, and basic class implementation, making it a suitable task for a technical interview.
