# unit-5-9-notes

5. HTML Working with Graphics and Images

The image's URL is pasted into the source, as can be seen in the example, and then the image starts loading. We are not finished yet. Add an ALT attribute, which serves as a replacement for the image when it cannot be seen. For instance, people who are visually impaired may use a screen reader that reads the ALT text aloud to them. 

Make the ALT text interesting. Describe it as a shiny black dog appearing pensive. No need to mention that it is a photo, as it is obvious. There is no need to write a lengthy description, just focus on what it depicts. You have the option of making the ALT text funny or poetic, and if there is nothing significant to convey about the image, simply leave the ALT text blank.

In the example, there is this header where the company name is in a big font (h1) and their logo is an image. Now, pay attention to the ALT text labeled as B. We could describe it as a happy dog — It is basically a drawing of a cheerful dog. However, constantly hearing "happy dog, happy dog, daycare" does not improve the user experience. This is why the ALT attribute is added, which shows that ALT text was considered, but a decision was made to leave it blank. This way, it will be skipped over and not spoken aloud. If the ALT attribute is omitted altogether, there is a chance that the image file name will be read aloud, and we definitely do not want that to happen.

The browser also needs to be informed about the size of the image in pixels. In this case, the image is 400 pixels wide and 300 pixels tall. If the image is opened in a program like Photoshop, those dimensions can be verified. Include that information in the image element using the width and height attributes. The units for these numbers do not have to be specified; just the numerical values are enough. It is universally understood that the dimensions are actual pixels. 



6. HTML Working with Media


We are going to use the track element and link it to a text file to add captions to the video. This element adds functionality to the video player, allowing viewers to toggle captions on and off or switch between different subtitle options. On the web, a file format called ibvtt, which stands for web video text tracks, will be used. It is a simple text file with a vtt extension that follows a specific convention for providing information. In the file, each line of text is accompanied by a time code, indicating when it should be displayed in the video.

To display these captions on the video, insert a track element within the video element. Similar to the source element, it is one of the options the browser uses to render the video player. On the track element, use the source attribute to specify the file, the kind attribute to indicate that it contains captions, and a label attribute to display the caption option as "English" in the player. Additionally, use the source lang attribute to indicate the language and add a default attribute to make this track the default choice when captions are enabled.

Notice a captioning icon appeared. Clicking on it reveals options for turning captions off, enabling automatic captioning, or selecting English captions. The word "English" appears because of the label that was set. If a Spanish translation for example is required as a different subtitle option, another vtt file for Spanish can be created and another track element to the same video element can be added. This time, set the kind attribute to "subtitles," the source lang attribute to "es" for Spanish, and the label attribute to "Español." As a result, a second choice for subtitles appears in the list, now including Spanish subtitles.

There are a few other options for the kind attribute. For example, using "descriptions'' allows us to create a vtt file that describes the visual elements of the video. Users can choose a track that reads aloud these descriptions, making the video more accessible to those who are visually impaired. Another option is "chapters," which provide a text file listing the different sections of the video, allowing users to jump to specific parts. 

In the next section, using platforms like YouTube or Vimeo will be discussed, where you can upload caption files and provide similar functionality. Captions and subtitles are not only powerful but also often required by law. By including them, your content will be more accessible and inadvertently increase your audience base. So, add captions and watch your traffic grow!



7. HTML Content Identification

Here is a good example. There is a simple article wrapped in an article element. It has a headline and four paragraphs. When working on the CSS layout, you are required to group these paragraphs together. The goal is to add a background color only to the paragraphs, excluding everything else. To achieve this, introduce a div with a class called "boxes". By targeting this box class with CSS, the changes taking effect can be seen.

Now, imagine there is a particular phrase in the middle of the text that needs to be specifically targeted for some reason e.g. it is written in Spanish, and we want to change its language attribute to reflect that. To accomplish this, use the inline element span to mark the desired phrase. Both div and span can make use of various global attributes like class, id, lang, and aria roles.

Div and span come in handy when there is not another suitable element to use, acting as a last resort option. Remember, use them wisely.

Before 2010, when HTML5 came along with its helpful semantic elements, we relied heavily on divs for all sorts of purposes. Divs were used to create sections, sidebars, and everything in between. People still tend to use divs and spans excessively in HTML, without much else. This course aims to emphasize the value of semantic HTML.

Technically you can get away with using divs and spans for everything. Some developers even put their titles in divs and make spans pretend to be buttons. The HTML will not give an error, and the browser will still try its best to do its job and parse the page. But to be honest, it is not good practice. It adversely affects many users. We strongly urge you to avoid using divs and spans for every little thing. Opt for the appropriate HTML element that serves the purpose. 

Now, with that being said, there are times when a generic element is needed. Div is a block-level element, while span is an inline element. They essentially do nothing until CSS or Javascript is applied to them.




 8. HTML Integration

 9. Let's start putting the pieces together. This will give you a sense of how we are going to assemble web pages out of hundreds of nested elements, each conveying meaning and each playing off of the other, adding up to the whole. 

When you are unsure what the best way to mark up a page is, travel around the web, find similar sites, and use developer tools to see how others have decided to use HTML elements in their content. The exact way to combine these HTML elements differs with every webpage created. It is hard to be sure it is done correctly because the right way to do it always depends on what the content is, and what the page is for. 

In fact, usually, there are several good ways to do it, and none of them are necessarily right or better. There is a bit of an art to structuring HTML. There is a lot of creative freedom here. We are, after all, trying to represent human communication in code, and while code may want to be correct and perfect, human connection is not always.

Inside the head of a webpage, you put important information that the browser needs to know about the website. Remember the section on specifying the character set? Well, that is where it comes in. 

The character set is not something you want your users to see, it is intended for the browser. To convey this, use the meta element. Ensure that meta elements are only placed inside the head as they provide metadata about the page. For example, to define the character set, use the character set attribute and set it to UTF-8. Before delving into other things that can be conveyed through meta tags, let's start with something that is required on every webpage: the title element. Just to clarify, this title element is not something that appears as visible content.





9. HTML Working with Forms and Interactive Elements
    

Form fields have been an essential part of the web for a long time. They are used for various tasks like logging into websites, making purchases, conducting searches, and adding content. 

It is important to use semantic form elements in HTML instead of divs and spans because it allows us to leverage the built-in power of the browser. This way, we avoid wasting time and effort trying to recreate functionalities that already exist in the browser. Moreover, by using HTML form elements, we ensure that forms will be compatible with all devices and input/output hardware, even those we may not be familiar with. 

To start off, create a simple form to sign up for an email newsletter. We need two fields for this: 

The person's name. 
Their email address.

To create a form, we start with the form element, which informs the browser about the presence of a form using opening and closing tags. In the newsletter signup form, there will be two fields: name and email. These field names can be turned into labels using the label element. 

Use the input element to provide places for users to input their name and email. Unlike other elements, the input element does not have a closing tag due to its older structure. It acts as a marker for the browser to bring in functionality and place it there. This is where the form's magic happens. 

Now, a button is needed for users to submit the form. Use the button element for this. The text on the button can be customized to whatever is required. Although the form looks good visually, it currently lacks functionality. To make it work, we need to connect it to a backend. We can add an action and method attribute to make a demo work, although using the "get" method is not secure and is not recommended for real websites.

Once set up, land on the response page, but the data that was entered does not appear. This is because the input fields need a "name" attribute to report the data. Add "name=name" to the first input element and "name=email" to the second. The name attribute can be customized as desired. After making these changes, the form works successfully, but only if you interact with it using a screen and a mouse. 

To make it accessible to everyone, we need to address the issue of the label and input elements not being connected. There are two options to achieve this. 

Add a "for" attribute to the label that matches the "id" attribute of the input. 
Wrap the input with the label. 
Both methods work, and it is a matter of choosing the desired markup structure. You can test the connection by clicking on the label and ensuring that the focus jumps to the corresponding input. This is crucial for accessibility, as many people rely on this connection. Clicking on the label is a quick way to verify its functionality. 

These are the basics of building an HTML form. Next, we will explore how to utilize additional browser features to enhance the user experience.










