# Support for dynamic content #
[This video](https://youtu.be/A6nhXP-RHwE) shows you how to support dynamic content using an `aria-live` attribute and how to prioritise the announcing of messages using the values of **polite** or **assertive**. 

Screen reader users navigate onscreen content audibly. If parts of the screen change visually, we need to ensure the change is identifiable programmatically as well. By making a change programmatically identifiable the screen reader monitors what has changed and announces the change audibly.

## Live demo ##
[Support for dynamic content](https://canaxess.github.io/canaxess-teaches/chatbot-accessibility-fundamentals/3-support-dynamic-content/)

## NVDA<sup>i</sup> and User Agent compatibility ##

&nbsp;        | Internet Explorer 11 | Edge | Chrome 72 | FireFox Quantum 65
:-------------: |:-------------:| :-----:| :-----:| :-----:
`aria-live`    | YES | NO* | YES | YES

*Edge only announces the container title 'chatbot-conversation' not individual messages

<sup>i</sup>NVDA version 2018.2.1
