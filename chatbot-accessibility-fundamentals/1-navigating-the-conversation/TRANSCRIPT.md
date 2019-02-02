# Navigating the Conversation #
This video explains how to make a chatbot conversation history accessible. We'll explain why the conversation must be navigable and why we need to make it work with the mouse and keyboard. 

We'll Use the CSS property `OVERFLOW-Y` to make a `SECTION` element scroll vertically with overflowing content. And add the `TABINDEX` attribute to make the element appear in the keyboard focus sequence.

All users need to be able to navigate through the entire conversation history at any point when talking to a bot. But, if we only allow navigation via the mouse, keyboard users will be unable to see the history. So, we need to build in extra keyboard support, and when we build in the keyboard support we also need to make the element appear in the keyboard tab sequence.

If we look at the code, every conversation is rendered in a `SECTION` element which alternate between messages from the bot and messages from the user. `SECTION` elements can help a screen reader user by providing better context than generic `DIV` elements, in essence a `SECTION` element means this content is special and within the screen reader a user can usually navigate to named regions on the page.

Every `SECTION` element is rendered within a further `SECTION` element which is the chatbot conversation window and this contains all of the conversation history. We've set to this to a fixed height of `150px` and the `OVERFLOW` property set to `HIDDEN`. 

The conversation window has content which overflows the fixed height dimensions. But because the `OVERFLOW` property is set to `HIDDEN`, we're unable to see further messages. This is changed by removing the `OVERFLOW` property and adding the property `OVERFLOW-Y` with a value of `SCROLL`. 

This means when the content overflows the `SECTION` elements fixed height, a vertical scrollbar appears and we can scroll through the entire conversation history.

Even though we've now made the entire conversation history viewable a user navigating with the keyboard won't be able to scroll the conversation history as `SECTION` elements don’t receive keyboard focus. Add the attribute `TABINDEX` and the value of 0 to the parent `SECTION` containing all of the children elements. This makes it focusable from the keyboard and a value of 0 makes it appear in the regular keyboard ordering sequence of the other focusable page elements.

We covered why the conversation history must be navigable and how to go about it. We used the CSS property overflow-y to make a SECTION element accommodate for overflowing content, and we used the TABINDEX attribute to make the SECTION element appear in the keyboard sequence. 

When the conversation overflows a vertical scrollbar appears. Adding `TABINDEX` to this `SECTION` element then makes the element appear in the keyboard tab sequence and the up and down arrow keys are used to scroll through the container.

Check the descriptions below for background information, WCAG 2 success criteria, links to the transcript and completed HTML source on GitHub and remember to like and share.
