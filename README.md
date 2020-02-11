# Lesson 6.0 Practice
## Asynchronous Programming w/ Callback Functions

### Directions
#### Abstracting Over `XMLHttpRequest`
1. Write a function `logData` that takes a URL string, makes a GET request to that URL and logs the response to the console. Test your function by making a call to the [JSON Placeholder API](https://jsonplaceholder.typicode.com/)

2. The above function is only able to log the AJAX call's response to the console. Let's make a function that is more flexible. Write a function called `get` that takes a URL string _and_ a callback function as arguments. This function makes a GET request to the passed URL and then invokes the given callback function on the response. Once again, test your function by making a call to the [JSON Placeholder API](https://jsonplaceholder.typicode.com/).

3. Test the above function with an incorrect endpoint (`'https://jsonplaceholder.typicode.com/postszz'`). Since this request results in a 404 response, our function does not give us much helpful information back. Add a condition that checks for a response status of `404`. For such responses, you should log, `"404: Resource not found."`

4. Let's get some practice using APIs that require a key. We will use [Open Weather Map](https://openweathermap.org/api). To use this API, you must sign up for an account to receive an API Key. Please sign up [here](https://openweathermap.org/home/sign_up).

5. Test out your above functions using the Open Weather API.
