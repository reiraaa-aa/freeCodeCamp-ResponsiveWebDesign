# HTML Fundamentals

This document outlines core HTML concepts, covering basic structure, semantic elements, media inclusion, lists, forms, and input.

## I. Basic HTML Structure and Elements

### A. HTML Tags:

* HTML elements have opening tags like `<h1>` and closing tags like `</h1>`.
* The text an element will display goes between its opening and closing tags.

### B. Headings (h1-h6):

* The `h1` through `h6` heading elements are used to signify the importance of content below them.
* The lower the number, the higher the importance, so `h2` elements have less importance than `h1` elements.
* Only use one `h1` element per page and place lower importance headings below higher importance headings.
* When you add a lower rank heading element to the page, it's implied that you're starting a new subsection.

### C. Paragraphs (p):

* The `p` element is used to create a paragraph of text on websites.

### D. Comments:

* Commenting allows you to leave messages without affecting the browser display.
* It also allows you to make code inactive.
* A comment in HTML starts with ``.

## II. Semantic HTML5 and Structure

### A. Semantic Elements:

* HTML5 has some elements that identify different content areas. These elements make your HTML easier to read and help with Search Engine Optimization (SEO) and accessibility.

### B. Main Content (main):

* The `main` element is used to represent the main content of the body of an HTML document.
* Content inside the `main` element should be unique to the document and should not be repeated in other parts of the document.

### C. Sections (section):

* The `section` element is used to define sections in a document, such as chapters, headers, footers, or any other sections of the document.
* It is a semantic element that helps with SEO and accessibility.

### D. Figures and Captions (figure, figcaption):

* The `figure` element represents self-contained content and will allow you to associate an image with a caption.
* A figure caption (`figcaption`) element is used to add a caption to describe the image contained within the `figure` element.

## III. Adding Media and Links

### A. Images (img):

* You can add images to your website by using the `img` element.
* `img` elements have an opening tag without a closing tag.
* An element without a closing tag is known as a void element.
* HTML attributes are special words used inside the opening tag of an element to control the element's behavior.
* The `src` attribute in an `img` element specifies the image's URL (where the image is located).

### B. Links (a):

* You can link to another page with the anchor (`a`) element.
* To open links in a new tab, you can use the `target` attribute on the anchor (`a`) element.
* The `target` attribute specifies where to open the linked document. `target="_blank"` opens the linked document in a new tab or window.

## IV. Lists and Emphasis

### A. Unordered Lists (ul, li):

* To create an unordered list of items, you can use the `ul` element.
* The `li` element is used to create a list item in an ordered or unordered list.

### B. Ordered Lists (ol, li):

* The code for an ordered list (`ol`) is similar to an unordered list, but list items in an ordered list are numbered when displayed.

### C. Emphasis (em):

* To place emphasis on a specific word or phrase, you can use the `em` element.

## V. Forms and Input

### A. Forms (form):

* The `form` element is used to get information from a user like their name, email, and other details.
* The `action` attribute indicates where form data should be sent.

### B. Input Elements (input):

* The `input` element allows you several ways to collect data from a web form.
* Like `img` elements, `input` elements are a void element and do not need closing tags.
* There are many kinds of inputs you can create using the `type` attribute. You can easily create a password field, reset button, or a control to let users select a file from their computer.
* In order for a form's data to be accessed by the location specified in the `action` attribute, you must give the text field a `name` attribute and assign it a value to represent the data being submitted.
* Placeholder text is used to give people a hint about what kind of information to enter into an input.
* To prevent a user from submitting your form when required information is missing, you need to add the `required` attribute to an `input` element. There's no need to set a value to the `required` attribute. Instead, just add the word `required` to the `input` element, making sure there is space between it and other attributes.
* In order to make a checkbox checked or radio button selected by default, you need to add the `checked` attribute to it.
* There's no need to set a value to the `checked` attribute. Instead, just add the word `checked` to the `input` element, making sure there is space between it and other attributes.

### C. Buttons (button):

* The `button` element is used to create a clickable button.
* Even though you added your button below the text input, they appear next to each other on the page. That's because both `input` and `button` elements are inline elements, which don't appear on new lines.
* The button you added will submit the form by default. However, relying on default behavior may cause confusion.

### D. Labels (label):

* `label` elements are used to help associate the text for an `input` element with the `input` element itself (especially for assistive technologies like screen readers).
* There's another way to associate an `input` element's text with the element itself. You can nest the text within a `label` element and add a `for` attribute with the same value as the `input` element's `id` attribute.

### E. Radio Buttons:

* You can use radio buttons for questions where you want only one answer out of multiple options.
* Remember that an `input` element is a void element.
* Notice that both radio buttons can be selected at the same time. To make it so selecting one radio button automatically deselects the other, both buttons must have a `name` attribute with the same value.
* If you select the `Indoor` radio button and submit the form, the form data for the button is based on its `name` and `value` attributes. Since your radio buttons do not have a `value` attribute, the form data will include `indoor-outdoor=on`, which is not useful when you have multiple buttons.

### F. Checkboxes:

* Forms commonly use checkboxes for questions that may have more than one answer. The `input` element with a `type` attribute set to `checkbox` creates a checkbox.
* Like radio buttons, form data for selected checkboxes are `name` / `value` attribute pairs. While the `value` attribute is optional, it's best practice to include it with any checkboxes or radio buttons on the page.

### G. ID attribute:

* The `id` attribute is used to identify specific HTML elements. Each `id` attribute's value must be unique from all other `id` values for the entire page.

### H. Indentation:

* Nested elements should be placed two spaces further to the right of the element they are nested in. This spacing is called indentation and it is used to make HTML easier to read.
