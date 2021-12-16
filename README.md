# ImageSteganography.
Hiding secret information in image file.
This Image Steganpgraphy project is written in HTML5, CSS and JavaScript.
It uses Steganography.js, a JavaScript library created by Peter Eigenschink to encode secret messages into an image. The resulting image is downloaded and decoded to reveal the embedded secret message.

The application calls on algorithms in steganography.js to transform the secret message into binary form that can then be concealed in the alpha channel of the supplied cover image using the functionalities in HTML5 canvas. The decode function is executed through similar algorithm to retrieve the hidden message found in the image.

**How to create the Application:**

The main process is as follows:
* A website is created using HTML, JavaScript and CSS.
* The steganography.js file is added.

```<script src="steganography.min.js"></script>```

*	Make use of global object steganography or (stegobject).

*	Make use of encode function.
* To Encode
    * Accepts a message as String. 
    * Accepts image as Image
    * HTMLImageElement or String representing the data-URL of the cover image.
    * And returns the data-URL of the image with the encoded message within it.

*  Make use of decode function.
* To Decode
    * Accepts image as Image.
    * HTMLImageElement or String representing the data-URL of the image.
    * And returns any message found within the image.

**How to use the application:**

Sender:

* Step 1: Loads the original image
* Step 2: Types in the secret message
* Step 3:  Encode the Message (Hide message in the image supplied).

Receiver: 
* Step 1: Loads the downloaded Image
* Step 2: Recovers the secret message
