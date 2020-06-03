# Transcript #

Nearly all form elements need a label. Without a label form controls that receive keyboard focus will only announce the type of control to the screen reader user not what type of data is required. When a label doesn’t provide enough information describing what to enter, more errors are likely. 

In this lecture I'll explain the label element and show how correctly labelling controls makes it much easier for a screen reader user to understand the type of data a control requires. 

I'll use the FOR and ID attributes to create a programmatic relationship between labels and form controls, this programmatic relationship means when the control receives keyboard focus the label element will be announced automatically by the screen reader.  

By the end of this lecture you'll understand why labels are critical in helping a user understand the type of input a form control requires and you'll know how to use the FOR and ID attributes to create a programmatic relationship which triggers the screen reader to announce the label when the control receives keyboard focus.

When form controls receive keyboard focus, the screen reader will announce the type of control. Form controls often have a text label adjacent to the control which gives the user a hint as to what type of information is required, if the input control had a label of first name, you'd know that that control accepts a first name. 

However just relying on physical placement of the label to provide that information means screen reader users won't be able to understand what type of data the control requires.

When the control receives focus it will only announce the type of input control not the adjacent label, the screen reader may announce “input type and text”. It's an input control and the type of input is text, the screen reader user is aware a control is there but not what data the control requires because the label hasn't been programmatically associated to the control. Because the label is not programmatically associated, the label remains unannounced effectively hidden.

Creating a relationship between a label element and the input control overcomes this by using the FOR attribute on the label element with the ID of the form control. In this example the ID of the input control is "firstname" and this is the value in the FOR attribute on the label. A programmatic relationship is then created, this establishes a physical connection which the screen reader can use when the form control receives focus.

When the same process of navigating through the form is repeated. On keyboard focus the screen reader will announce the text label describing the type of input required for the control, providing a really clear indication that the control is for a certain type of data. In our example it will announce “first name input type and text”.

Not all form controls require an explicitly associated label, the following controls do require a label:

*	Text input
*	Checkbox
*	Radio button
*	File upload
*	Password 
*	Textarea
*	Select

Several controls don’t require a label, as a text description is provided by the value attribute of the control, the ALT attribute or content within the element:

* Submit and reset buttons have a text description provide by the value attribute
* Image buttons have the description provided by the ALT attribute of the control
* Hidden input fields don’t require a text description
* Button elements have the description provide by the enclosed text

An additional benefit of programmatically associating a label to a form control is it provides a larger clickable area for the control. Rather than just clicking within the control to activate it, the activation can now happen from either the label or the control which is especially helpful for users with dexterity problems as it presents a large clickable area.

Using programmatically associated labels with form controls satisfies the HTML specific technique H44 Using label elements to associate text labels with form controls which means this has passed success criterion 1.3.1 Info and Relationships: Information, structure, and relationships conveyed through presentation can be programmatically determined or are available in text at level A.

Using programmatically associated labels with form controls is a nice quick win to improve the accessibility of online forms. I showed how to associate a label to a form control using the FOR and ID attributes, explained which form controls require a label and which don’t and describe an additional benefit of a larger clickable area to activate a control.

This video is from our Introduction to Web Accessibility WCAG 2.1 Udemy course. The course is designed to teach you the fundamentals of web accessibility and how to apply those techniques to websites that you create. If you're interested in finding out a little more, checkout the link in the description below as well as links to a full transcript.

If you want to stay up to date with web accessibility and to learn cutting edge techniques, consider subscribing and click the bell icon to be notified when new videos are uploaded.
