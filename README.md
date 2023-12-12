# Autocomplete Demo
This project demonstrates a basic autocomplete functionality using JavaScript.

## Overview
The index.html page contains a textarea for user input and a div to display autocomplete suggestions.

When the user types in the textarea, the input value is saved and used to fetch suggestions from a mock API endpoint. The suggestions are displayed below the textarea.

Pressing the tab key will insert the currently displayed suggestion into the textarea.

## Code Explanation
`fullPageEditor` references the textarea element
`autocompleteText` references the suggestion display div
`lastText` tracks the last input value
An input event listener on the textarea saves the current input on each keystroke.

The `fetchSuggestions()` function makes a POST request to the mock API, passing the input text. This would normally return an array of suggestions.

A keydown event listener checks for tab presses. If tab is pressed, it inserts the current suggestion into the textarea.

## Future Improvements
Areas that could be expanded:

- Implement actual API call/response for suggestions
- Highlight matched text in suggestions
- Add filtering as user types
- Support selecting suggestions with arrow keys