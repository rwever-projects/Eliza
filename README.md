# Eliza
http://www.public.asu.edu/~rwever/
## Client-side implementation
#### Languages: HTML, CSS, JS

![Eliza screenshot](https://github.com/rwever-projects/Eliza/blob/master/Eliza_Screenshot.png)

### Objective:
Implement a client-side single page browser-based web application with GUI interface.  (No server component is used).

This project features:
- DOM manipulations
- Event handling
- Browser-based storage solution
- Usage of JSON data structures

By parsing the user's input, a custom algorithm finds matches within its dictionary to select one of multiple appropriate responses.  This algorithm also introduces randomization to minimize the number of duplicate responses from the same input, so that no 2 sessions follow the same pattern of responses.

If users let 20 seconds lapse before providing a new input, the user is prompted with a dialog message.  This message also feature a randomization so that messages are not repeated.

The program also allows the user to input a new dictionary (in JSON format) from the input form.  This is added dynamically to the existing dictionary, and Eliza will announce: 'I just got smarter'.

Eliza is also stateful by saving responses to a user.  When the browser is closed and restarts, upon returning to Eliza the same user name is given to Eliza and the program restore the state of the application.

A 'clear' operation is also implemented so that it clears the state of the application for that user, then returns the application to the start form.
