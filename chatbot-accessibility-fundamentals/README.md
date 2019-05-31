# Chatbot accessibility fundamentals #
The hard work creating an accessible website can be quickly undermined by using a chatbot with poor accessibility support. By learning the concepts in [these videos](https://www.youtube.com/playlist?list=PLknXoWiYr_QynKoP276ZlGV73aM8uWdq_), you’ll be able to design a bot that aligns with best practice web accessibility principles.

* [Navigating the conversation](https://www.youtube.com/watch?v=pHvMPSL_2CM&list=PLknXoWiYr_QynKoP276ZlGV73aM8uWdq_&index=2&t=0s) shows how to make the conversation history scrollable using the CSS property `overflow-y` and appear in the keyboard focus sequence by adding the attribute `tabindex`.

* [Identifying the conversation](https://www.youtube.com/watch?v=NYLo6cdz5_Y&list=PLknXoWiYr_QynKoP276ZlGV73aM8uWdq_&index=3&t=0s) shows how to create conversation labels using the `aria-label` attribute, and how each label is made unique by providing a timestamp of when the message was received.

* [Support for dynamic content](https://www.youtube.com/watch?v=A6nhXP-RHwE&list=PLknXoWiYr_QynKoP276ZlGV73aM8uWdq_&index=4&t=0s) shows how to use an aria-live region to audibly announce content and prioritise the announcing of messages using the values of polite or assertive.

* [Understand the range of responses](https://www.youtube.com/watch?v=F5A6XC5m8gY&list=PLknXoWiYr_QynKoP276ZlGV73aM8uWdq_&index=5&t=0s) explains several different ways the Microsoft bot framework can respond to the user through rich card templates, and how to add accessibility support into these range of bot responses.

* AZURE proof of concept puts all of these concepts together by creating an echo chatbot on the Azure platform, and uses the fenton UI to connect to the bot. 

Each video is approximately 5 minutes in length, with full transcripts and compatibility information between browsers and screen readers.

## Chatbot taxonomy ##
* `conversation` = each single message from the bot or the user
* `conversation history` = all messages 
* `conversation window` = all messages in a container
