❌ Bad Code:
```javascript
function example() {
    console.log('Hello World');
}
```

🔍 Issues:
*   **Documentation Missing:** Even for simple functions, it's a best practice to include a docstring (e.g., JSDoc for JavaScript) explaining its purpose, parameters (if any), and return value (if any). This greatly enhances code readability and maintainability for future developers.
*   **Generic Naming:** The function name `example` is too generic. In a production environment, function names should be descriptive and clearly indicate their specific responsibility (e.g., `logGreeting`, `displayWelcomeMessage`). This improves code clarity and makes the code easier to navigate.
*   **Lack of Defined Purpose in Context:** While functionally correct, a senior reviewer would question the ultimate purpose of such a simple, generic logging function within a larger application. Functions typically serve a more specific, business-oriented role.

✅ Recommended Fix:

```javascript
/**
 * Displays a simple "Hello World" greeting message to the console.
 * This function is typically used for basic demonstrations or initial testing purposes.
 */
function logGreeting() { // Renamed for clarity and specific action
    console.log('Hello World');
}

// Example of how it might be called:
// logGreeting();
```

💡 Improvements:
*   ✔ **Enhanced Readability:** The added docstring provides immediate context and understanding of the function's intent.
*   ✔ **Improved Maintainability:** Clear documentation and descriptive naming make the codebase easier to understand, modify, and debug over time.
*   ✔ **Contextual Naming:** Renaming `example` to `logGreeting` accurately describes the function's action, aligning with best practices for clear code.
*   ✔ **Promotes Consistency:** Encourages the habit of documenting all functions, leading to a more consistent and professional codebase.