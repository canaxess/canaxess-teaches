# Identifying the Conversation #
[This video](https://youtu.be/NYLo6cdz5_Y) shows you how to make the conversation identifiable using the `aria-label` attribute, and how the label is enhanced by providing a timestamp of when the message was received.

Screen reader users may use the chatbot in a non-visual way and each conversation block must be identifiable, is each message spoken by the bot or the user. Providing a label of who spoke and the time they spoke provides greater context for screen reader users.
## Live demo ##
[Identifying the conversation](https://canaxess.github.io/canaxess-teaches/chatbot-accessibility-fundamentals/2-identifying-the-conversation/)
## NVDA and User Agent compatibility ##

&nbsp;        | Internet Explorer 11 | Edge | Chrome 72 | FireFox Quantum 65
:-------------: |:-------------:| :-----:| :-----:| :-----:
`aria-label`    | NO* | YES | YES | YES

## JAWS and User Agent compatibility ##

&nbsp;        | Internet Explorer 11 | Edge | Chrome 72 | FireFox Quantum 65
:-------------: |:-------------:| :-----:| :-----:| :-----:
`aria-label`    | YES | NO | YES | NO

*`aria-label` when applied to `<section>` elements is not showing in the NVDA landmarks tab in IE11<br>

NVDA version 2018.2.1<br>
JAWS version 17.0.2729
