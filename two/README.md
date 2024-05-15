### Question 2: Write a TypeScript Utility Type

**Question:**

Create a TypeScript utility type `MyPartial<T>` that makes all properties of a given type `T` optional. This custom utility type should mimic the built-in `Partial<T>` utility type provided by TypeScript.

**Type Specification:**

1. `MyPartial<T>` - Takes a type `T` and returns a new type with all properties of `T` set to optional.

Ensure your implementation is type-safe and correctly handles various types, including nested objects.

**Example Usage:**

```typescript
type MyPartial<T> = {
  // Implement the type here
}

interface User {
  id: number;
  name: string;
  email: string;
}

type PartialUser = MyPartial<User>;

const user1: PartialUser = {};
const user2: PartialUser = { id: 1 };
const user3: PartialUser = { id: 1, name: "Alice" };
```

**Constraints:**

- The utility type should be implemented using TypeScript.
- The type should handle any given type `T`, including those with nested properties.
- The implementation should ensure type safety.

---

This question requires a solid understanding of TypeScript's type system and the ability to create advanced utility types, making it a suitable task for a technical interview.

---
