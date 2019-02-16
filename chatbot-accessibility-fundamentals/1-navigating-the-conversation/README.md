# Navigating the conversation
[This video](https://www.youtube.com/watch?v=pHvMPSL_2CM) shows you how to make the conversation history scrollable using the CSS property `overflow-y` and appear in the keyboard focus sequence by adding the attribute `tabindex`.

The conversation history of a chatbot must be navigable by the user with and without using the mouse. If we only provide support for mouse navigation it's unable to be used by keyboard users and means we fail a WCAG 2.0 AA success criteria. 

## CSS, HTML and User Agent compatibility ##

&nbsp;        | Internet Explorer 11 | Edge | Chrome 72 | FireFox Quantum 65
:------------- |:-------------:| :-----:| :-----:| :-----:
`overflow-y: scroll`    | YES | YES | YES | YES
`tabindex` | YES | YES | YES | YES
