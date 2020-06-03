# Group Related Links #

Sometimes links on a page are related, they may be links in the header such as navigation or links in the footer. When a grouping mechanism is used for these links it can trigger the screen reader to announce extra information which can assist the user in understanding how the page is structured.

In this lecture I'll walk through using the list elements. I'll explain why grouping related links can be helpful for a user, ordered and unordered list elements will be used to group links and show how the screen reader responds when using the different list elements.

By the end of this lecture you'll understand the added extras that come with grouping related links together provides to the user, and also why you need to use this technique carefully, additionally you'll be able to identify which list element to use to trigger the screen reader to give out this extra information.

Screen reader users navigate websites in a non-visual way. Links which are arranged to convey meaning visually relying on a presentational effect also need to be marked up in a way to induce the screen reader to provide extra helpful information. Without this screen reader hint, the broader meaning of what these links mean and if they're related can become confusing. 

If there were several links in the header of a webpage which navigated to different sections of a site, visually they're located at the top of page, laid out close to each other and related. This is all known purely from how they look on screen. 

Screen reader users don’t always have the ability to identify visual cues and so instead rely on other information and this is where the screen reader can be leveraged to help us provide extra non-visual cues. 

The list elements ul and ol can be used to trigger the screen reader to announce the type of list, the number of items in the list and depending on the list type, whether its bulleted or numbered. 

For example, an unordered list with 3 items will trigger some screen readers to announce "list with 3 items" and then every item will trigger the screen reader to announce "bullet item a", "bullet item b", "bullet item c".

An ordered list with the same 3 items will trigger the screen reader to announce the same as before "list with 3 items" except this time the screen reader will announce every items position in the list first followed by the item "1 bullet item a" and so on.

The behaviour is dependent on the assistive technology, different screen readers and different versions of screen readers may announce the element type first followed by the elements. Using ul and ol elements to group links acts as meta data for the screen reader and provide subtle extra hints for the user to understand and interpret.

Whilst this extra grouping is helpful for the user, avoid the urge to group all page links into list elements. This is a case of using the technique carefully and applying it only when necessary. Because the screen reader announces the list type and element position it adds to the audible overhead a screen reader user has to understand and take in. The more noise a user listens to, the more fatiguing it can become.

This is where once again you need to make a judgement call. Do the collection of links require grouping into list elements. Does providing list meta data provide helpful information to the user allowing them to understand the relationship of the contained links, or is it providing unnecessary noise, only you can answer that.

Using OL and UL elements for grouping together related links satisfies the HTML specific technique H48 Using ol, ul and dl for lists or groups of links which means this has passed success criterion 1.3.1 Info and Relationships: Information, structure, and relationships conveyed through presentation can be programmatically determined or are available in text at level A.

I explained how related links can be grouped together using the list elements UL for unordered lists and OL for ordered lists and how by using these elements extra meta data is provided for free by the screen reader or assistive technology to inform the user about the list. I also emphasised that whilst it’s a convenient way to group related links together care should be taken to not overuse the technique due to the extra noise of meta data used to inform the user about the links.

This video is from our Introduction to Web Accessibility WCAG 2.1 Udemy course. The course is designed to teach you the fundamentals of web accessibility and how to apply those techniques to websites that you create. If you're interested in finding out a little more, checkout the link in the description below as well as links to a full transcript.

If you want to stay up to date with web accessibility and to learn cutting edge techniques, consider subscribing and click the bell icon to be notified when new videos are uploaded.
