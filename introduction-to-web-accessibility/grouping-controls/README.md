# Transcript #

Grouping related controls together can help a user understand relationships more clearly between components. For example, form controls for an address may be grouped visually next to each other, but if the user is unable to identify the visual grouping any relationship between controls can be difficult to understand.

In this lecture I'll show how to group related controls together semantically. I'll explain why you may want to apply groupings to similar controls and how to use semantic HTML to ensure the grouping is identifiable via a screen reader and therefor perceivable to a larger collection of users.

At the end of this lecture you'll understand how to group related form controls together using semantic HTML to allow screen reader users to understand related controls. You'll understand that although grouping is a good way of creating relationships which are conveyed without relying on the way components are arranged, the technique should be used only when necessary.

The way form controls are laid out on screen can help and enhance the understanding of relationships and how controls relate to each other. 

A collection of dropdown list controls for a date of birth may be understandable when adjacent to each other, but if a user can't perceive the visual grouping, they will only hear the individual labels and be unclear how they relate to each other. 

They may guess it’s a grouping of controls requiring the date of birth, but when a relationship becomes complex, grouping controls together semantically can help a user understand how components relate to each other. 

In the previous lecture "add labels to controls", a label provided a description of the individual control. But to identify groups of controls which are related the fieldset and legend elements can be used to provide a description for the whole group. This grouping mechanism triggers a screen reader to announce the legend text before the label text of each control.

Form controls can be grouped together using the fieldset and legend elements, all controls which are contained within the fieldset are then related. The legend element is the first element within the fieldset, and this describes the grouping and what is announced by the screen reader. When a screen reader focuses on any control within the fieldset the legend text is announced prior to the label of each control.

Grouping controls using the fieldset and legend element is most important for radio buttons and checkboxes. The individual label for each control may be insufficient to describe the whole groups description. 

In this example there are several controls asking a user to select their shipping options, the label of each control describes the value but not the relationship to each other. In this instance grouping must be used to provide an additional description.

The numerous shipping options could therefore be enhanced by wrapping all of the radio buttons within a fieldset element and use the legend element to provide an extra level of description. When each control receives focus, the legend text will be announced first followed by the control label.

The technique is a convenient way to provide an additional level of detail for controls which may have an unclear relationship. However, don’t overuse it. Only use it where there is a need to provide additional relationship information. Because a screen reader conveys onscreen information audibly extra irrelevant content is announced which can become fatiguing.

Using the fieldset and legend elements for additional relationship information is covered by the HTML specific technique H71: Providing a description for groups of form controls using fieldset and legend elements which means this has passed success criterion 1.3.1 Info and Relationships: Information, structure, and relationships conveyed through presentation can be programmatically determined or are available in text at level A.

Using fieldset and legend elements are a great way to group related controls together. When controls are contained within this grouping the screen reader announces the legend text followed by the control label so it’s a convenient way to describe a collection of related controls which belong together. 

Although it can be applied to all controls, its best suited to use for checkboxes and radio buttons where the individual label for each control may be insufficient to describe the whole groups description.

This video is from our Introduction to Web Accessibility WCAG 2.1 Udemy course. The course is designed to teach you the fundamentals of web accessibility and how to apply those techniques to websites that you create. If you're interested in finding out a little more, checkout the link in the description below as well as links to a full transcript.

If you want to stay up to date with web accessibility and to learn cutting edge techniques, consider subscribing and click the bell icon to be notified when new videos are uploaded.
