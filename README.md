# ENGLISH DICTIONARY PROJECT

## what learnt

- 1 using the addEventListener method
- 2 using fetch() API method
- 3 How to handle error

- 4 using try catch method
- 5 using audio tag in html

## using addEventListener

### An event listener is a procedure in JavaScript that waits for an event to occur.

### The addEventListener() is an inbuilt function in JavaScript which takes the event to listen for, and a second argument to be called whenever the described event gets fired

### The addEventListener() method makes it easier to control how the event reacts to bubbling.

### When using the `addEventListener() `method, the JavaScript is separated from the HTML markup, for better readability and allows you to add event listeners even when you do not control the HTML markup

### Example

### Alert "Hello World!" when the user clicks on an element:

```
element.addEventListener("click", myFunction);

function myFunction() {
  alert ("Hello World!");
}
```

### The first parameter is the type of the event (like "click" or "mousedown" or any other HTML DOM Event.)

### The second parameter is the function we want to call when the event occurs.

### The third parameter is a boolean value specifying whether to use event bubbling or event capturing. This parameter is optional.

# 4 using try catch method

### The <b><u>`try`</u></b> statement allows you to define a block of code to be tested for errors while it is being executed.

### The <b><u>`catch`</u></b> statement allows you to define a block of code to be executed, if an error occurs in the try block.

### The `try` and `catch` keywords come in pairs:

### The catch statement allows you to define a block of code to be executed, if an error occurs in the try block.

### The try statement always starts with a try block. Then, a catch block or a finally block must be present.

## Example

```js
function test {

    try {
      const name = "user";
      name = "newUser";
    } catch ( e) {
      console.log("Something went wrong.");
    }

}

```

## the output will be `something went wrong.` since we tried reassigning a constant

# 4. Using the Fetch Api in Javascript

### The Fetch API is a modern interface that allows you to make HTTP requests to servers from web browsers.

### The fetch() method is available in the global scope that instructs the web browsers to send a request to a URL.

## Sending a Request

### The fetch() requires only one parameter which is the URL of the resource that you want to fetch:

```js
let response = fetch(url);
```

## Using async/await with fetch

### A better and cleaner way of handling the promise is through the async/await keywords. You start by specifying the caller function as async and then use await to handle the promise.

## EXAMPLE

```js
async function getResponse() {
  const response = await fetch(
    "https://carbonfootprint1.p.rapidapi.com/CarbonFootprintFromCarTravel?distance=100&vehicle=SmallDieselCar",
    {
      method: "GET",
      headers: {
        "x-rapidapi-host": "carbonfootprint1.p.rapidapi.com",
        "x-rapidapi-key": "your_api_key",
      },
    }
  );
}
```

### Because of the await keyword, the asynchronous function pauses until the promise is resolved. The Response object is assigned to response once the request completes.

# using audio tag in html

## The `<audio>` tag is used to embed sound content in a document, such as music or other audio streams.

## example

```html
<audio controls>
  <source src="horse.ogg" type="audio/ogg" />
  <source src="horse.mp3" type="audio/mpeg" />
  Your browser does not support the audio tag.
</audio>
```

### You can access an `<audio>` element by using getElementById():
