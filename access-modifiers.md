# Access Modifiers in TypeScript OOP:

## Introduction:

I use access modifiers in OOP or classes to control where a property will be shown, accessed, and updated, and where it will not. I use access modifiers to control these properties from other classes or outside code. In TypeScript, classes have strict rules, so I use `public`, `private`, `protected`, and `readonly` modifiers to control the behavior based on my requirements.

## How Access Modifiers Work:

1. `public`: The `public` modifier is used to access the property from everywhere, such as inside the class, in a child class, or from outside the class.
2. `private`: The `private` modifier only allows access inside the exact class where it is defined. It cannot be accessed from a child class or outside.
3. `protected`: The `protected` modifier works and allows access or modification only inside its own class and its child classes (subclasses).
4. `readonly`: I use `readonly` to only read the property. Once the value is set in the constructor, it cannot be modified or updated later.

```ts
class Student {
  public name: string;
  private password: string;
  protected department: string;
  readonly id: number;

  constructor(name: string, password: string, department: string, id: number) {
    this.name = name;
    this.password = password;
    this.department = department;
    this.id = id;
  }
}
```

## Conclusion:

These access modifiers help me protect my code. For example, if a bank account class has sensitive data like balance or password, I use these class modifiers for safety. Each modifier has its own ability and restrictions to keep our OOP code secure.