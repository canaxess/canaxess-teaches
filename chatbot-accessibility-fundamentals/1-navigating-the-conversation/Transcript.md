# Navigating the Conversation
This video covers how to make a chatbot conversation history accessible. We'll use the CSS property `overflow-y` to make a scrollable DIV, and add the `tabindex` attribute to make this DIV appear in the keyboard focus sequence.

## Things to consider

All users need the option to navigate through the entire conversation history at any point when they're talking to a bot. But if we only allow the conversation history to be navigated via the mouse, keyboard users will be unable to access the content. This presents some interesting design decisions where we add attributes to make HTML elements work in different ways.

## How it is made accessible

If we look at the code, every conversation bubble is rendered in a DIV. As we can see they alternate between messages from the bot and messages from the user. All these DIVs are rendered within a further DIV element. This acts as the chatbot conversation window, and we've set to this to a fixed height of `150px` and the overflow property set to hidden. The conversation window has content which overflows the containers fixed height dimensions. Because the overflow property is set to hidden, we're unable to see further message bubbles.
We remove the overflow property and add the property overflow-y: scroll. This now displays a vertical scroll bar, which allows navigation of the entire conversation history.

Now ordinarily a DIV element doesn’t receive keyboard focus because it’s non-semantic. What this means is it has no meaning in HTML. Without keyboard focus its difficult for users who rely on the keyboard to navigate through the conversation history. To overcome this we add the attribute `tabindex` and the value of 0. Tabindex makes the element focusable from the keyboard, and a value of zero makes it appear in the normal keyboard ordering sequence of the page elements. 

We can add the `tabindex` attribute onto each message bubble so individual messages can become focusable from the keyboard. But the general view is to avoid adding behaviour onto elements which traditionally don’t have that default behaviour to begin with. 

## What we covered

In today's training session we covered making the conversation history navigable. We used the CSS property `overflow-y` to allow a DIV to accommodate for overflowing content, and we used the tabindex attribute to make the DIV appear in the keyboard sequence. 
When the conversation overflows a vertical scroll bar appears. Adding `tabindex` to this DIV allows the element to appear in the keyboard focus sequence with the up and down arrow keys used to scroll through the container.

Check the descriptions below for background information, WCAG success criteria, links to the transcript and GitHub source and remember to like and share.
