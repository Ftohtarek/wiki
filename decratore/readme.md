# Decorators

## Aim
Cross-cutting concerns that are not easily solved with inheritance.

## Definition
Provide a way to add both annotations and meta-programming syntax for class declarations and members, carrying metadata and function changes. This leads to the paradigm of using decorators.

### Concept of Aspect-Oriented Programming (AOP)
AOP is a programming paradigm that aims to increase modularity by allowing the separation of cross-cutting concerns.

## Types of Decorators

### Class
Applied to class constructors for observing, modifying, or replacing class definitions.

**Implementation:**

```typescript
function log(constructor: Function) {
    console.log(`${constructor} Decorator Invoked`);
}
```
- ### method:
    applied to method property for observing, modifying, or replacing method defination
- ### property:
    can be only leverage to observe that property has been declared for a class
- ### parameter:
    applied to method declaration for observing that parameters had been defined on a method.


