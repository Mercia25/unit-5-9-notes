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










