### Question 4: Implement a Generic Binary Search Tree (BST)

**Question:**

Create a generic Binary Search Tree (BST) in TypeScript that supports insertion, search, and in-order traversal. The BST should be able to store any type that can be compared using a comparison function provided at tree creation. Implement the following methods:

1. `insert(value: T): void` - Inserts a value into the BST.
2. `search(value: T): boolean` - Searches for a value in the BST and returns `true` if found, otherwise `false`.
3. `inOrderTraversal(callback: (value: T) => void): void` - Performs an in-order traversal of the BST and calls the provided callback function with each value.

Ensure your implementation uses TypeScript generics to handle different types and provide type safety.

**Example Usage:**

```typescript
class BinarySearchTree<T> {
  // Implement the class here
}

const compareNumbers = (a: number, b: number) => a - b;
const bst = new BinarySearchTree<number>(compareNumbers);

bst.insert(5);
bst.insert(3);
bst.insert(8);
bst.insert(4);

console.log(bst.search(3)); // Output: true
console.log(bst.search(7)); // Output: false

bst.inOrderTraversal(value => console.log(value)); // Output: 3, 4, 5, 8
```

**Constraints:**

- The BST should be implemented as a class.
- You must use TypeScript generics to handle different data types.
- The comparison function should be provided when creating the BST instance to allow for custom comparison logic.
- The tree nodes should be implemented as an internal class or type within the BST class.
