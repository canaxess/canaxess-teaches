# Transcript
Add the `FOR` attribute to the label element, and add the `ID` attribute to the input element. Now enter a value for the `ID` attribute of the input control and ensure this is the same value for the `FOR` attribute on the label element. 

A programmatic relationships between the form and label element has now been established. Refresh in the browser and click the label, the focus moves to the input element identifying a programmatic relationship between the label and form element exists. 

Confirm this by pressing F12 to open the developer toolbar, highlight the input control using the inspector tool and select the accessibility tab. Identify the name for the input control is from the label element.

In review to create a programmatic link between an input control and a label element use the `FOR` attribute on the label element and the `ID` attribute on the input control and ensure the value in both attributes is the same. Test the relationship is correctly set by clicking on the visible label where focus will move to the input control and confirm in the accessibility tab in the developer tools where the name of the component is obtained from the label element.
