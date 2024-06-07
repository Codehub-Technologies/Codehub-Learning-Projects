# Exercise: Fetching Data with Promises

### Task Description:
- Create a function `fetchData` that takes a URL as an argument and returns a Promise.
- Inside the `fetchData` function, use `setTimeout` to simulate a network request that takes 2 seconds to complete.
- If the URL is valid (e.g., "validURL"), the Promise should resolve with a success message.
- If the URL is invalid (e.g., anything other than "validURL"), the Promise should reject with an error message.
- Test the `fetchData` function by calling it with both a valid and an invalid URL, handling the resolved and rejected cases using `.then` and `.catch`.

Implementation:
- Define the `fetchData` function:
    - The function should return a new Promise.
    - Use `setTimeout` to simulate a delay.
    - Resolve or reject the Promise based on the URL.
- Test the `fetchData` function:
    - Call `fetchData` with a valid URL and handle the resolved value.
    - Call `fetchData` with an invalid URL and handle the rejected value.
