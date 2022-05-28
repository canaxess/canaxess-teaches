# How to decide if an image needs ALT text

ALT text for images is the one simple accessibility improvement that anyone can do right? Not quite, this bit of often repeated advice whilst helpful is open to wild interpretation.

To conform against WCAG, all images need to have a method to describe the image for people who can't see it. Ordinarily this is by using the ALT attribute. Think of it as a bit like meta data for the image element.

Image elements which have an ALT attribute are then able to be described by the screen reader using the text within the ALT attribute. Where this advice becomes misplaced is applying it to all image elements whether they need it or not. 

When ALT text is applied to images which need to be described and decorative images which don’t, the end result is that all images now have ALT text.

A user navigating with a screen reader will hear a description of images which need to be described and understood which is great along, with completely unnecessary descriptions of decorative images. Every image does not need ALT text.

Only provide ALT text to images which need describing. If there is a decorative image of lines, shapes or even patterns which don't provide any information to the user use null ALT text. This then causes the screen reader to ignore the image.

When providing ALT text to images which need explaining, use the same language as if you were describing it to someone. For example, if there was an image of a boat you could use alt text of "boat", which whilst technically correct in the literal sense it doesn’t provide anything really that useful to the user. 

Why is the image important, what is it showing? You don’t necessarily need to write a lot of text, but just enough that it explains the image, make the text succinct.

All images need an ALT attribute but only some images need ALT text. If the image needs to be understood provide ALT text which succinctly describes what's in the image. If, however the image is decorative, set the ALT text to empty.

If you've found the video useful click the thumbs up and leave a comment below and be sure to click subscribe to be notified when new accessibility videos are available.
