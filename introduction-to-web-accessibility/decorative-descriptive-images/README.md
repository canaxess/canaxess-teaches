# Transcript #

For vision impaired users every image needs to provide a text alternative, which is a way for the user to understand what the image is describing. But if the image is decorative, this description is not required, in both instances though the ALT attribute is required.

In this lecture I'll explain the ALT attribute, a way to describe descriptive images and a way to make a screen reader ignore decorative images. The often-repeated phrase all images require ALT text is only partially correct, some images require ALT text and some don’t.

At the end of this lecture you'll learn how a visually impaired user can understand an image when they can't see it. Understand when to apply succinct ALT text to describe a descriptive image and when to use blank ALT text to ignore a decorative image. 

As I've discussed previously a visually impaired user may use a screen reader to navigate a webpage. The screen reader uses the HTML semantic structure to make sense of the page and describe its content audibly, so all the appropriate options for elements are used to give the screen reader the best chance of conveying content correctly.

The first rule for adding any images via the IMG element is making sure every image has an ALT attribute. When an image is missing an ALT attribute a text description (if required) can't be provided.

When images are encountered by a screen reader it uses the value of the ALT attribute to provide a text description for the user. If an image has no ALT attribute the screen reader will announce "image". So, the user is aware an image is there, it may be relevant it may not, but they are uncertain. 

The ALT attribute is the way to provide a text description or conversely to indicate to the screen reader that the image serves no purpose other than being decorative and it can be ignored.

For an image of a boat appropriate ALT text could be "boat" as after all the image is of a boat. Whilst technically correct, the image is of a boat adding such succinct ALT text really isn't in the spirit of web accessibility. 

What is the image describing, why is it relevant, what does it show? If you were describing the boat to a friend, you would say more than the literal description, apply that same richness when adding ALT text why is the image relevant, it may be a boat sailing under Sydney Harbour bridge on a sunny morning, or "A replica sailing ship leaving Sydney Harbour".

Avoid overly verbose descriptions as well, ALT text of a short sentence is probably the upper limit when describing most images. Use enough of a description to convey what the image is showing.

The second rule for adding images is descriptive images require ALT text, decorative images don’t. Unless an image is crucial for a user to understand the content of the page, set the ALT attribute to null.

When an image is decorative and doesn’t require an explanation use blank ALT text. The image still has the ALT attribute, but it has no value. So, don’t have ALT text with the value of "blank" or "null" or have a blank space, the ALT attribute value is nothing except two double quotes next to each other. Using null ALT text means the screen reader will ignore the image, this is particularly useful if you have spacer images, or images which are decorative.

Providing ALT attributes for images satisfies the HTML specific technique H37: Using alt attributes on img elements and the general technique G82: Providing a text alternative that identifies the purpose of the non-text content. Which means this passes 1.1.1 Non-text Content: All non-text content that is presented to the user has a text alternative that serves the equivalent purpose at level A.

I explained how a vision impaired user relies upon the ALT text of images to understand what the image depicts. The screen reader uses this ALT text to provide a text description of an image which is announced by the screen reader. If an image is decorative and can be ignored by the user, the ALT attribute value can be set to null. In both cases all images require an ALT attribute, but only some images require ALT text.

This video is from our Introduction to Web Accessibility WCAG 2.1 Udemy course. The course is designed to teach you the fundamentals of web accessibility and how to apply those techniques to websites that you create. If you're interested in finding out a little more, checkout the link in the description below as well as links to a full transcript.

If you want to stay up to date with web accessibility and to learn cutting edge techniques, consider subscribing and click the bell icon to be notified when new videos are uploaded.
