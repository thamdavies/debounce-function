# Debounce Function
This package provides a `debounce` function to help you execute a function after a certain wait time, since the last time it was called.
Avoids executing the function too many times when the user interacts continuously (e.g., scrolling, typing)
# Usage
```js
import debounce from 'debounce-function';

const myFunction = () => {
  // ...
};

const debouncedFunction = debounce(myFunction, 1000);

// Call debouncedFunction multiple times
debouncedFunction();
debouncedFunction();
debouncedFunction();

// After 1000ms, myFunction will only be executed once
```

# Parameters
- `func`: The function to debounce
- `wait`: The wait time in milliseconds
- `immediate`: (Optional) If `true`, the function will be executed immediately, then wait wait ms before executing the next time. Default is `false`.

# Usage examples
- Debounce the click event of a button to avoid submitting a form repeatedly
- Debounce the scroll event to only update content when the user stops scrolling
- Debounce the keyup event to only perform a search after the user has finished typing a string
# Contributing
You can contribute to this package by submitting a pull request on GitHub.
