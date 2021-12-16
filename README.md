# HTML Validation

## Learning Goals

- Identify W3C organization
- Validate sample HTML
- Identify HTML errors

## Introduction

You have written a few HTML pages by now. Did you accidentally break nesting and
put emphasis on a whole page? Or did you type `<he>` instead of `<h3>`? How can
we guard HTML? Many editors try to catch errors for us, and most browsers are
pretty good at guessing what you meant. But what happens when Windows Edge
guesses differently than Google Chrome? How can we be certain that our HTML
meets standards and is error free? Luckily, the W3C – the people who define the
tags of HTML – have a validation service we can use. We'll explain the W3C and
their validator in this lesson.

## Identify W3C organization

The World Wide Web Consortium (W3C) is an international community that develops
open standards to ensure the long-term growth of the web. It operates under a
strict [code of ethics and professional
conduct](https://www.w3.org/Consortium/cepc/) and provides many [free
tools](https://www.w3.org/developers/tools/) for developers.

## Validate sample HTML

Take a look at this file: [`example_code.html`][s3-invalid] in a new tab. We'll
call this the **viewing tab**. It looks relatively OK, right? There's some
oddness happening with the list at the bottom (we might not have wanted
everything hyperlinked), and there's an odd bullet point with no content, but
everything else looks pretty good.

Now let's try validating the code to identify where we went wrong.

1. In your **viewing tab**, navigate to View &rarr; Developer &rarr; View Source
   _or_ press Command-Option-U. This will give you the "Source View" of the
   document
2. Select the whole of the HTML contents in the file, and copy them
3. In your web browser, open a new tab to [W3C's HTML Validator][valid8r]
4. If not already selected, select the tab that says "Validate by Direct Input"
5. Paste all of your copied HTML in the text box labeled "Enter the Markup to
   validate:"
6. Click the button labeled "Check"

As you scroll down the page, you should see a list of errors, or invalid HTML.

### What is HTML Validation?

Like all other programming languages, HTML can contain all kinds of different
errors. These can range from missing angle brackets to wrong or missing opening
or closing tags, unnecessary or missing attributes, and many other issues. Our
web browsers are pretty good at filling in the missing pieces but we can't
always count on it being the same experience with every one. Tools like W3C's
HTML Validator can catch these errors and prevent our user from having a poor
experience.

## Identifying HTML Errors

Now that we have a page full of HTML validation errors, how do we start fixing
them? There are several parts of the error message that will help us parse the
error, and figure out exactly where it is and what we can do to fix it.

### Error Description

The first line of the error is our error description. This is a narrative that
gives us a little bit more information about our error.

![HTMLValidationErrors](https://s3.amazonaws.com/learn-verified/html-error-description.png)

In this case, it's saying that there was an ending `</h2>` tag, but there was a
different opening tag that came before it.

### Error Location

The second and third lines of this error give us the exact location of the
error, as well as a highlighted snippet of our HTML to help us exactly locate
where the error is.

![HTMLValidationErrorLocation](https://s3.amazonaws.com/learn-verified/html-error-location.png)

In this case, it's letting us know that our error is on line 10, from column
34-38. Line numbers will become very important in troubleshooting errors, in
JavaScript and CSS as well as HTML. These error messages can serve as a road map
to us, and help us troubleshoot much more efficiently.

### A Valid HTML Experience

Now, let's see what a valid HTML file returns.

1. Open the [`example_code_passing_validation.html`][s3-valid] file in a new
   tab. This will now be our new **viewing tab**
2. In your **viewing tab**, navigate View &rarr; Developer &rarr; View Source
   _or_ press Command-Option-U. This will give you the "Source View" of the
   document
3. Select the whole of the HTML contents in the file, and copy them
4. In your web browser, navigate to [W3C's HTML Validator][valid8r] in a new
   tab
5. If not already selected, select the tab that says "Validate by Direct
   Input"
6. Paste all of your copied HTML in the text box labeled "Enter the Markup to
   validate:"
7. Click the button labeled "Check"

You should see a green bar denoting that there are no errors or warnings to
show.

![HTMLValidationPassed](https://s3.amazonaws.com/learn-verified/html-passing-validation.png)

## Resources

- [W3C](https://www.w3.org/)
- [HTML Validation Tool](https://validator.w3.org/)
- [Why Validate?](https://validator.w3.org/docs/why.html)

[s3-invalid]: https://curriculum-content.s3.amazonaws.com/web-development/html-validation/example_code.html
[s3-valid]: https://curriculum-content.s3.amazonaws.com/web-development/html-validation/example_code_passing_validation.html
[valid8r]: https://validator.w3.org/#validate_by_input
