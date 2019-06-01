# AZURE Proof of Concept
In the last video we explained rich cards and how several bot frameworks can return a combination of images, form controls and text in addition to plain text.

This video is the last in the series putting all of the techniques from the previous four videos together. We'll be using the fenton UI code to create a proof of concept chatbot running on the Azure platform which demonstrates all of the accessibility principles we've covered.

If you haven’t done so already make sure you have a Microsoft AZURE account setup, and you've added the Web App Bot resource.

We won't be going through the process of configuring the bot on AZURE, but links are provided in the descriptions which take you through the necessary steps. For convenience we'll be using the default echo bot which repeats back whatever is typed but these steps can also be followed using the rich cards chatbot sample project.

Clone or download a copy of the fenton UI from the CANAXESS GitHub. Open the `index.html` file and this is where you'll be adding the values of your own bot from Azure to the property fields for the bot object. We'll be adding **bot id**, and **bot secret**.

Within Azure, navigate to the **Channels** submenu on your web app bot. Navigate to **Add a featured channel** and click a **Directline channel**. Configuring a DirectLine channel allows communication with the bot outside of the provided Microsoft webchat control. 

Whilst we can add the webchat control to our pages easily and with minimal configuration, the control isn’t accessible and is rendered in an iFrame. By using DirectLine it allows us to create a customised UI where we can add in accessibility features easier.

**Add a new site** and click **Done**. Under the textfield labelled Secret keys click **Show**. Copy this value and place between the quotes in the `bot.secret` property in `index.html`. Follow this by clicking **Done**, we now have enabled a Directline channel for our bot.

In `index.html` add your bot name from AZURE to the property `bot.id`, you don’t need to worry about the other properties userId, botname, email, organisation and site. These are provided to demonstrate several other ways which the bot can be customised. And that's its, all the configuration has been completed.

To test out the bot load `index.html` in Chrome, click **Start**, enter any message in the textfield and click **Send**. After a slight pause the bot will echo back all what you type. 

If you view the page source, you'll see every message is contained in a `section` element which we covered in video 1 navigating the conversation. `aria-label` is used on each of these elements to provide a label for screen readers covered in video 2 identifying the conversation, and lastly, we use an aria-live polite region to audibly announce all new content covered in video 3 support for dynamic content.

Additionally, the code supports the display of richcards covered in video 4 understand the range of response. The chatbot configured earlier is a simple echo bot which doesn’t return messages in the rich card format. This can easily be changed to communicate with a rich card enabled bot, and the code has extra libraries to handle the click events of buttons on rich cards through JQuery, and render HTML through the use of the Showdown library.

We created an echo bot on the AZURE platform and enabled the Directline channel to allow communication to the bot via a custom UI. The fenton UI was downloaded from the CANAXESS GitHub repository and two properties in the HTML code were altered to allow communication to happen, these were adding a bot ID and the secret key from the Azure bot.

We also demonstrated in the live code all of the principles covered in the previous four videos. Check the descriptions below for background information, links to the transcript and remember to like and share.
