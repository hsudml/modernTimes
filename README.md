# AR Madness!!! :sparkles: &#x1F984; :zap: :wolf: :boom:

## Welcome to Glitch

Click _Remix_ to make a new version of this project that you can edit and call your very own! Share with friends and add collaborators! Glitch is a great place to work and learn with others. Learn more about using Glitch through their [YouTube channel](https://www.youtube.com/channel/UCEXPMR0aWP1RuwXyOy4iv0g). 

Click _Show Live_ in the header to see your app live. Updates to your code will instantly deploy and update live. When using [AR.js](https://github.com/jeromeetienne/AR.js/blob/master/README.md) (like this project), you will notice that you get strange error messages when you view the live site. This is due to the fact that we are accessing the device's camera. On computers with no camera, the message will basically say that the page won't work. On computers with cameras, you will need to allow the site to access your camera. On phones and other mobile devices, you may see the no camera message unless you type in the full URL, with the https:// header. To view the live version of this project on your phone you will need to type in the full URL: 

```https://hsulibrary-ar-beginner.glitch.me```

**Glitch** is the friendly community where you'll build the app of your dreams. Glitch lets you instantly create, remix, edit, and host an app, bot or site, and you can invite collaborators or helpers to simultaneously edit code with you.

Find out more [about Glitch](https://glitch.com/about).

Glitch is made by [Fog Creek](https://fogcreek.com/)

-------------
-------------

## Tutorial

If you are interested in remixing this but don't know where to start - you're here! This is a beginner [A-frame tutorial project](https://hsulibrary-vr-beginner.glitch.me/) that you can start remixing following the instructions below. 

If you're not already in Glitch and are not sure how to proceed, the easiest way to get into this project is to remix the [Glitch version](https://hsulibrary-vr-beginner.glitch.me/) (go to this link and click on the fish in the upper right-hand corner and select 'Remix on Glitch.' It's free and you don't need to create an account - though all anonymous projects will get deleted in 5 days).

## Tutorial License

![CC BY Logo](https://cdn.glitch.com/9987c5bc-7eaf-48cb-9912-5a51cfeb553c%2Fccby.png?1555086175886)
This tutorial is CC BY Tim Miller, 2019

-------------------
## Your AR Project :art: :city_sunrise: :rainbow:


### ← README.md

That's this file, where you can tell people what your cool website does and how you built it. You're reading this site's README.md file now. You can edit it by clicking on the 'Markdown' button with the eyeball above. 

### ← index.html

Where you'll write the content of your website. We will be doing everything in here for this project. More details below.

### ← style.css

CSS files add styling rules to your content. For this project, we will ignore this file. The only thing it is doing is hiding a diagnostic tool for debugging. 

### ← assets

Drag in `assets`, like images or music, to add them to your project. For this project, we have a model for our butterfly and I've also included a [PDF for the Hiro marker](https://cdn.glitch.com/9987c5bc-7eaf-48cb-9912-5a51cfeb553c%2FhiroMarker.pdf?1551216651589) so you can download and print it out. If you don't have access to a printer, you can display the image on a computer screen and view it through your device. You will need to avoid glare. 

-------------------

## Resources :hammer: :books: :flashlight: 

All of the following resources are free and provide more information and help with this project.

### Using AR.js and Aframe 

This tutorial is built on the work of the folks below. Please take a look at their sites if you have questions or want to learn more.

[Building an Augmented Reality Treasure Hunt with A-Frame and AR.js](https://www.womenwhocode.com/blog/building-an-augmented-reality-treasure-hunt-with-a-frame-and-ar-js) - Women Who Code

[Creating Augmented Reality with AR.js and A-Frame](https://aframe.io/blog/arjs/) - Aframe Blog

[Marker Generator](https://jeromeetienne.github.io/AR.js/three.js/examples/marker-training/examples/generator.html) - Jerome Etienne

[How To Create your Own Marker](https://medium.com/arjs/how-to-create-your-own-marker-44becbec1105) - Alexandra Etienne

[https://aframe.io/docs/0.8.0/introduction/models.html##sidebar](3D Models Aframe Docs) - 

Another blog post with AR instructions: [Augmented Reality in 10 Lines of HTML](https://medium.com/arjs/augmented-reality-in-10-lines-of-html-4e193ea9fdbf) - Alexandra Etienne

Places to find free and openly licensed models: 
+ [Sketchfab](https://sketchfab.com/)
+ [Google Poly](https://poly.google.com/)
+ Find more on the Aframe doc page for [3D Models](https://aframe.io/docs/0.9.0/introduction/models.html#sidebar)

### Aframe

_Note: Working with AR in Aframe is fairly different from VR, so if you want to learn VR first, there are quite a few things that don't apply to AR. It's not necessarily a bad idea to start with VR first, but it's not necessary, either._

[Aframe School](https://aframe.io/aframe-school/#/) is an interactive presentation about using Aframe and Glitch. It's a perfect precursor to this project if you feel like this is too much. 

[WebVR Starter Kit](https://www.youtube.com/watch?v=zzUHF85gZno&list=PLkkL3Pim_xkUDkK1TkSFHL1QO1UxCOXjt) this YouTube playlist from the folks at Glitch will give you a quick overview of creating a VR project. 

### Learn HTML

The [Dash tutorial by General Assembly](https://dash.generalassemb.ly/) is a great beginner tutorial to get you started with HTML, CSS and JavaScript (JS). These three are the main languages that are used to create websites and if you complete these tutorials you'll be more than prepared for this project and using Aframe. 

The [Getting started with HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started) tutorial from Mozilla MDN Web Docs, is a text-based tutorial that serves as a great introduction as well.

The [Mozilla MDN Web Docs](https://developer.mozilla.org/en-US/) are great for finding answers to your HTML questions. If you Google something like "img element" you can look for the results from MDN. 



-------------------
-------------------

# :boom: Tutorial :rocket:
-------------------

## Aframe

[Aframe](https://aframe.io/) is a framework for creating VR and AR on the web. It is based on WebVR and Three.js (and other cool tools) but simplifies them so that you can use basic HTML to create your project. You don't need to know HTML to follow this tutorial, but you will need to know some basics (which we will cover next). 

Aframe is used to create VR projects and you will no shortage of tutorials and remixable projects to explore VR with Aframe. Today, though, we will be looking at AR. This is a little more complicated because testing and trouble shooting is a bit more difficult. To implement AR with Aframe, we will be using another library that makes it easier- [AR.js](https://github.com/jeromeetienne/AR.js/blob/master/README.md), by Jerome Etienne. 

When using AR.js (like this project), you will notice that you get strange error messages when you view the live site. This is due to the fact that we need to access the device's camera. On computers with no camera, the message will basically say that the page won't work. On computers with cameras, you will need to allow the site to access your camera. On phones and other mobile devices, you may see the "no camera" message unless you type in the full URL, with the https:// header. **To view the live version of this project on your phone you will need to type in the full URL:**

```https://hsulibrary-ar-beginner.glitch.me```

## HTML

All websites are built using [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML). It is the code that adds information to a site. A site is broken down into [HTML elements](https://developer.mozilla.org/en-US/docs/Web/HTML/Element). Elements are indicated by angle brackets, ```<``` and ```>```. For example, when you write out a paragraph, it is a ```<p>``` element. The ```<p>``` element has an opening tag and a closing tag, like so: 

```<p>This is a paragraph.</p>```

The ```<p>``` is the opening tag and starts the paragraph. The ```</p>``` is the closing tag and ends the paragraph. All of the text in between those tags is the paragraph that shows up on your visitors' screens.

Images are also elements but since there is no text, they are constructed a little different, with no closing tag (the / at the end of the ```<img>``` tag serves to close it): 

```<img src="photo.png" alt="Photograph of a butterfly" />```

Unlike the ```<p>``` element above, this one has a bit more info in between the angle brackets. These are called [attributes](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started#Attributes) and can set different characteristics of the element: 

```src="photo.png"```

Indicates the source (src) for the photo. It's really just the spot where the photo is stored- much like the file location on your computer. The name of the file is 'photo' and it's a .png file. In this case, the _attribute name_ is src and the _attribute value_ is photo.png. Attribute values are almost always enclosed in quotation marks, with a notable exception being boolean values (true or false). In this case, the attribute value is the file name, which is enclosed in quotation marks. The source is set to point to the photo because of the equal sign that connects the two (with no spaces). 

```alt="Photograph of a butterfly"```

Indicates the alternative text that would show up on the screen if there was a problem and the image was unable to load. This is also used by people who have visual impairments and use a screen reader to audibly read out the content of the webpage for them. 

With this project we will be using a lot of elements and attributes. 

Two major elements for every webpage are the ```<head>``` and ```<body>``` elements. The ```<head>``` is where we link to other code and tell the browser how to display the page. The ```<script>``` element on line 9 is where we grab the Aframe code to run the project. The ```<title>``` element on line 4 is simply the name of our project (which appears in the tab on your browser). 

The ```<body>``` is where we put all of the content you will see. In this case, it is our Aframe scene. 

-----------------
### &#x1F634; tl;dr

HTML elements are how we add information to a web page. Elements that contain text have opening and closing tags like so: 

```<p>This is a paragraph.</p>```

Other elements can be self-closing: 

```<img src="photo.png" alt="Photograph of a butterfly" />```

In the example above, there are two attributes in the ```<img>``` element. ```src``` and ```alt``` are what we call _attribute names_. The file name and alternative text are what we call _attribute values_. Values should be enclosed in quotation marks. An equal sign with no spaces connects the name and value.

-----------------

## Basic Aframe Scene

The Aframe elements all start with a- like ```<a-scene>``` and ```<a-entity>```. Inside our ```<body>``` element we have the ```<a-scene>``` element, which is where all of our Aframe project resides. For this project, we also have an attribute to declare that we are going to use arjs, so want access to the device's webcam. Notice that there is no value set for the arjs attribute. Attributes don't always have values.

The ```<a-scene>``` element is quite big and has many other elements nested inside it. The opening tag is on line 14 and the closing tag is on line 38. More complicated projects may have hundreds of lines of code inside the ```<a-scene>``` element. Inside our scene we have assets, entities, and a marker. All of these show up as elements. 

### Assets :sound: :musical_score: &#x1F39E; &#x1F58C;

[Assets](https://aframe.io/docs/0.9.0/core/asset-management-system.html#sidebar) are the content we will be using. AR projects may have images, videos, 3D models, or other content that displays in the scene. In this case we have a butterfly model. To load the butterfly model into our assets, we add an element within the ```<a-assets>``` element, as an ```<a-asset-item>```. 

If we wanted to add other types of content, we can use the following elements to load different types of asset items: 
+ ```<audio>``` - Sound files
+ ```<img>``` - Image textures
+ ```<video>``` - Video textures

For now, we are just loading the butterfly model and the code for the model is: 

```<a-asset-item id="butterfly" src="https://cdn.glitch.com/c3ad0a0f-3e2f-4c85-ad9b-78b04bb6c512%2Fbutterfly.gltf?1550798193212"></a-asset-item>```

#### A-asset attributes

The ```id``` attribute will be how we refer to the model when we want to use it later in our scene. The ```src``` is just like the with the ```img``` example above- it's where the model is saved on our server. To save things like this to your Glitch project's server, you can upload them (drag and drop) to the 'assets' box on the left above the dark blue link to this README.md file. Click on that link to see the model files and/or upload your own.

![Screenshot of assets folder link location](https://cdn.glitch.com/9987c5bc-7eaf-48cb-9912-5a51cfeb553c%2FassetsMenu.png?1552078808974 "File Menu: Assets")

Go ahead and click on the assets link to view the assets for this project. You will see a big collection of all of the images and models that appear in the entire project, including the image of the assets link that you see displayed above in this README.md file. 

### Models :carousel_horse: :airplane: :car:

Note in the assets folder that the ```butterfly.gltf```, ```butterfly.bin```, and ```butterflyTxt.png``` files. These make up our butterfly model. This model is in the gltf format, which is the preferred format for Aframe ([learn why])(https://aframe.io/docs/0.9.0/components/gltf-model.html#why-use-gltf). 

The .gltf format works well and is fairly easy to implement (with one exception, which we'll cover below). You can see in the index.html file that the ```<a-asset-item>``` with the 'butterfly' id is the only asset we have listed (line 18). It points to the .gltf file: 

```
      <a-assets>
        <a-asset-item id="butterfly" src="https://cdn.glitch.com/c3ad0a0f-3e2f-4c85-ad9b-78b04bb6c512%2Fbutterfly.gltf?1550798193212"></a-asset-item>
      </a-assets>
```

And then later in our ```<a-scene>``` we will place that model as its own entity so that it will be displayed to our viewers (more on that later). The trick here is that we don't load the .bin or .png files into our ```<a-assets>``` element, but we need to link them somehow. We know that all three files make up our model and we need to tell the browser that as well. In Aframe, this is done by modifying the .gltf file itself before we upload it to Glitch. You can try uploading your own .gltf model and follow the instructions below or just read along. 

---------------

Places to find free and openly licensed models: 
+ [Sketchfab](https://sketchfab.com/)
+ [Google Poly](https://poly.google.com/)
+ Find more on the Aframe doc page for [3D Models](https://aframe.io/docs/0.9.0/introduction/models.html#sidebar)

---------------

#### GLTF Models

The .gltf file internally points to the other peripheral files that are needed to render the model. With our butterfly, that is two files: a .bin file and a .png file. To modify the .gltf file to point to those two files, you should first upload the .bin and .png files to your Glitch assets. 

_Note: if you are uploading a different .gltf model and there are more (or fewer) files, just be sure to upload any file(s) aside from the .gltf file -- that comes later._

Now that the files are uploaded to Glitch, open the .gltf file in a text editor (I like [Atom](https://atom.io/) but [Notepad++](https://notepad-plus-plus.org/) is also a favorite if you're using Windows). In this file, somewhere about three quarters of the way down, you will see the spots where we will need to add the URLs to your new Glitch asset(s). 

A bit about the .gltf file: 
+ This may be a confusing step for you non-coders. Don't panic. 
+ You can simply search (ctrl+f) for the word "uri" to locate the spots you need to modify. 
+ If you want to know more, a [.gltf](https://en.wikipedia.org/wiki/GlTF) file is basically a set of JavaScript objects in [JSON format](https://en.wikipedia.org/wiki/JSON), each of which has a name and some data inside it (similar to HTML elements). We are looking for the ```"buffers"``` and ```"images"``` objects. One of the bits of data within those is the ```"uri"``` which is what we need to change. 

Once you've found the ```"uri"``` location(s), you will need to replace the file path that is listed and update it with the Glitch URLs to your .bin and other files. Simply copy and paste those URLs (in the .gltf file, they will need to be enclosed in double quotes) and save your .gltf file. 

Last step: upload your .gltf file, copy that URL, and paste it into your index.html page as the source for the ```<a-asset-item>```.

You can learn more from the Aframe docs for [gltf models](https://aframe.io/docs/0.9.0/components/gltf-model.html#sidebar).

##### OBJ files

Aframe also works quite well with .obj model formats. This format is a little more straightforward, compared to .gltf files, but we won't get into them. The .gltf basic ideas are the same, except you won't need to modify any files. You can learn more in the Aframe docs for [obj models](https://aframe.io/docs/0.9.0/components/obj-model.html#sidebar).

### :round_pushpin: Marker

The next entity in the scene is an ```<a-marker>``` element. The marker is the trigger for the AR to appear. There are many ways to start an AR animation, but this is a simple and effective one that works across devices (even on laptops and desktops with cameras, though that's pretty awkward) and is a good starting point for learning about AR. All AR requires an anchor where the scene is going to be located or centered. The marker serves as the anchor for this project. As the viewer moves her phone, the model will stay in the same place relative to the real world, not her phone -- thanks to the marker. 

One notable shortcoming of the marker method is that it only works when the entire marker is in the viewport (screen) and it has to be close enough to be read clearly by the camera. You could not, for example, have a scene where your viewer focuses on the marker and then a bee flies out and circles around so that the viewer spins around. Once they start to spin and the marker falls out of the viewport, the AR disappears. 

However, the marker is a very effective and simple way to trigger and anchor our scene, so let's get started!

#### Types of markers :triangular_flag_on_post: :crossed_flags: :checkered_flag:

For this project, the marker is set to the preset Hiro marker, which is a default you can use for getting started. You can do a search on the web for 'hiro marker' to find printable versions to play around with. This Glitch project also has a [PDF Hiro Marker](https://cdn.glitch.com/9987c5bc-7eaf-48cb-9912-5a51cfeb553c%2FhiroMarker.pdf?1551216651589) loaded that you can print out (or share the URL with friends). 

However, you can easily create your own markers following Alexandra Etienne's blog post, [How To Create your Own Marker ?](https://medium.com/arjs/how-to-create-your-own-marker-44becbec1105). The basic idea is that you upload an image that has some randomness to it (text on a black icon or assymetrical shape works quite well) and then you get an image file to print out and a .patt file to upload to your Glitch project so that the viewer's camera will recognize it. 

#### What the marker does

You will notice that within the ```<a-marker>``` element, there is an ```<a-entity>``` element for the gltf model, which is how we make the butterfly appear in the scene. 

```
      <a-marker preset="hiro">
        <a-entity gltf-model="#butterfly"
                  position="0 0 0"
                  scale="0.05 0.05 0.05"
                  rotation="0 180 0"
                  animation="property: scale; to: 0.025 0.05 0.05; dir: alternate; dur: 2000; loop: true;">
        </a-entity>
      </a-marker>
```

Since the butterfly is nested inside the marker, its position will be relative to the marker. Hence, even when the camera moves, the butterfly stays in place relative to the marker. Since it is nested in the marker, it also doesn't show up until the marker is recognized. If the marker is not fully inside the camera viewport, the butterfly will not appear. This is a limitation, but also can be useful, because you can have multiple markers within one project, each with its own scene inside that will be visible when its marker is in view. This could be a good way to create a virtual tour that is entirely self-paced. 

#### Make Your Own Marker

This is completely optional, and is a good idea to tackle after you've gotten everything else down. 

* Create a design in a square template
    * Feel free to use this [Google Slides Template](https://docs.google.com/presentation/d/1jGfpMYnhERaGJnKwJQ9On6EZ2xuRxAG7qUlGPUc5Qjc/edit?usp=sharing) if you have a Google account. But any image editor will work. 
    * Black and white designs that are asymmetrical are best. This could be a simple icon or some large text.
* Upload this to the [AR.js Marker Generator](https://jeromeetienne.github.io/AR.js/three.js/examples/marker-training/examples/generator.html) by Jerome Etienne
* Download the .patt file and the printable pdf
* Upload your .patt file to your Glitch assets
* Copy that URL and paste it into your marker: 

```
<a-marker type="pattern" url="https://cdn.glitch.com/theurltoyourpatternfile.patt">
  <!-- All your cool stuffs that appear in your AR scene -->
</a-marker>
```
* Print out your pdf and look at it through your phone!

### :statue_of_liberty: Model attributes

The ```<a-entity>``` element nested in the marker is how we call up the butterfly model. There are attributes for the element that declare (in order): 
+ it as a gltf model
+ its position
+ its size (scale)
+ its rotation
+ the animation to make the butterfly flap its wings

#### gltf-model
The ```gltf-model="#butterfly"``` attribute simply points to the ```<a-asset-item>``` above, which has its id set to: ```id="butterfly"```. In HTML, a hash mark (#) is a reference to an id, so ```#butterfly``` translates to "the asset with the id set to 'butterfly.'"

#### :dart: position
The position, as already mentioned, is relative to the marker. A position of 0 0 0 is centered on the x-, y-, and z-axes over the marker. Positions must contain all three axes, each separated by a space. Otherwise, you will get an error that may prevent your model from rendering. 

In some cases, it may be good to have some models up above the marker, which means it would need to be positioned higher on the y-axis, such as: 0 1 0. Setting the y value to a negative would mean that it is below the marker, and won't show up. 

If you look at the marker oriented right-side up, you can think of the x-axis as being East-West and the z-axis as being North-South, like on a map. A negative x value would move the model to the West and a postive toward the East. A negative z value would move the model toward to South and a positive toward the North.

_Note: all objects are set to a position of 0 0 0 by default, so this isn't necessary._

#### :whale: scale
The scale is also specified using the three axes. To make the butterfly larger or smaller but still maintain the same proportions, you need to set all three to be the same. You can play with the options to see what happens when you change one at a time. 

One very important thing to keep in mind is that the scale of the original may be very large or small, in comparison to the project scene. Many models need to be scaled much, much smaller to be visible. The butterfly model is set to 0.05 0.05 0.05 -- far smaller than the original. 

#### :ferris_wheel: rotation
Yet again, rotation is set using all three axes. Rotation is set around the axis. You can visualize a line going through the model as the axis and the model rotating as if it were attached to the line, kind of like a lolipop or kebab skewer. A merry-go-round is rotating on the y-axis. The wheels of a bicycle heading straight toward you are rotating on the x-axis. If you are watching that bicycle from the side, the wheels are rotating on the z-axis. These examples are all relative to you as you stand looking at the objects. In VR and AR, you need to think about how the object rotates, irrespective of the camera. If you look at the marker upside-down, the butterfly rotation will upside-down to you as well. This obviously can get confusing. For this reason, it's always best to start with a model that is rotated in the position you want before it is imported. However, this needs to be done in a 3D modeling program and isn't always possible. 

In this scene, the butterfly's rotation is set to 0 180 0. It is rotated half of a turn through the y-axis. If it were set to 0 0 0, the butterfly's head would be oriented toward the bottom of the marker. Depending on your model, you may also need to rotate it on the other axes to orient it to your preference. 

#### :mountain_bicyclist: animation

In Aframe there are two ways to include animations, but this method, using attributes, is a bit cleaner and simpler. You can add additional animations by giving them different names using double underlines like so: ```animation__1``` or ```animation__2```. The butterfly has one animation: 

```animation="property: scale; to: 0.025 0.05 0.05; dir: alternate; dur: 2000; loop: true;"```

Aframe animations, as with most digital animations, have beginning (_from_) and end (_to_) states that the object moves between. Each animation affects one property and the starting state is assumed to be the object's property setting as coded in the ```<a-entity>``` element. Animations can have many other properties, take a look at the Aframe documentation on [Animation](https://aframe.io/docs/0.9.0/components/animation.html#sidebar) to learn about other options that aren't covered here.

In this example, the property that is being animated is the scale. Therefore the beginning state is 0.05 0.05 0.05. The end state is set to 0.025 0.05 0.05, which means that it will get narrower. The direction (_dir_) is set to _alternate_, which means that it will perform the animation forward and then again backward. The default is forward. The duration (_dur_) is set to 2000 miliseconds (JavaScript uses miliseconds, so 2000 ms is equal to 2 seconds). Lastly, the animation is set to loop infinitely. The _loop_ attribute can also be set to a number if you only want the animation to happen a few times. 

If we put all of these together, we see that the butterfly gets narrower and then wider, making it appear to flap its wings. It gets narrow because the x scale is halved and it gets wider again because the direction is set to _alternate_. It keeps flapping its wings because the animation is set to loop. It flaps every 2 seconds, which give the appearance of a butterfly that is flapping its wings while resting. If we wanted to make it look like it was flying, we may try to set the duration to something shorter, so that the wings flap more quickly. Similarly, it may be good to change the scale so that the wings appear to be flapping in flight. 

To further develop the flying animation, another animation could be added that changes the butterfly's position up and down as if flitting through a sunlit meadow on a calm, sunny day. It may look something like this snippet below. Try it for yourself by copying and pasting this code on the line after your animation and before the closing angle bracket, _>_.  

```
animation__1="property: position; from: 1 2 -1.5; to: 0 0 0; dur: 4000; dir:alternate; loop:true; easing: easeInOutCubic"
```
Easing refers to the smoothness of the animation. The default is linear, which means that the animation simply moves at the same rate throughout the animation. The other options make the animation move at varying speeds throughout, creating bouncing or floating effects. The easing property is a complicated one that requires some trial and error to understand (at least for me -- it's still not entirely clear to me how those work). Take a look at the [easing options](https://aframe.io/docs/0.9.0/components/animation.html#easings) and try some out for yourself.  


To make it look like the butterfly flies in and lands on the marker to let you look at it, you may try something like this, instead: 

```animation__1="property: position; from: 2 4 -1.5; to: 0 0 0; dur: 4000; easing: easeInOutCubic"```

In this case, we don't want the animation to loop or alternate, so we just get rid of those properties.

### Working with .gltf models (some tricks)

[GLTF Viewer (Don McCurdy)](https://gltf-viewer.donmccurdy.com/)

[GLB Packer](https://glb-packer.glitch.me/)

You have two major options for getting the gltf model hosted - two options

#### GitHub

* Load into a GitHub repo and publish on [GitHub Pages](https://pages.github.com/). 
    * Then use the pages (github.io url) link for the ```scene.gltf``` file and it will reference the associated files just fine. 
    * Files other than a .bin file will often need to be added to a new file, so just create a ```/textures``` directory with a ```README.md``` file and upload those there. 
* This option is more cumbersome than the .glb route (see below) but it is more reliable (in my experience) and has the added benefit of offering a second spot to host your project if you also [sync your Glitch project to GitHub](https://hsudml.github.io/glitch/). 
    * *Warning: I have no clue how to prevent overwriting the .gltf files if you load them directly to GitHub, so you should probably load those into your Glitch project first and then sync to GitHub and then publish to GitHub Pages.*
    
#### Package into a .glb file

* Pack your model files up with the [GLB Packer](https://glb-packer.glitch.me/)
* Upload to your Glitch assets and use that url. This method seems a little less reliable than the GitHub route (see above), but it's much simpler and easier. 
  
#### :thinking: Model troubleshooting

If you loaded a model and don't see it, there are a few things to consider: 
+ position: try setting it at 0 0 0 to make sure it is centered.
+ scale: try setting it smaller and smaller, incrementally. Remember that the butterfly is 0.05 scale. If it were set to 1, it would be so big we wouldn't see it (we'd be standing under it)!.
+ texture/material: check your files to make sure there is color or an image to wrap around the model. Otherwise, it very well may be there... just invisible. I have downloaded some that have corrupted or empty files- it's not apparent until you open the file in a text editor. 
+ [Aframe docs on Troubleshooting 3D models](https://aframe.io/docs/0.9.0/introduction/models.html#troubleshooting)

_Note: There are two ways to insert a .gltf model. The ```<a-entity>``` element and the ```<a-gltf-model>``` element. If you look up more info about using 3D models and other entities in Aframe you'll see these entities referenced in different ways. In effect, they are the same, but the ```<a-entity>``` method is more distilled. The ```<a-gltf-model>``` method is a special wrapper for making it easier to learn Aframe -- under the hood, it basically just gets converted to an ```<a-entity>```._

### :movie_camera: Camera

The last entity that is included in our scene is the ```<a-entity camera>``` element. This is just the camera with which our viewers 'see' into our virtual (or in this case, augmented) world. Since we are using AR and the physical camera built into our viewer's phone, this is just a simple camera with no particular settings. You can read the Aframe documentation for more information about [cameras](https://aframe.io/docs/0.9.0/components/camera.html#sidebar).

## &#x1F44D; Overview &#x1F917; 

That's all for this project! Hopefully you now have your own AR project that you can share with friends. If you found this tutorial helpful, please share your project with the HSU Digital Media Lab and we'll post a link to it from our site(s). We love to showcase the different types of projects people make! 

Additionally, if you have any questions, suggestions, or feedback, please let us know at dml@humboldt.edu. 

### :unlock: Attribution

Feel free to remix, reuse and share this Glitch project and tutorial. 

CC BY Tim Miller, Humboldt State University Library, 2019