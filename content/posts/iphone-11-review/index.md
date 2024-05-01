---
title: iPhone 11 Pro Long Term Photography Review
draft: false
showtoc: true
date: 2024-05-01
showReadingTime: true
env: production
summary: Why you don't need a Digicam
cover:
    image: '/img/iphone11/IMG_3752.jpg'
tags: [Apple, iPhone, iPhone 11 Pro, Halide, Review, Photography, Mobile, iOS]
---
{{< rawhtml >}}
<style>
figure.entry-cover {
 width:100vw;
 position: relative;
 left: calc(-50vw + 50%);
}
</style>
{{< /rawhtml >}}

{{< exif src="/img/iphone11/IMG_2710.jpg" >}}
*"The best camera is the one you have with you."* -Chase Jarvis

Everyone carries a phone with them, all of those phones come with cameras, usually more than one. I owned the iPhone 11 Pro from 2019-2023, and through those years I took thousands of photos. Through apps like Snapchat, to BeReal to Halide. We're all taking photos with our phones now, social media pretty much requires it.
## Design
{{< figure src="/img/iphone11/header.jpg" caption="Remember when we thought this was a big camera bump?! &#169;Apple" >}}
## Triple Sensors, three lenses
The iPhone 11 Pro came with three rear cameras. The Telephoto is a 52mm Full Frame (**FF**) equivalent had such poor performance this generation and was so close to the main sensor's focal length (26mm FF equivalent) that I couldn't find any pictures taken with the camera within the past two years. The Ultrawide (13mm FF equivalent) was novel and could get you images simply impossible with the main, so despite its shortcomings, saw a decent amount of use. Known as the 0.5x camera on social media, the way it distorts its subjects at close range makes for novel and fun shots.
### The Main Camera
{{< exif src="/img/iphone11/IMG_3752.jpg" >}}
{{< exif src="/img/iphone11/IMG_3355.jpg" >}}
The sharpest lens combined with the largest sensor (1/2.55" inch), this was my go-to for 95% of my shots. Minimum focus distance wasn't shabby at 4.7 inches either. Later models see their minimum focus distance go all the way up to 7.8 inches, nearly doubling the length you have to be from your subject. Apple's gotten around this by trying to cleverly switch to its ultrawide lens, but the behavior can be annoying if you don't know whats happening and things seem to switch on you.

But on this generation, this lens was the best one to use, and the pictures on this post are all taken with it. This was a good 12MP, the lens was easily able to outresolve what the sensor was capable of capturing, which made for some decent cropping ability. This combo was so good that at low light, your iPhone would sometimes just take a crop of the main sensor's image when you were trying to take a photo with your Telephoto lens! The only way to know for sure would be to check the metadata in the photo and see what the resolution would come out to be.
{{< exif src="/img/iphone11/IMG_2756.jpg" >}}

### The Ultrawide Camera
Not too much to say here. This was Apple's first attempt at putting ultrawide optics camera on an iPhone. As with the rest of the cameras, feed the sensor enough light, and you can get good quality images out of it. The lens was fixed-focus at this time, so all you had to do was hope the exposure was right and fire away. I wouldn't bother with this camera at night, the sensor was too small and the optics weren't great either. No RAW from this camera in the iPhone 11 either, but later generations added this feature. Either through ProRaw or giving you access to the full fledged raw.
{{< exif src="/img/iphone11/IMG_3738.jpg" >}}
### The Telephoto
This is a 2x of the wide lens, bringing up to around a 50mm in Full Frame terms. Oddly enough, I couldn't find any images worth sharing that I took with this lens. I think a combination of not being *that* much longer than the normal wide, combined with a slower aperture and a smaller sensor just made this overall unappealing. It wasn't a big enough change from the default len, and would completely fall apart in any challenging lighting conditions. When Apple moved the telephoto from 2x to 3x they got it right. Big enough change combined with larger sensors made them worth using. But for this generation, unless you were shooting in bright light or outdoors it didn't get me excited enough to want to use it.

## The RAWs
The RAWs out of this camera are finnicky. Under good lighting, they can be quite easy to work with. In Capture One, they're pretty easy to correct the basic flaws. Limited Dynamic range means you'll need to bring down the highlights and up the shadows to get something looking more 'normal' as a base, and there's quite a bit of vignetting to the images that needs to be fixed. I went ahead and created a 'style' in Capture One and just applied it to all of my images tagged with the camera as a starting point.

### RAW vs Processed RAW vs HEIC
{{< exif src="/img/iphone11/no_adjustments.jpg" >}}
{{< exif src="/img/iphone11/edited_raw.jpg" >}}
{{< exif src="/img/iphone11/SOOC.jpg" >}}
Here I tried to show that you can get a Raw image to look pretty close to the HEIC's the camera puts out. It's tricky to do it in camera, and you'll need a third-party tool to really get close, but I prefer the look of the edited raw to the HEIC in this shot.

You lose some dynamic range, with the clouds going to white quicker than in the HEIC, but you get a more balanced look in the edited RAW I feel. I chose to get rid of the hazier look of the mountains in the background in this shot, but if you wanted to, keep the midtones of the image a little flatter and you could keep that hazy look too. 

It's almost impossible to take the RAWs and make them look like the SOOC images in anything but super flat lighting, but that's because the iPhone is combining multiple shots taken with different exposures intelligently behind the scenes whereas the RAW is just that. One shot, and you get all the pixel data to mess around with. 

Example Images Captured using Halide's HEIC+RAW mode.

## Straight Out of Camera (SOOC) Images
With good lighting, you can get really punchy images with good color and very little noise. 
{{< exif src="/img/iphone11/IMG_2516.jpg" >}}
{{< exif src="/img/iphone11/IMG_2593.jpg" >}}

I love the colors and details in these images. Colors seem vivid without coming across as oversaturated, and there's enough light so the phone doesn't have to do aggressive noise reduction to smooth images out. Deep fusion does a good job of keeping the details on the jacket nice and sharp and well separated without giving *too* many oversharpening artifacts on other areas of the image. Relatively flat lighting on this overcast day means that the HDR didn't have to work too hard to balance the exposure, pretty much a dream scenario for showing off this generations HDR capabilities.

{{< exif src="/img/iphone11/IMG_1831.jpg" >}}
In challenging lighting conditions, Apple tries to do everything, preserve highlights and raise shadows, resulting in scenes that look a bit too HDR-ish. The tones feel off in this photo, it was quite dark inside with bright sunlight beaming through this AirBNB. I do feel like most people would like this photo, as the subject is well lit, but it doesn't feel true to the scene.

{{< exif src="/img/iphone11/IMG_1110.jpg" >}}
In really dark situations like seen here @ Radio City Music Hall, the Phone really makes the scene quite bright, and adds lots of processing. Zoom in to see the massive amounts of noise reduction applied to the musicians in their seats!

#### Verdict:
Overall I'd give the SOOC shots a 8/10. Very usable, even when they're not all to my taste.

## Taking Pictures
There were two ways I took photos on this phone:
- Native Camera App
- [Halide](https://halide.cam)

### Halide Mini Review:
Will likely cover Halide in another post, but the short of it is:
- Well Designed
- Well Thought out Features
- Inconsistent Quality throughout the years
- Pricey

I'd give the app itself a 8.1/10, some really unique features, I think the design is one of the best out there, and the experience is quite delightful. But unless you're serious about taking photos on a phone, I wouldn't recommend it because of its subscription model. 

On newer iPhones (such as the iPhone 15 Pro), you can shoot proRAW straight from the native camera app. You could only do this from the iPhone 12 series onward, and you can't shoot regular RAW from this app, so you'll need to download a third-party app to cover that.

## Closing Thoughts
Cameras on Phones have officially gotten good. They've been good since around the iPhone 6S, and have only improved year after year. Whatever phone you have, iPhone or Android, don't let the fact that you kept your other camera at home stop you from taking that shot. I haven't owned a Pixel but I've seen what they're capable of, Samsung phones too. They're all really good.

Embrace the all-auto life, let the camera do the thinking for you and trust in the algorithms. Or switch to Raw and edit them later. It's important to study and understand the characteristics of your phone and its cameras to best use them. Knowing *whether* taking a shot with Raw or with the SOOC jpegs is important to maximize image quality.

But if the moment is fleeting, just take the shot, you'll regret not taking it more than anything else.