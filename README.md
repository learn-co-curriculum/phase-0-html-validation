# HTML Validation
## Problem Statement 

By now, you've probably noticed that the nested structure of HTML elements lends itself to multiple typos, as well as the opportunity to wonder if you've actually closed all of your tags or not. While text editors can help, and modern day browsers are pretty good at compensating for malformed HTML, neither can always accurately predict a developer's intentions. Additionally, what Chrome chooses to display when an HTML error occurs could be very different from what Safari, Firefox, Internet Explorer, or any other browser chooses to display. How can we be certain that the HTML that we are writing is both within the current HTML standards, and error-free? Luckily, there are validation services that can help.

## Objectives
1. Identify W3C organization.
2. Validate sample HTML.

## Identify W3C organization and available HTML validation tools. 

The World Wide Web Consortium (W3C) is an international community that develops open standards to ensure the long-term growth of the web. It operates under a strict [code of ethics and professional conduct](https://www.w3.org/Consortium/cepc/) and provides many [free tools](https://www.w3.org/developers/tools/) for developers.

## Validate sample HTML. 

Look for the file named `example_code.html`. Open the file in your web browser (if you are working in the IDE, [this](http://help.learn.co/the-learn-ide/common-ide-questions/viewing-html-pages-in-the-learn-ide) might help). It looks relatively ok, right? There's some oddness happening with the list at the bottom (we might not have wanted everything hyperlinked), and there's an odd bullet point with no content, but everything else looks pretty good. 

Now let's try validating the code to identify where we went wrong.
1. Open the `example_code.html` file in your IDE or text editor.
2. Select the whole HTML contents in the file, and copy it.
3. In your web browser, navigate to [W3C's HTML Validator](https://validator.w3.org/#validate_by_input).
4. If not already selected, select the tab that says "Validate by Direct Input". 
5. Paste all of your copied HTML in the text box labeled "Enter the Markup to validate:"
6. Click the button labeled "Check".

As you scroll down the page, you should see a list of errors, or invalid HTML.

### What is HTML Validation? 
Just as documents written in regular languages can have errors, so too can HTML. These can range from missing angle brackets to wrong or missing opening or closing tags, unnecessary or missing attributes, and many other issues. As stated above, modern browsers are pretty good at filling in the missing pieces, but with unpredictable results. By using tools like W3C's HTML Validator, we can catch these errors and prevent our user from having a poor experience. 

### A Valid HTML Experience 
Now, let's see what a valid HTML file returns. 

1. Open the `example_code_passing_validation.html` file in your IDE or text editor.
2. Select the whole HTML contents in the file, and copy it.
3. In your web browser, navigate to [W3C's HTML Validator](https://validator.w3.org/#validate_by_input).
4. If not already selected, select the tab that says "Validate by Direct Input". 
5. Paste all of your copied HTML in the text box labeled "Enter the Markup to validate:"
6. Click the button labeled "Check".

You should see a green bar denoting that there are no errors or warnings to show. 

### A note about cross-browser compatibility 


## Key Terms

## Resources
[W3C](https://www.w3.org/)
[HTML Validation Tool](https://validator.w3.org/)
[Why Validate?](https://validator.w3.org/docs/why.html)

<iframe width="640" height="480" src="//www.youtube.com/embed/nYglnxMUixM?rel=0&modestbranding=1" frameborder="0" allowfullscreen></iframe>

<p><a href="https://www.youtube.com/watch?v=nYglnxMUixM">HTML Validation</a></p>.

<p data-visibility='hidden'>View <a href='https://learn.co/lessons/html-validation' title='HTML Validation'>HTML Validation</a> on Learn.co and start learning to code for free.</p>
