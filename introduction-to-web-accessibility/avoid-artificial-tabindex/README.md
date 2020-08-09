# Transcript #

Every interactive element on a webpage receives keyboard focus when the user presses the tab key. That is unless the attribute tabindex is added to elements. When the value of tabindex is artificially altered and used incorrectly it causes many headaches.

In this lecture I'll discuss the tabindex attribute, an attribute that has the power to really ruin the logical tab order of any webpage. I'll explain the implied tab ordering of interactive components, how this can be changed using tabindex and show how the values of -1 can be used to restrict keyboard focus from hidden elements and a value of 0 creates a sequential ordering sequence.

By the end of this lecture you'll understand how an incorrect tabindex value can adversely affect the keyboard navigation of a webpage. You'll be able to hide content from the keyboard tab sequence using the value -1, introduce content into the regular keyboard sequence using a value of 0 and understand nothing good ever comes from a positive tabindex value.

Every tab key press advances the screen focus one position to the right onto the next interactive element. Links and form controls have an implied focus and these elements receive screen focus in the order they're laid out on screen. 

This ordering begins at the very first interactive element and is at the top of the screen before moving across and down in a sort of Z pattern, depending how a page is structured.

The tabindex attribute on elements can be used to reorder the sequence in which interactive elements receive focus. Elements laid out on screen in no particular order receive keyboard focus in the same way they are displayed visually, and it's how users expect the behaviour to work.

The tabindex attribute accepts three possible values, -1, 0 and 1 and above. The most problematic values are 1 and above, the positive numbers bring negative outcomes.

Adding tabindex=-1 to any element removes it from the documents tab order and renders it unfocusable from the keyboard. Elements with a tabindex of -1 are displayed to the screen as expected so nothing visual changes, but when navigating via the keyboard, these elements which should be natively focusable from the keyboard are now ignored.

Using this value is useful to alter the focus sequence on elements. links in a hamburger menu where many of the navigation links are hidden in a popout menu aren't required to be focusable until the menu is shown. When the menu is shown tabindex=-1 is replaced with tabindex=0 and the items are now focusable.

Tabindex=0 will allow a component to become focusable and part of the documents natural tab sequence. Native HTML elements provide this behaviour as standard and the attribute isn't required to be added to those elements. If it is added it won't change anything to an ordinarily focusable element, but it is redundant.

This attribute and value are used when custom components are developed. Custom components constructed with DIV and SPAN elements don’t receive keyboard focus natively because the span and div elements are non-semantic and have no meaning. Adding a tabindex=0 onto the element fixes this and allows the elements to become focusable and its focusable in the order it's laid out onscreen. 

But when using regular interactive HTML elements, it's unlikely this attribute and value would need to be used as the behaviour is default.

Tabindex=1 and above, this is the problem value. Users expect the focus elements on a page to be navigable from the keyboard in a sequential order. How elements are laid out on screen should be how they receive focus. But this all changes with a tabindex value of 1 or above, this is repurposing the elements natural tabindex ordering. 

Elements with a tabindex=1 and above take precedence when the tab key is pressed, and they have an elevated priority to be focused first. Interactive elements which may be laid out visually at the very top of the page will not be tabbed to first and instead any elements with a positive tabindex will be focusable first. Confusing isn't it? 

When all links in the footer region of a page have positive tabindex values, the value elevates the focus priority of elements. 
A user tabbing through the page would tab to these links first before the focus jumps to the top of the page to focus on links which don’t have the tabindex value. This small change has resulted in the page becoming a confusing sequence of tab positions.

A positive sequential tabindex can be used on every interactive element and this will result in in a logical focus sequence if it also matches the visual order. But this behaviour is already available when regular interactive elements are used which already have an implied tabindex=0 value.

Avoid tabindex values of 1 and above, unless used very carefully it can end up making a page really difficult to understand and navigate around.

Avoiding an artificial tabindex on interactive elements satisfies the general technique G59: Placing the interactive elements in an order that follows sequences and relationships within the content and the HTML specific technique H4: Creating a logical tab order through links, form controls, and objects. Which means this passes 2.4.3 Focus Order: If a Web page can be navigated sequentially and the navigation sequences affect meaning or operation, focusable components receive focus in an order that preserves meaning and operability at level A.

I explained the tabindex attribute and how its values can have a big impact on the tab ordering sequence of a page. The only values which should be used are -1 and 0. A value of -1 removes the element from the focus sequence and a value of 0 adds the element into the natural document tab sequence. If values of 1 and above are used without understanding how it affects the page focus it can result in the focus order of the page being different to its visual order.

This video is from our Introduction to Web Accessibility WCAG 2.1 Udemy course. The course is designed to teach you the fundamentals of web accessibility and how to apply those techniques to websites that you create. If you're interested in finding out a little more, checkout the link in the description below as well as links to a full transcript.

If you want to stay up to date with web accessibility and to learn cutting edge techniques, consider subscribing and click the bell icon to be notified when new videos are uploaded.
