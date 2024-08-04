# Scroll Trigger Method in Gsap


ScrollTrigger enables anyone to create jaw-dropping scroll-based animations with minimal code. Infinitely flexible. Scrub, pin, snap, or just trigger anything scroll-related, even if it has nothing to do with animation.


cdn: 
```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.5/ScrollTrigger.min.js" integrity="sha512-onMTRKJBKz8M1TnqqDuGBlowlH0ohFzMXYRNebz+yOcc5TQr/zAKsthzhuv0hiyUKEiQEQXEynnXCvNTOk50dg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
```


### Simple Example
```javascript 
gsap.to('.box', {
    scrollTrigger: '.box', // start the animation when ".box" enters the viewport (once)
    x: 500
});
```

## Scroll Trigger Properties

***1. trigger:*** The trigger element (if one was defined). If selector text was used, like ".trigger", the trigger will be the element itself (not selector text)

```javascript 
scrollTrigger: {
    trigger: "#page1 #box" 
}
```
***2. scroller:*** The scroller element (or window) associated with the ScrollTrigger. It's the thing whose scrollbar is linked to the ScrollTrigger. By default, it's the window (viewport).

```javascript 
scrollTrigger: {
    scrollTrigger: "body"
} 
```

***3. start:*** The ScrollTrigger's starting scroll position (numeric, in pixels).

```javascript 
scrollTrigger: {
    start: "top 60%"
}
```

***4. end:*** The ScrollTrigger's ending scroll position (numeric, in pixels).

```javascript 
scrollTrigger: {
    end: "top 30%"
}
```

***5. Scrub:*** Links the progress of the animation directly to the scrollbar so it acts like a scrubber. You can apply smoothing so that it takes a little time for the playhead to catch up with the scrollbar's position! It can be any of the following

```javascript 
scrollTrigger: {
    scrub: true // It can be boolean value or for smooth transition (1 - 5)
}
```

***6. Pin:*** Boolean | String | Element - An element (or selector text for the element) that should be pinned during the time that the ScrollTrigger is active, meaning it will appear to "stick" in its starting position while the rest of the content continues scrolling underneath it. Only one pinned element is allowed, but it can contain as many elements as you want. Setting pin: true will cause it to pin the trigger element.

```javascript 
scrollTrigger: {
    pin: true
}
```
