# Identifying the conversation #
This video shows you how to make the conversation identifiable using the `aria-label` attribute, and how the label is enhanced by providing a timestamp of when the message was received.

Screen reader users may use the chatbot in a non-visual way and each conversation block must be identifiable, is each message spoken by the bot or the user. Providing a label of who spoke and the time they spoke provides greater context for screen reader users.

## NVDA 2018.2.1 and User Agent compatibility ##

&nbsp;        | Internet Explorer 11 | Edge | Chrome 72 | FireFox Quantum 65
:-------------: |:-------------:| :-----:| :-----:| :-----:
`aria-label`    | NO* | YES | YES | YES

*`aria-label` when applied to `<section>` elements is not showing in the landmarks tab in IE11
