# Django CRUD and Forms

## Django Forms

HTML Forms - use to create, update, and delete model instances

 HTML Form - a grouping of fields that are used to collect information users for submission to a server

Example Html Form

```html
<form action="/team_name_url/" method="post">
    <label for="team_name">Enter name: </label>
    <input id="team_name" type="text" name="name_field" value="Default name for team.">
    <input type="submit" value="OK">
</form>

```

Action - URL where data is to be sent for processing when the form is submitted

- If this is not set in the form, it will be submitted back to the current page

method - The HTTP method used to send the data

- POST - used if the data is going to result in a change to the server's database
- GET - used only if it does not change user data

### Form Fields

Common field arguments

- required - Field cannot be left blank
- label - Label to use when rendering form
- widget - displays a widget for use
- error_messages - list of error messages that can be overrided with a custome messages
- validators - list of functions that will be called on a field when it is validated
- help_text - text can be displayed in forms to help guide use

[Django Tutorial Part 9: Working with forms](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms)
