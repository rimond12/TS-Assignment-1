# Type Alias vs Interface in TypeScript:

## Introduction:

In TypeScript, I use `type` to keep the types safe for variables, function parameters, return values, arrays, and objects. On the other hand, I also use `interface` for type safety in my code. At first look `type` and `interface` look almost the same, but they have some important differences between in syntax and features.

## Main Differences:

1. Object vs Other Types: I mainly use `interface` to define the shape of an object. However, `type` can also be used for objects, primitive types, union types (`|`), and tuples.
2. Extending: An `interface` uses the `extends` keyword to inherit properties, while a `type` uses the intersection symbol (`&`).
3. Declaration Merging: If I write two interfaces with the same name, TypeScript automatically merges them together. A `type` alias cannot be declared twice with the same name.

```ts
// Interface example
interface Student {
  name: string;
}
interface Student { // It will be merged automatically
  roll: number; 
}

// Type alias example
type ResultStatus = "passed" | "failed";
```

## Conclusion

I use `interface` specifically for objects and `type` for the other things like when I have to define a type for variables, return values, and also for arrays. And also I use `interface` when I am working with OOP in TypeScript.