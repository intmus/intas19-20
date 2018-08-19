# Creating links to images and pdfs in Markdown

To link to files to download from your content pages, first add the files:

- prep the image or pdf file by giving it a standardized filename with no spaces (and easiest if all lowercase).
- make sure the file size is not too big.
- add the file to the "images" folder of the repository (`intas18-19/images/`).

To display an image on a content page, use this markdown notation:

`![alt text]({{ '/images/filename.jpg' | relative_url }})`

*Replace "alt text" with a description of the image, this will only be displayed if the image can't load or for a screen reader. Replace "filename.jpg" with the actual image filename. The curly brackets are "Liquid" code that makes sure the link to the image will be correct.*

To link to a PDF to download, use this markdown notation: 

`[title]({{ '/images/filename.pdf' | relative_url }}){:target='_blank'}`

*Replace "title" with the name of the file, this will be the text that is the link. Replace "filename.pdf" with the actual pdf filename. The funny looking "target" code at the end makes sure that the link opens in a new tab.*

# Use download button include

`{% include download.html title="Link name" filename="example.pdf" %}`

- add file to "images" folder
- paste the include code on your markdown page where you want the button to appear
- fill in the title and correct filename values
