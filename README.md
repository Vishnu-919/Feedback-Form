# Feedback-Form

# Feedback Form

A simple HTML feedback form that allows users to submit their name, message, and satisfaction level. The form uses basic client-side validation and displays a thank-you alert on submission.

---

## 📋 Features

- Text input for user name
- Textarea for detailed feedback
- Radio buttons to rate satisfaction
- Form validation using HTML5 `required` attributes
- Custom alert message on submission (no page reload)

---

## 🚀 How to Use

1. Clone or download this repository.
2. Open the `index.html` file in your web browser.
3. Fill out the form with your name, feedback message, and satisfaction level.
4. Click **Submit**.
5. A browser alert will confirm your submission.

> Note: The form does **not** send data to a server. It simply shows an alert. You can extend it to use JavaScript or connect it to a backend.

---

## 🧾 Form Structure

```html
<form onsubmit="alert('Thank you for your feedback!'); return false;">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required>

    <label for="message">Feedback:</label>
    <textarea id="message" name="message" rows="5" cols="40" required></textarea>

    <label>How satisfied are you?</label>
    <input type="radio" id="satisfied" name="satisfaction" value="Satisfied" required>
    <label for="satisfied">Satisfied</label>
    <input type="radio" id="unsatisfied" name="satisfaction" value="Unsatisfied" required>
    <label for="unsatisfied">Unsatisfied</label>

    <button type="submit">Submit</button>
</form>



🗂️ File Structure

feedback-form/
├── index.html
└── README.md

