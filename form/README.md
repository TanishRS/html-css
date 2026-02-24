# Registration Form

A styled HTML registration form with required field validation, a gender dropdown, and a submit button.

## Files

| File | Description |
|------|-------------|
| `form.html` | Main HTML file with the form structure and two embedded style blocks |
| `form.css` | External stylesheet (linked but mostly commented out in practice) |

## HTML Concepts Used

- `<form>` element as the form container
- `<label>` with `for` attribute linked to input `id` for accessibility
- `<input type="text">` for Full Name
- `<input type="email">` for Email Address
- `<input type="password">` for Password
- `<input type="tel">` for Mobile Number
- `<select>` with `<option>` elements for Gender dropdown
- `required` attribute on all fields for native browser validation
- `placeholder` attribute on inputs for hint text
- `<input type="submit">` as the form submit button
- Multiple `<style>` blocks embedded inside `<head>`

## CSS Concepts Used

- Attribute selector `input[required]` and `select[required]` to apply a red border and pink background to all required fields
- Attribute selector `input[type="password"]` for a specific red border on the password field
- Attribute selector `input[type="submit"]` for the blue styled submit button
- `background-color`, `color`, `border-radius`, `padding` on the submit button
- `margin-top` for spacing between the submit button and the form fields
