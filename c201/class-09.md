# Forms and JS Events

## Forms

There are several types of form controls

- Adding text, think search bar

- Making choices, think check boxes

- submitting forms

To diffrentate data forms use name/value pairs

```js
// name     value
username = Ivy
vote = herb
```

## Form Structure

```js
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>

```
<cite> HTML Forms, https://www.w3schools.com/html/html_forms.asp</cite>


### Fieldset and legends

- fieldset are uses to group together controls in a related element
- legends are captions explaining purpure of set

```js

<fieldset>
  <legend>Name input</legend>
  <form action="/action_page.php">
    <label for="fname">First name:</label><br>
    <input type="text" id="fname" name="fname" value="John"><br>
    <label for="lname">Last name:</label><br>
    <input type="text" id="lname" name="lname" value="Doe"><br><br>
    <input type="submit" value="Submit">
  </form>
</fieldset>

```

## Events

- Interactions create Events
- events trigger code
- code responds to user

### Event types
pg.246

#### Terminology

- *Fired* or *Raised* - When a event has occured
- *Trigger* - When a event sets code in motion

- #### __UI__

  - when user interacts with browser

    - webpage loads
    - webpage unloads
    - browser window resized
    - etc..

- #### __Keyboard__

  - when user interacts with keyboard

    - key down
    - key press
    - etc..

- #### __Mouse Events__

  - when user interacts with mouse

    - click
    - dblckick
    - etc..

- #### __Form Events__

  - when user interacts with form element

    - input - Value of input or text area has changed
    - change - Value select box or checkbox has changed
    - submit - User submits a form
    - etc...

### How events trigger javascript
  
  1. Select element you want script to respond together
  2. Indicate which event on selected nodes will Trigger
  3. Select the code you want to run
