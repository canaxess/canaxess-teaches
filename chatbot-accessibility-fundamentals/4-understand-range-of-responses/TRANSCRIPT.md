# Understand the range of responses #
In the last video we covered how to support dynamic content. We used the `aria-live` attribute to trigger dynamically updating content to be announced by the screen reader, and used the value of polite to make the messages be announced after existing screen reader announcements.

This video shows how to add accessibility support into the range of bot responses. We'll step through several different response types and explain what needs to be added to ensure accessibility is maintained regardless of how the bot is responding.

Many bot frameworks return several different types of responses in addition to regular text, because of this we need to ensure accessibility is being maintained regardless of the type of response.

One such bot framework from Microsoft returns rich cards which allow a bot to reply in one of 7 templated card types including Hero Cards, Thumbnail Cards and Video Cards. These cards typically contain an image text and a button. 

Bot framework can also return an additional template called an adaptive card which can contain any combination of text, images, buttons and input fields.

Because of this variety of content being returned to the user we need to ensure we follow accessibility principles. These include:
* Provide all images with ALT attributes
* Programmatically associate labels to form controls

All images displayed as part of a rich card must have an `ALT` attribute. The `ALT` attribute is a way to provide alternative text to an image for users who may use a screen reader. 

When a screen reader user encounters an image which has an `ALT` attribute with text describing what the image is of, this is audibly announced. 

So, its vitally important to use `ALT` text which describes the image in such a way the user clearly understands what it means and what it is depicting. 

An image depicting Australia's parliament house may have `ALT` text describing its location. Avoid very short one-word descriptions as these rarely convey what an image is depicting or why it is important.

If the image is decorative no `ALT` text is required. If you're unsure whether to include `ALT` text or not, ask yourself, would a user benefit from understanding what the `ALT` text describes?

If the rich card has several form controls ensure each control (input, select, radiobutton, checkbox, textarea) all have a programmatically associated label. The label acts as a hint for the assistive technology user providing a description of what type of data the control requires. 

There are several ways to add a programmatically associated label:

* `FOR` and `ID` relationship
* `ARIA-LABEL` attribute

The `FOR` attribute value on the label element, uses the same value of the `ID` attribute on the form control. When the control receives keyboard focus, the assistive technology will announce the label text followed by the form control providing enough context of what the control represents.

There may be times when its impractical to use a visible label and the `FOR` and `ID` technique, use `aria-label` instead. `aria-label` is an attribute which is added to the control, when the assistive technology focuses on the control the `aria-label` value will be announced audibly.

If we look at the code, an adaptive rich card is displayed in the chatbot conversation container. It has an image, but because the image is decorative only and doesn’t really provide any benefit to the user we've included no `ALT` text (but we've still provided the `ALT` tag). 

There are several form controls each with a programmatically associated label. We've associated the label element to the input control using the `FOR` and `ID` attributes with the `ID` of the input control used as the value for the `FOR` attribute in the label. And we've used the `aria-label` attribute to provide a programmatically identifiable label on the home state selectbox. 

When each control receives keyboard focus the screen reader announces the label text followed by the control, we've used two different techniques to provide form controls with a programmatically associated name and both approaches are acceptable. 
If you find limitations with using a label element and the `FOR` and `ID` attributes, consider using the `aria-label` attribute instead.

We explained the variety of rich card types available on the Microsoft bot framework. And because of this variety you need to ensure that all content being outputted via rich cards need to follow principles for maintaining accessibility:

* Ensure all images have an `ALT` tag. If the image is decorative no `ALT` text is required. However, if an image requires a description this is where it would be written.

* Make sure all form controls have proper labelling for screen reader users to understand. Creating a programmatically associated label 
means screen reader users will understand what data is required when the form control receives focus. And we used 2 techniques, the label element using the `FOR` and `ID` values, and the `aria-label` attribute on the form control.

Check the descriptions below for background information, WCAG 2 success criteria, links to the transcript and completed HTML source on GitHub and remember to like and share.
