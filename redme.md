TypeScript Problem Solving Assignment 1

This repository contains solutions to 8 TypeScript coding problems covering core concepts including type narrowing, generic functions, interface design, OOP with access modifiers, tuple handling, array manipulations, and asynchronous promises.

Summary of Problems & Solutions

1. multiplyValue (Optional & Default Parameters)

Goal: Multiply a number by a given multiplier, defaulting to 2 if omitted, while correctly handling 0.

Key Concept: Used TypeScript default parameters (b: number = 2) to safely handle undefined without falsely treating 0 as falsy.

2. processInput (Union Types & Type Narrowing)

Goal: Process a input of type string | number | boolean and return formatted output depending on its type.

Key Concept: Leveraged typeof type narrowing to handle strings (.trim().toLowerCase()), numbers (* 10), and booleans ("Active" / "Inactive").

3. formatCoordinate (Readonly Tuples)

Goal: Format a 3-element coordinate tuple [latitude, longitude, locationName] into a descriptive string.

Key Concept: Applied readonly [number, number, string] parameter modifier to ensure tuple immutability and used array destructuring.

4. concatenateArrays (Generics & Rest Parameters)

Goal: Combine an arbitrary number of arrays of the same type T into a single flattened array.

Key Concept: Used generic type parameter <T> combined with rest parameters (...arrays: T[][]) and .flat() without resorting to any.

5. getPopularCourses (Interfaces & Array Filtering)

Goal: Define a Course interface and return published courses matching a minimum student threshold.

Key Concept: Utilized custom interface typing and the non-mutating .filter() method to keep data immutable.

6. pluckValues (Generic Constraints & keyof)

Goal: Extract values of a specified property key from an array of objects.

Key Concept: Employed <T, K extends keyof T> constraints and indexed access return type T[K][] for end-to-end type safety.

7. Employee & Manager Classes (OOP & Access Modifiers)

Goal: Build an Employee base class and a Manager subclass demonstrating inheritance.

Key Concept: Applied protected and private access modifiers alongside super() constructor calls.

8. validateAgeAsync (Promises & Async Handling)

Goal: Return a Promise<string> that resolves after 1 second if age >= 18 or rejects immediately with an Error if underage.

Key Concept: Explicitly typed Promise<string>, using setTimeout for delayed resolution and new Error() for immediate rejection.

Tech Stack & Features

Language: TypeScript

Concepts: Strict Type Safety, Generics, OOP Inheritance, Immutability, Type Narrowing, Async Promises.

Opinon: I try my to best within short time and learned many things during I solved the problem.