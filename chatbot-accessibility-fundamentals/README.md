# Chatbot accessibility fundamentals #
The hard work creating an accessible website can be quickly undermined by using a chatbot with poor accessibility support. By learning the concepts in [these videos](https://www.youtube.com/playlist?list=PLknXoWiYr_QynKoP276ZlGV73aM8uWdq_), you’ll be able to design a bot that aligns with best practice web accessibility principles.

We'll show you how to [make the conversation history scrollable](https://www.youtube.com/watch?v=pHvMPSL_2CM&list=PLknXoWiYr_QynKoP276ZlGV73aM8uWdq_&index=2&t=0s) using the CSS property `overflow-y` and appear in the keyboard focus sequence by adding the `tabindex` attribute.

We explain how to [use the aria-label attribute to create conversation labels](https://www.youtube.com/watch?v=NYLo6cdz5_Y&list=PLknXoWiYr_QynKoP276ZlGV73aM8uWdq_&index=3&t=0s) and make them unique by adding a timestamp, and [how to announce and prioritise dynamic content](https://www.youtube.com/watch?v=A6nhXP-RHwE&list=PLknXoWiYr_QynKoP276ZlGV73aM8uWdq_&index=4&t=0s) through an aria-live region. 

We discuss several different ways the Microsoft bot framework can respond to the user through [rich card templates](https://www.youtube.com/watch?v=F5A6XC5m8gY&list=PLknXoWiYr_QynKoP276ZlGV73aM8uWdq_&index=5&t=0s), and finally put it all together by [creating an echo chatbot on the Azure platform](https://www.youtube.com/watch?v=41nwy4oAWtc) using the [fenton UI](https://github.com/canaxess/fenton) to connect to the bot. 

Each video is approximately 5 minutes in length, with full transcripts and compatibility information between browsers and screen readers in each directory.

## Chatbot taxonomy ##
* `conversation` = each single message from the bot or the user
* `conversation history` = all messages 
* `conversation window` = all messages in a container
