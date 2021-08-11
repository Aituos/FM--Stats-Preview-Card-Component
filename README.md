For me, there were two challenges in this... uh, challenge, that I didn't really know how to tackle.

First of all:

## The image you get is in grayscale

Okay cool, I thought, the solution would be to throw it into something like GIMP and just colorize it - but there's nothing to learn from that really. I already know how to do it. I knew it was possible to do this with just CSS and I recently saw a video on the very subject. Obviously I couldn't remember anything from the video, so I searched for it with no luck.

(Takes a deep breath)
The next hours were full of convoluted ideas involving absolute positioning of precisely-sculpted half-transparent pinkish divs over the image or using ::after pseudo-elements to achieve the desired end result and it was all *horrible*.

After two or three days I finally caved and looked for a solution on YouTube. This is the video I selected:

https://www.youtube.com/watch?v=2tlbKm8_4mg

I watched the first few minutes, then decided to get distracted and look at the comments. One comment in particular casually mentioned background-blend-mode.

background-blend-mode...

:weary:

BACKGROUND BLEND MODE, oh my god.

It was relatively quick and painless after that. I simply created a div, set its' background-image and background-color, and background-blend-mode to soft-light. I then tweaked the color to make it look as close to the preview as possible. Done. Three lines of code (and I think it might be possible to do with just two).