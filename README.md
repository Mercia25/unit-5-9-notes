# unit-5-9-notes

5. HTML Working with Graphics and Images

The image's URL is pasted into the source, as can be seen in the example, and then the image starts loading. We are not finished yet. Add an ALT attribute, which serves as a replacement for the image when it cannot be seen. For instance, people who are visually impaired may use a screen reader that reads the ALT text aloud to them. 

Make the ALT text interesting. Describe it as a shiny black dog appearing pensive. No need to mention that it is a photo, as it is obvious. There is no need to write a lengthy description, just focus on what it depicts. You have the option of making the ALT text funny or poetic, and if there is nothing significant to convey about the image, simply leave the ALT text blank.

In the example, there is this header where the company name is in a big font (h1) and their logo is an image. Now, pay attention to the ALT text labeled as B. We could describe it as a happy dog — It is basically a drawing of a cheerful dog. However, constantly hearing "happy dog, happy dog, daycare" does not improve the user experience. This is why the ALT attribute is added, which shows that ALT text was considered, but a decision was made to leave it blank. This way, it will be skipped over and not spoken aloud. If the ALT attribute is omitted altogether, there is a chance that the image file name will be read aloud, and we definitely do not want that to happen.

The browser also needs to be informed about the size of the image in pixels. In this case, the image is 400 pixels wide and 300 pixels tall. If the image is opened in a program like Photoshop, those dimensions can be verified. Include that information in the image element using the width and height attributes. The units for these numbers do not have to be specified; just the numerical values are enough. It is universally understood that the dimensions are actual pixels. 
