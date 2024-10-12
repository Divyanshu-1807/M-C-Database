## Type Utilities

JavaScript is a dynamically typed language, meaning the types of variables can change during runtime. Many interview questions involve recursion of values that contain different types, and handling each value type varies depending on its type (e.g., different code is needed to iterate over an array vs. an object). Knowledge of handling JavaScript types is crucial for solving questions like **Deep Clone** and **Deep Equal**.

In this section, we will implement the following utility functions to determine the types of primitive values:

- **isBoolean(value)**: Returns `true` if the value is a boolean, `false` otherwise.
- **isNumber(value)**: Returns `true` if the value is a number, `false` otherwise. Note that `NaN` is considered a number.
- **isNull(value)**: Returns `true` if the value is null, `false` otherwise.
- **isString(value)**: Returns `true` if the value is a string, `false` otherwise.
- **isSymbol(value)**: Returns `true` if the value is a Symbol primitive, `false` otherwise.
- **isUndefined(value)**: Returns `true` if the value is undefined, `false` otherwise.
