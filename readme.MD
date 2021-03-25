# Split Text Library for GSAP 
This is a basic function that will split characters into spans either by word
or by character. 
  
  
## What is the point of this library?  
Well, I don't make enough money with gsap to justify the annual membership to
use GreenSock's SplitText plugin.  It works in a similar manner, but doesn't
do nearly as much as Green Sock's own plugin.  If you need the more advanced
features, you can get Green Sock's plugin with an annual membership.
  
  
## How do you use this function and why should I care? 
Good question. You basically would send the function an HTML element and an
optional config object if you want to split the text by individual letters.
The default will split the text by word.  You can then send the children
of the element to gsap to animate each word or letter individually.
  
  
```
const text = document.getElementById('text')
SplitText(text, {split: 'letter'}) // 2nd argument is optional

// Each character will now be wrapped in spans with the style property with display: inline-block

gsap.to(text.children, {
    // gsap animation properties.  Add a stagger to have them animate one after another.
    })

```