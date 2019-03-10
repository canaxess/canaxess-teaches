# Support for dynamic content #
In the last video we covered how to identify the conversation. We used the `ARIA-LABEL` attribute to provide a better name for each conversation and we enhanced this by adding a timestamp to make it easier to understand the message history, and to provide a unique name for every message.

This video shows how to support dynamic content. We'll use an `ARIA-LIVE` attribute to make each `SECTION` element be announced through the screen reader and we'll explain how to use the `ARIA-LIVE` value to increase the priority of when new content is announced.
Things to consider

Screen reader users navigate onscreen content audibly. If parts of the screen change visually, we need to ensure the change is identifiable programmatically as well. By making a change programmatically identifiable the screen reader monitors what has changed and announces the change audibly.

Looking at the code, every conversation block is rendered within a parent section container which has the ID of `conversation-body`. When a new message is received either from the bot or user it is added into this container. To trigger the screen reader to announce the change audibly the attribute `ARIA-LIVE` is added with a value of polite.

Accessible Rich Internet Applications (ARIA) are a collection of attributes which can be added to HTML to make screen readers and other assistive technology programmatically aware of dynamic changes to the interface.

When new content is added to the conversation-body container, the `ARIA-LIVE` attribute causes the screen reader to announce the new content audibly. The value **polite** determines how the screen reader should prioritise announcing the message. 

Screen readers announce all content audibly and there may be a buffer of previous content which is currently being announced. A value of **polite** will pause announcing new messages until existing messages have been announced first. The priority can be increased by changing to a value of **assertive**, which causes all existing messages being announced by the screen reader to pause and the chatbot messages to take priority. Unless a message is urgent, there is little need to use assertive.

Clicking the button named "click" will cycle through a simulated chatbot conversation with the messages output to the container with a short delay, the screen reader NVDA is running and will announce the new content audibly.

_[Hello, I see you're looking at loans can I book you into see one of our lenders? Chatbot conversation]_<br>

_[That would be great, can I book in for Monday? Chatbot conversation]_<br>

_[What's the closest branch to you? Chatbot conversation]_<br>

_[I'm in Canberra, so it's the city branch Chatbot conversation]_<br>

_[Great, I've booked you in to speak to one of our lenders on Monday Chatbot conversation]_<br>

It's important to understand the `ARIA-LIVE` attribute and value cannot be added dynamically and must be present when the page loads. The assistive technology needs to be aware of the live region before it can begin monitoring for changes.

We showed how the `ARIA-LIVE` attribute triggers assistive technology (in this case a screen reader) to announce newly updated and dynamic content. And how messages can be announced according to the priority value. 

A value of **polite** adds the message to the existing queue of content to be announced whilst **assertive** jumps the queue and is announced immediately.

Check the descriptions below for background information, WCAG 2 success criteria, links to the transcript and completed HTML source on GitHub and remember to like and share.
