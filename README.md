# CSS Animations

## What is CSS Animations?

You can write raw css and change as many CSS properties as you want.
You won't need to rely on JavaScript or any libraries. This will make
your code more efficient and your code base uses everything there is
because usually CSS libraries has a lot of animations that you don't need.

## How It's Done?

1. Within a class, you define the animation property and link it to an animation that you will create.
2. Define that animation using keyframes.

Example
```css
.new {
  transform: scale(0);
  animation: new 0.25s linear 0.2s forwards;
}

@keyframes new {
  from { transform:  scale(0); }
  to { transform: scale(1); }
}
```

## Syntax of Animation Property

-  Animation property is like the settings of the animation
-  You define how long you want the animation to take, delays, times the animation will run, and timing of the animation

Sugar Synatx
```css
.syntax {
  animation: duraction  timing-function  delay  iteration-count  direction  fill-mode  play-state  name;
}

.example {
  animation: 3s ease-in 1s 2 reverse both paused name;
}
```

Long Gross Syntax
```css
.grossLongSyntax {
  animation-name: name;
  animation-duration: 2s;
  animation-delay: 2s;
  animation-timing-function:ease;
  animation-iteration-count: 2;
  animation-fill-mode: backwards;
  animation-direction: normal;
  animation-play-state: running;
}
```

### Important Note

-   The order of the items in animation is not imporant
-   Only the order of timing is. Duration must be infront of delay
-   You don't need to fill in all the options for animation

## Keyframes

-  This is where you define if you want something to change colors, get bigger,
   move, or do some crazy flips. You can play around with all the css properties
   like color, size, height, width, margin, padding, position.

### Synatx of Keyframes

- There are two ways to do it. You can use from and to, or use percents. If your animation
  is simple, you should use from and to. If you need something more advanced you should
  use percents.

Synatx of From and To
```css
@keyframes animationName {
  from { cssProperties: option; },  /* Start of the animation */
  to { cssProperties: option; }     /* End of the animation */
}
```

Example
```css
@keyframes new {
  from { transform:  scale(0); }
  to { transform: scale(1); }
}
```
### Important Note

- You can add as many properties are you want in from and to.
- If you want to incorporate movement, you usually use transform property.

Synatx of %
```css
@keyframes animationName {
  0% { cssProperties: option; },  /* Start of the animation */
  50% { cssProperties: option; }   /* Half of the animation */
  100% { cssProperties: option; }     /* End of the animation */
}
```

Example
```css
@keyframes upgraded {
  0% { transform: scale(1.4) }
  50% { transform: scale(0.7) }
  100% { transform: scale(1) }
}
```

# Resources
1. [W3Schools](https://www.w3schools.com/)
2. [CSS-Tricks](https://css-tricks.com/css-animation-tricks/)
3. [Net Ninja CSS Animations](https://www.youtube.com/watch?v=jgw82b5Y2MU&list=PL4cUxeGkcC9iGYgmEd2dm3zAKzyCGDtM5)
4.
