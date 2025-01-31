# GSAP-JS

GSAP (GreenSock Animation Platform) is a powerful JavaScript library for creating animations. Below are some of the essential methods and properties you can use in GSAP to create stunning animations:

## Methods

### 1. `gsap.to("", {})`

The most common type of animation is a `to()` tween because it allows you to define the destination values (most people think in terms of animating to certain values). Basically, `.to` is used to move the object from its initial position to its final position.

### 2. `gsap.from("", {})`

The `from()` method is used to move the object from its final position to its initial position.

## Properties

### 3. GSAP Stagger Property

When you have multiple elements and want to apply the effect one by one, you can use the `stagger` property. 

```javascript
stagger: 1 // Executes the elements line by line
```

### 4. GSAP Repeat Property
The repeat property can be used to repeat the effect multiple times.
```javascript
repeat: 1 // Repeats the animation once
repeat: 2 // Repeats the animation twice
repeat: -1 // Repeats the animation infinitely
```

### 5. GSAP Yoyo Property
Gets or sets the tween's yoyo state, where true causes the tween to go back and forth, alternating backward and forward on each repeat.

```javascript 
yoyo: true
```

### 6.GSAP Timeline
A Timeline is a powerful sequencing tool that acts as a container for tweens and other timelines, making it simple to control them as a whole and precisely manage their timing. Without Timelines, building complex sequences would be far more cumbersome because you'd need to use a delay for every animation.

Example:
```javascript
var tl = gsap.timeline();
```

