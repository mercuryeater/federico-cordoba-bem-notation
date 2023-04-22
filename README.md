# federico-cordoba-bem-notation

This is the solution to "card" proyect of Make It Real using flex.

## Overview

### The challenge

The user will see a card in the center of the screen with the profile 
of someone, where you can see the photo of the person, name, visual rating 
and a brief description.
Below this, in the same card two buttons, one more attractive than the other, 
appearing as if one of them was selected or just about to be pressed.

### Screenshots
One and only:  

![SS of the challenge "card"](https://raw.githubusercontent.com/mercuryeater/federico-cordoba-bem-notation/main/ss/ss.png)

## My process
### Built with
- HTML5
- CSS
- Block Element Modifier (BEM) Notation
- Flexbox 
### What I learned

First time using the BEM notation, was a little scare at first but it wasn't actually that hard, 
i feel sometimes that there's a lot of divs and long names for the classes going on.

Satarted creating the card container for everything in screen, inside it I created 3 divs, firts one for the photo, the name and the rating because they are closer together honestly *-and actually writing
this I realize that I could have made just two-*, second one for the description, and third one for the buttons.

In the first `<div>` with the photo on a circle I learned about the `object-fit` property and `cover`
value. This property sets how the content of a *replaced element* (it's representation is outside the scope of CSS: img, video, embed, iframe) should be resized to fit it's container.

I discovered there was something beyond the `border` called the `outline`, that behaves almost identical to the border but it is not read by as part of an element's dimention(can overlap other content).

I had a div for the buttons on the bottom of the card container and I wanted them to be rendered in a way that they almost fit the container, so I used `justify-content: space-between` on the div, and inside of each button I used `flex-basis: 49%` meaning that each of them filled the 49% percetn and 
because of the `space-between` they had a space in the middle. Also I had an issue with the font because tey were not inheriting the font, so I had to use `font-size: inherit`, and that made it.

I was a great way of practicing *flexbox*, the difference of items and content, the understanding of 
the *primary axis* and *cross axis* when using flexbox.

### Continued development

I need to keep practicing flexbox and how does their scopes work, and when to use it, becuse I feel it isn't always necessary *-maybe I'll regret saying this-*.
I think I'm ready to make something a little bit more complex, because I do feel that I need to consolidate what I just did.

I'm also intrigued by the use of `box-sizing` because I feel that it can correct overflow with it, we'll see.

After my correction I put the `h4` element displaying the name on his own div, and dis the same on the `p` element with the description. While donig this I checked and deleted some styles that were actually doing nothing (Sometimes I try something, it doesn't work and just forget to delete them, working on it). 

### Useful resources

- **'object-fit: cover'** to use on the image inside a circle, avoiding distortion: 

https://developer.mozilla.org/en-US/docs/Web/CSS/object-fit


- **'outline'** to give it a visual emphasis to the photo:

https://www.w3schools.com/css/css_outline.asp


- **'flex-basis'** to set the initial main size of a flex item:

https://developer.mozilla.org/en-US/docs/Web/CSS/flex-basis


## Author
- Name - Federico Cordoba 
- Twitter - [@mercuryeater](https://twitter.com/Mercuryeater/)



