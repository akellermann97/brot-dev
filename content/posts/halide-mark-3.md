---
title: 'Halide Mark 3 — First Impressions'
date: 2026-06-02
summary: "Halide Mark III promises \"the most beautiful photos from an iPhone.\" After running some old Raws through the new Photo Lab — iPhone, Leica M11, and all — I'm inclined to believe it. Just watch where you step, there are bugs around."
draft: false
tags: [Halide, iPhone, iPhone 15 Pro, iPhone 11 Pro, Apple, Leica, M11, Capture One, Project Indigo]
showreadingtime: true
cover:
    image: '/img/halide-v3-first-impressions/HEIF_Image-52EE2249BCC6-1.jpg'
---

The newest "camera and photo lab for iPhone" from [Lux Camera](https://www.lux.camera/halide-mark-iii/) is Halide Mark III, released May 26th, 2026. I've been using Halide since Mark I, having bought the perpetual license for Mark II, which granted me access to Mark III upon release. Mark III's update promises "The most beautiful photos that can come from an iPhone". Does it live up to the hype?

*All photos were shot on the iPhone 15 Pro in Raw unless labeled otherwise. Most were captured in Halide Mark II and in Adobe's [Project Indigo](https://research.adobe.com/articles/indigo/indigo.html), there will be comparisons of the two apps [later on.](#project-indigo-comparison)*

{{< figure src="/img/halide-v3-first-impressions/IMG_9854.jpg" class="wide">}}

## The iPhone Look

iPhones---and most mobile phones---have this over processed look on a lot of images. Excessive sharpening and compressing the dynamic range to the mids (lifting shadows, lowering highlights) leaves images flat and dull. There's no dynamism. No energy. No life!

Here's an example taken on a bright, sunny day in Switzerland:

{{< figure src="/img/halide-v3-first-impressions/IMG_8333.jpg" class="vert" caption="A Straight out of iPhone image" >}}

The trees directly in the path of the early sun, the trees behind the mountain are all *visible*, there's so much **gray**. You can see details in every part of the image. Visually, it's *boring*. There's no contrast. Apple won't let shadows fall to black. I don't fault Apple for doing this to their images. It likely stems from people wanting to see everything when they take a picture. If Apple weren't to flatten this image, they would need to make the decision to either have a highlight weighted image---which would show the tree tops nicely exposed, and the funicular in the sunlight---or bring up the shadows---Which would have the brighter parts of the image turn into a ghostly white.

Let's look at something more visually interesting as a point of comparison.

{{< figure src="/img/halide-v3-first-impressions/Christ-in-the-Storm-on-the-Sea-of-Galilee.jpg" class="vert" caption="A Straight out of iPhone image" caption="Christ in the Storm on the Sea of Galilee, 1633 Rembrandt Van Rijn " >}}

It's silly to compare an iPhone photo with a classic ([stolen!](https://en.wikipedia.org/wiki/The_Storm_on_the_Sea_of_Galilee)) Rembrandt. But as a point of comparison, here are some things that I think we can take away from this piece, and how we can learn to use some of these tricks in our photos.

**Contrast** 

That's the lightest parts of the image versus the darkest. It adds visual interest. The eye is drawn to the brightest part of the image and wanders around, discovering parts later. Reward the viewer for spending time with the piece as they find new details as they sit with the artwork.

I've since learned a term for this contrast between light and dark in art is called **chiaroscuro**---pictorial representation in terms of light and shade without regard to color---cool!

**Letting dark be dark**

Parts of the wave and even the sky don't have a ton of details for us to sink our teeth in. It gives the impression of how dark the storm is in contrast to how bright this beam of light in the middle of the crashing waves are.

Now there are probably other things I could talk about here, but I'm no art historian. I just like the piece. 

{{< figure src="/img/halide-v3-first-impressions/Adam_de_Coster_-_A_Man_Singing_by_Candlelight.jpg" caption="A Man Singing by Candlelight, by Adam de Coster, 1625–1635" class="vert" >}}

The above picture is another example of **Tenebrism** in art. A kind of "dramatic illumination" to quote Wikipedia. I really like seeing this play of light in photography.

There are other technical issues with iPhone pictures. They're often over sharpened. This can look fine on smaller screens, but the images look **crunchy** on larger screens. Little pixelated sections of light and dark closely interspersed. This can have the effect of making details look more pronounced from afar, but upon inspection it's creating this jagged noise that I think looks unappealing. And it's typically baked into the image itself, you don't get to decide if certain parts warrant it or to what degree it gets applied.

## Announcing Halide Mark III

{{< figure src="/img/halide-v3-first-impressions/HEIF_Image-EC683867E8D4-1.jpg" class="wide" >}}

{{< exhibit class="two-cl" >}}
{{< figure src="/img/halide-v3-first-impressions/IMG_9855.jpg" >}}
{{< figure src="/img/halide-v3-first-impressions/HEIF_Image-255D7168D59A-1.jpg" >}}
{{< /exhibit >}}

{{< figure src="/img/halide-v3-first-impressions/HEIF_Image-8CD193FB95E0-1.jpg" class="wide" >}}

{{< exhibit class="two-cl-vh" >}}
{{< figure src="/img/halide-v3-first-impressions/IMG_9856.jpg" >}}
{{< figure src="/img/halide-v3-first-impressions/HEIF_Image-A27B09C7F615-1.jpg" >}}
{{< /exhibit >}}

{{< exhibit class="two-cl-vh" >}}
{{< figure src="/img/halide-v3-first-impressions/IMG_9849.jpg" >}}
{{< figure src="/img/halide-v3-first-impressions/IMG_9850.jpg" >}}
{{< /exhibit >}}

{{< figure src="/img/halide-v3-first-impressions/IMG_9838.jpg" class="wide" >}}

{{< exhibit class="two-cl" >}}
{{< figure src="/img/halide-v3-first-impressions/IMG_9846.jpg" class="normal" >}}
{{< figure src="/img/halide-v3-first-impressions/IMG_9847.jpg" class="normal" >}}
{{< /exhibit >}}

{{< figure src="/img/halide-v3-first-impressions/HEIF_Image-52EE2249BCC6-1.jpg" class="wide" >}}

## The Photo Lab

The Photo Lab is the headline addition to Halide Mark III. It lets the user work with raw images to produce a *new* opinionated JPEG. All raw images need to be interpreted in some way before being shown to the user, this is just a set of presets that a user can choose from before getting a final output.

### Halation

Halation in film is caused by light hitting the very back of the film base and reflecting around. The last layer in color film is red, so typically the reflections will pick up that red more than the other layers, which causes the red/orange glow that can be seen in certain film shots. This shows up in the brightest parts of the image, typically bright points of light.

{{< exhibit class="crop-compare" >}}
{{< figure src="/img/halide-v3-first-impressions/IMG_9843.jpg" >}}
{{< figure src="/img/halide-v3-first-impressions/IMG_9843_100crop.jpg" caption="A better look at the halation effects, the orange glow around highlights" >}}
{{< figure src="/img/halide-v3-first-impressions/IMG_9843_100crop2.jpg" caption="See how the halation bleeds over in to the girls hair" >}}
{{< /exhibit >}}

Halide introduces halation to its film recipes, and there are two options you can choose from to change how the effect renders: The Halation Strength and the Scatter. I didn't really mess with the sliders in any of the recipes here. It's hard to judge how the effect looks on the small screen of the iPhone, but if I had an iPad I'd mess with it some more.

### MTF

They call this "Micro-contrast" in the original blog post, but honestly I can't tell you how it works. I didn't experiment much with this, one of the sliders looks like it just put a Gaussian blur over the whole image. I left them at their default values for all of these exports. I like how the default recipes look, so it doesn't bother me.

### Editing raws from other cameras

You can import your regular Camera's DNGs into Halide and edit them there. I've imported some older Raw files from my M11 and run them through Halide. Let's first look at Halide's Process Zero versus its Nova profile:

{{< exhibit class="two-cl" >}}
{{< figure src="/img/halide-v3-first-impressions/IMG_9869_Process_Zero.jpg" caption="Exported with Halide's Process Zero" >}}
{{< figure src="/img/halide-v3-first-impressions/IMG_9869_Nova.jpg" caption="Exported with Halide's Nova preset" >}}
{{< /exhibit >}}

By default Process Zero doesn't add things like Halation or Grain like the other Presets. This output is just adjusting Exposure, Crop and other very basic elements of the photo. Considering this is a RAW photo from a Leica, I think the rendering is very pleasing. I prefer Halide's Process Zero over Leica's own JPEG engine. You can enable halation/grain/MTF if you go into the recipe and click a toggle.

Compared to Process Zero, the Nova image has added halation around the overhead lights, there's a vignette around the edges of the image to darken it and draw attention towards the center, and the colors are vibrant. I like how the Nova Preset works for this image.

{{< exhibit class="two-cl" >}}
{{< figure src="/img/halide-v3-first-impressions/L1000395.jpg" caption="Exported from an old Capture one file" >}}
{{< figure src="/img/halide-v3-first-impressions/HEIF_Image-92E606779DD2-1.jpg" caption="Exported with Halide's Rembrandt preset" >}}
{{< /exhibit >}}

The crops don't match up since the cropping of the RAW wasn't preserved when I moved the file over to Halide, and I just tried eyeballing it. I prefer the product of Halide's Photo Lab over my original Capture One edit! I think the white balance leans more neutral, it handles the M11's slight magenta lean better. The film effects also soften the edges around the hair a bit.

### iPhone 11 Pro

Trying out the photo lab with some old iPhone 11 Raw files yielded equally great results here. Nothing unexpected with the conversions here. The biggest thing I noticed is that the newer files off the iPhone 15 Pro held up better to darker scenes, but these shots look beautiful.

{{< exhibit class="two-cl-vh" >}}
{{< figure src="/img/halide-v3-first-impressions/11_Pro_IMG_9924.jpeg" >}}
{{< figure src="/img/halide-v3-first-impressions/11_Pro_IMG_9928.jpeg" >}}
{{< /exhibit >}}

{{< exhibit class="two-cl" >}}
{{< figure src="/img/halide-v3-first-impressions/11_Pro_IMG_9922.jpeg" >}}
{{< figure src="/img/halide-v3-first-impressions/11_Pro_IMG_9926.jpeg" >}}
{{< /exhibit >}}

The darker scene demonstrates how dynamic range and low-light performance has improved since the iPhone 11. It's serviceable.
{{< figure src="/img/halide-v3-first-impressions/11_Pro_IMG_9927.jpeg" class="vert" >}}


## Limitations

The Photo Lab is limited to the iPhone (and iPad, but I don't have one). Editing photos on a small screen sucks. And the iPhone's screen is very HDR-y, and the Photo Lab's pipeline favors an HDR-first editing approach. Often times I'll be editing a photo in HDR without realizing it (and I've disabled HDR in my Halide Settings), and then watched the export to SDR and it looks completely washed out, or too bright, or otherwise messed up.

### Crashing

This app tends to crash *a lot*. As of this review I've been using the latest release: Version 3.0.1 released on May 28th. Occasionally I've edited a photo, given it a look, and tried to edit it a second time, only for it to crash the app. After poking around, I realized that these new pictures were being saved in-place to the HEICs that Halide writes  to the gallery. If you open the Photos app and 'reset to original', it will open in Halide again. I'm sure this will get fixed in a future update, but if you're experiencing this issue in the app, that's my fix!

It is quite annoying to deal with the constant crashing. Halide's gallery feature doesn't have much in terms of filtering, so if you're navigating to the end of the gallery, or just have a lot of Raws, it can be a pain to search through. I recommend 'favoriting' any images you want to edit just so it's easier to find. The bugginess has been a recurring issue with Halide in my experience. It's a small team, so I forgive them, but it did make this review a pain to write.

Using the app in practice I believe it would be less of an issue, but it was so rampant I needed to call it out.


### Project Indigo Comparison

I've been trialing Adobe's Project Indigo in the months prior to this. Project Indigo excels at low light compared to ProRAW. I find the resulting images to be better balanced than Apple's attempt. Since Halide doesn't offer an answer to Apple's or Adobe's low light computational chops, it doesn't stack up.

{{< figure src="/img/halide-v3-first-impressions/HEIF_Image-91385DFAD3AE-1.jpg" class="normal" caption="Project Indigo Raw edited in Halide" >}}

Project Indigo Raw files are a result of Adobe's computational pipeline, combining multiple exposures to get a cleaner image (less noise) and with more dynamic range. This picture above was taken in typical dark Lower East Side NYC bar lighting. The details were so precise that Halide was able to specifically find the individual LEDs that constituted the light and applied only halation on those points. I had to adjust the halation spread to make the bar appear like a bar of light, which it looked like to our eyes. Crazy stuff.

{{< exhibit class="three-cl big" >}}
{{< figure src="/img/halide-v3-first-impressions/IDG_20251101_181523_425_2.jpg" caption="Project Indigo Export" class="vert" >}}
{{< figure src="/img/halide-v3-first-impressions/IDG_20251101_181523_425_2_Zephyr.jpg" caption="Exported with Halide's Zephyr" class="vert" >}}
{{< figure src="/img/halide-v3-first-impressions/HEIF_Image-5B63342EC083-1_Process_Zero.jpg" caption="Exported with Halide's Process Zero" class="vert" >}}
{{< /exhibit >}}

Above you can see the SOOC (Straight out of camera) differences between the JPEGs coming straight out of Project Indigo, versus Halide's Zephyr and Process Zero looks on the same image. These images were made without tweaking things like exposure in the Photo Lab, so you could adjust them slightly. I'd tone down the exposure in Zephyr and it'd look pretty good. Process Zero doesn't play nicely with Project Indigo files. I think it suffers from the same "flatness" issues that ProRAWs have.

{{< exhibit class="two-cl big" >}}
{{< figure src="/img/halide-v3-first-impressions/IMG_2947848_Valencia.jpg" caption="Exported with Halide's Valencia" >}}
{{< figure src="/img/halide-v3-first-impressions/IMG_2947848_Valencia_Indigo.jpg" caption="Project Indigo JPEG" >}}
{{< /exhibit >}}

Another comparison, this time from Prague. You can see Halide's Photo lab choosing to bloom the highlights, and we lose some of that bright white detail in the clock that we can see in the Project Indigo version. While Project Indigo's version is more technically perfect, and I do like the straight out of camera look, I think Halide captures a better *5am in Prague* feeling.

### ProRAW is weird

I can't blame Halide for this. ProRAWs are Apple's proprietary format. They already try to do some balancing between highlights and shadows, and probably bake some of that into the demosaiced RAW they save back to the file. ProRAW photos definitely have some of Apple's tastes built into the image file. The images preserve an incredible amount of data. During day shots you can recover information in the majority of the sky, as well as bring up the shadows to expose all the details lurking inside.

{{< exhibit class="two-cl" >}}
{{< figure src="/img/halide-v3-first-impressions/HEIF_Image-177A841C3A73-1.jpg" caption="Exported with Halide's Valencia" class="vert" >}}
{{< figure src="/img/halide-v3-first-impressions/HEIF_Image-4A1F-8486-48-0.jpg" caption="Exported with Halide's Valencia" class="vert" >}}
{{< /exhibit >}}

Here's a ProRAW example from the West 4th Street Courts. There's latitude to bring up everything in the shadows, and you're getting all that color information on the first image. Being a super bright and sunny day, Halide treats all those overexposed spots as needing a bunch of halation, which adds a decent effect. It's not to my tastes, and you can turn that down in the Photo Lab tab if you don't want it.

The second image is more natural looking to my tastes. We lose most of that color in the jerseys to the shadows, but we see more true colors in the court and on the trees. This is a very difficult scenario for any camera to shoot, it's incredibly contrasty. ProRAWs are difficult to edit because I think they tend to always look a bit *manufactured*, like there was some HDR-ifying to save all those details. 

There are still many reasons to shoot in ProRAW--It's the only way to get 48 Megapixel files off the iPhone. At night, that computational photography produces better results than shooting with true raw, where you'll get limited dynamic range and noise in your images.

{{< exhibit class="three-cl big" >}}
{{< figure src="/img/halide-v3-first-impressions/c1_courtsquare.jpg" caption="Capture One" >}}
{{< figure src="/img/halide-v3-first-impressions/hdr_courtsquare.jpg" caption="First Attempt, accidentally leaving HDR on" >}}
{{< figure src="/img/halide-v3-first-impressions/halide_courtsquare.jpg" caption="Nova Preset" >}}
{{< /exhibit >}}

### HDR vs SDR

Let's dive into HDR vs SDR images. If you don't care about the technical aspects, skip this section. This HDR vs SDR comparison is why sometimes you'll notice an image looks different in the 'editing' section of Halide vs when you save it. The flatter image with less contrast version? That's SDR.

iOS has support for HDR images. In this case I'm referring to HDR as the technical ability for parts of the image to be literally brighter than other parts of the screen. Nice TVs with OLED, QLED, Mini LED have the ability to make portions of the screen literally brighter than the portions. On SDR displays images are all 'emitting' the same amount of light in *lumens*, it's displaying a different 'brightness' in terms of color. That's the difference between brightness as viewed on a color wheel versus brightness in terms of a lightbulb versus a candle.

It's confusing. What's worse, there are several standards defining this new HDR: HDR10 being the most widely adopted, but there's Samsung's HDR10+ and other competitors like Dolby Vision.

What this amounts to is that you can't know for certain how your images are going to be viewed on another's monitor. If you export an HDR image, you risk the person on the other end having a monitor that applies slightly altered tone mapping. Even worse, the person on the other end might have a monitor that doesn't support HDR at all, and you'll have no creative control over what that final image looks like on their display. Different applications (like Web Browsers) can apply their own tone maps, so the same display under different applications can look different.

For this post, I've chosen to try and target just SDR for all exports. For the pictures that aren't just SDR, I've captioned them appropriately.


# Comparisons with Capture One

Capture One is currently my Image Editor of choice. I don't usually bring my iPhone Raws into Capture One unless I know I want to post them to an Instagram Post or write about them on this website. After using Halide's new photo lab, I see myself doing that even less. I thought this particular photo below, which I shot in Mong Kok, Hong Kong, would serve to best test the Photo Lab's limits. It's incredibly contrasty (Tenebristic?), with inky blacks and highlights that could easily be clipped if Halide couldn't handle the full range of the RAW file.

{{< exhibit class="three-cl big" >}}
{{< figure src="/img/halide-v3-first-impressions/L1005885_Nova.jpg" caption="Halide Nova Profile" >}}
{{< figure src="/img/halide-v3-first-impressions/L1005885_Rembrandt.jpg" caption="Halide Rembrandt Profile" >}}
{{< figure src="/img/halide-v3-first-impressions/L1005885.jpg" caption="Capture One Edited" >}}
{{< /exhibit >}}

I think the Photo Lab held up really well here. I like the results a lot. Capture One gives us many more tools to deal with the wide Dynamic Range at display here--Namely, I'm able to pull down the harsh highlights to keep the color in them. You can see that most easily with the "45" in the top right of the image. The Capture One version maintains very strong coloring and vibrancy throughout all the colors, but the two Halide options flatten the image out. I acknowledge this is personal taste, I just really like punchy, constrasty looks right now.

There is one *flaw* I think in the two Halide Images, and it's most visible in the Nova profile. Some of the blue channel looks like it's clipping. Take a look.

{{< exhibit class="crop-compare" >}}
{{< figure src="/img/halide-v3-first-impressions/L1005885_Nova.jpg" >}}
{{< figure src="/img/halide-v3-first-impressions/L1005885_Nova_crop.jpg" caption="Note the reflection of the Neon Sign's blue is incredibly dark. This looks like clipping to me." >}}
{{< /exhibit >}}

The RAW files from the M11 are pretty well balanced, rendering close to true. Because they don't exhibit the artificial flatness that the ProRAWs or the Project Indigo Raws had, I tested with a couple more images; Now for a comparison I'm embarrassed by:

{{< exhibit class="two-cl-vh" >}}
{{< figure src="/img/halide-v3-first-impressions/L1005502_Halide.jpg" >}}
{{< figure src="/img/halide-v3-first-impressions/L1005502.jpg" >}}
{{< /exhibit >}}

I like Halide's Nova output better than what I put together for this picture in Capture One (Left image is Halide, Right is Capture One). I didn't edit the image on the right, it's the same output as what's in the [Japan 2026 post](/gallery/japan-2026) right now! The lighting around the lanterns is less harsh, and the image isn't as constrasty. There's no right or wrong way to edit images, but I definitely like the *feel* of the Halide Image more. The halation around the cat really works for this image.

## Verdict

This is now my favorite app to edit iPhone photos. Here's my current list of camera apps I keep in rotation:

* Halide Mark III
* Adobe Indigo
* Default Camera App

The default Camera app is mostly just to shoot in night mode if I think I need the ultra-processing. Project Indigo is used in tricky lighting situations where I think the computational photography aspect can help out. For dark interior scenes with not much light, it's usually my go to. Halide will be for everything else. It can take ProRAW images, regular RAW, but the main selling point these days is the new Photo Lab. I think going forward I'll be replacing Lightroom mobile with Halide for quickly editing the Raw images from my Leica M11 before posting them to social media if I don't have a computer nearby.

I would recommend Halide as a better use of money for those wishing to get the "Digicam" or "Vibey" look from older cameras. People tend to want to spend around 300 dollars or less for a digital camera to capture a more nostalgic look, and I think throwing a RAW into the photo lab with Process Zero, Valencia or Nova yields better results. And now you don't have to carry around an additional camera.

[Halide Mark III is available on the App Store](https://apps.apple.com/us/app/halide-mark-iii-pro-camera/id885697368) for $60 dollars as a one-time purchase, or $20 dollars for a yearly subscription. There's a 1 week free trial if you're on the fence!


### Pros and Cons 

**Pros**
* Best JPEG output from any iPhone App
* Perpetual purchase option available
* Multiple Film Recipes offer several options
* Great general photo taking app, supporting Raw, ProRAW, and regular JPEG shooting
* Options for lock screen integration, action button integration

**Cons:**
* Limited to iPhone and iPad
* Currently, crash prone in Photo Lab
* Heavy CPU usage (But, mostly expected)
* Filtering in Photo Lab is limited, hard to find photos if there is a crash
* Export Options limited to 10MP

#### Disclaimer -- HEIC conversions

The photos you'll see are either JPEG or JPEG-XL depending on your browser's support for the formats. Halide Mark III currently only exports in HEIC format, so there was some formatting using Mac OS's built in `sips` tool at Quality 95. So there may be some image degradation as a result of the conversion.

*Edit:* Occasionally I did get the option when saving to export in JPEG, but it's seemingly random. So this is probably a bug of some sort that needs fixing. You can also choose to have the iPhone do the conversion for you if you're airdropping the photos to yourself.

Halide does have a toggle for exporting in JPEGs, but it seems like there is a bug where that isn't respected. I tried a couple different approaches, like Airdropping the output of a Film simulation directly to my Mac vs saving the image to the gallery and exporting it from there. It was always saving it as HEIC. The quality difference is probably negligible, but it was another bug that I thought was annoying.

#### Further reading

There are plenty of third party camera apps on the app store. Here are some apps I've heard good things from but never tried out myself in case you want to explore:

* [Better Camera](https://bettercamera.heygor.com)
* [Moment Pro Camera II](https://apps.apple.com/us/app/moment-pro-camera-ii/)
