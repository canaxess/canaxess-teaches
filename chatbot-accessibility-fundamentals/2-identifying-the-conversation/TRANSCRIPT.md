# Identifying the Conversation #
In the last video we covered how to make a chatbot conversation history navigable. We used the overflow-y property to make the `SECTION` element scroll vertically when its content overflowed, and the `TABINDEX` attribute to make it focusable from the keyboard.
This video explains how to make the conversation history identifiable to the user. We'll use the ARIA-LABEL attribute to add an identifier to each conversation, and add a timestamp to show when the message is received.

Vision impaired users can navigate onscreen elements through their screen reader without having to interact with the page. We need to make sure the conversation identifier (that is who spoke, was it the bot or the user) can be identified by text as well as visually. 
But this isn’t enough, adding a conversation identifier is great, but if you don’t know the sequence each message is spoken it becomes confusing if there are lots of messages.

Looking at the code, each conversation block is rendered in a `SECTION` element. This element provides context for screen reader users as it becomes a page landmark within the screen reader, this means blind and partially sighted users can orientate themselves and navigate around the page. 

The accessibility tree in Chrome shows this hierarchy correctly. One `SECTION` element which represents the chatbot window containing all conversations and several nested `SECTION` elements which are the individual conversations. 

However, if we open the screen reader NVDA and navigate to the landmarks tab we see one `SECTION` element with all the text from every conversation. Semantically we've chosen the correct element to provide meaning but by not providing a name for each element NVDA isn’t able to display it correctly. It's difficult to read and unhelpful for a screen reader user trying to understand the chatbot and the hierarchy of the messages.

Let's improve upon this and add the `ARIA-LABEL` attribute onto every `SECTION` element to provide more helpful text for screen reader users. We'll add the `ARIA-LABEL` attribute to the chatbot conversation container and then every nested section element alternating between the bot and the user and we'll then refresh the page. In the landmark view in NVDA we see each `SECTION` now has contextual text describing the:

* chatbot conversation which is the wrapper of the individual conversations, and 
* each individual conversation which alternates between the bot and user.

But it's not a unique label and it still doesn’t tell us what time the message was sent. There are several "the bot said" or "the user said" labels and it's difficult to identify individual conversations. So, jumping back into the code, we add to each message conversation the time it was received. 

In a production environment this text would be dynamically created and added but for the benefit of convenience we're hard coding it here. Refreshing the code and jumping back into the landmarks view in NVDA we see each nested `SECTION` element now has a label of who the message is from, and the time it was sent. This results in making it easier to identify the chatbot region and understand the sequence of the messages.

We explained how to use the `ARIA-LABEL` attribute to provide extra helpful text for screen reader users, and we saw how this is displayed in the NVDA screen reader and we enhanced this text to provide a timestamp indicating when the message was sent, this value was hard coded but in a production environment it would be dynamically created.

The `ARIA-LABEL` attribute provides a text description for users who may navigate the chatbot via the screen reader. In this instance it provides context for a user to navigate the chatbot hierarchy and to individual conversations.

Check the descriptions below for background information, WCAG 2 success criteria, links to the transcript and completed HTML source on GitHub and remember to like and share.
