# Jquery PasswordField [Demo](https://prefect9.github.io/Jquery-PasswordField/demo/)
## Dependencies
For the library to work, you need to connect [jQuery](https://jquery.com/download/). JQuery need to be connected before the \<script\> tag with the FormField library.



## Documentation
You need to initialize the \<div\> container that contains the input with the password and the button that shows/hides the password.

For automatic initialization, add the `data-password-field` attribute to the container with the password field.

For js-initialization, use the `$("#field_container").passwordField()` method.

If the password is shown, the `data-password-shown="true"` attribute will be added to the container. The button that shows/hides the password must contain the attribute `data-password-field-btn' and be inside the container.



## Examples
```html
<div data-password-field>
    <input type="password">
    <div data-password-field-btn><span>Show</span><span>Hide</span></div>
</div>
```
```css
[data-password-field-btn] > span:nth-child(2){ display: none }
[data-password-shown] > [data-password-field-btn] > span:nth-child(1){ display: none }
[data-password-shown] > [data-password-field-btn] > span:nth-child(2){ display: block }
```
