You don't know what sort of rubbish the end-user would enter in the text box that says input your email in the contact form so we add validations and error handling so that only email addresses may be entered in that input box.

Error handling and clean code have a very clear relation, Error handling is important in developing modern day software due to many factors(Slow network, old devices, etc..) but it shouldn't be the dominant force in your code base and obscure your logic.

Back in the distant past there were many languages that didn’t have exceptions. In those languages the techniques for handling and reporting errors were limited. You either set an error flag or returned an error code that the caller could check.

Using try-catch-finally statements in your code is a great way of catching errors. In a way, try blocks are like transactions. Your catch has to leave your program in a consistent state, no matter what happens in the try. 

For this reason it is good practice to start with a try-catch- finally statement when you are writing code that could throw 
exceptions.

## Catching bugs

If you don't use a try-catch block in your code and happen to run into an error the error won't be displayed and the program will just stop running, leaving the user in a bad mood and you puzzled as to what could have gone wrong.

Create informative error messages and pass them along with your exceptions. Mention the operation that failed and the type of failure. If you are logging in your application, pass along enough information to be able to log the error in your catch block.

## Wrap third-party APIs

wrapping third-party APIs is a best practice. When you wrap a third-party API, you minimize your dependencies upon it. 

You can choose to move to a different library in the future without much penalty. Wrapping also makes it easier to mock out third-party calls when you are testing your own code.

One final advantage of wrapping is that you aren’t tied to a particular vendor’s API design choices. You can define an API that you feel comfortable with.

## Never pass or return Null

Returning Null values instead of a proper return statement in function calls can be a real headache and the program will just go in a frenzy state if their isn't any null checks in the code.

If there is something that is even worse than returning null on function calls then it will have it to be passing Null as function or method arguments. Unless you are working with an API which expects you to pass null, you should avoid passing null in your code whenever possible.