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

-  animation property is like the settings of the animation
-  you define how long you want the animation to take, delays, times the animation will run, and timing of the animation

Synatx
```css
animation: duraction  timing-function  delay  iteration-count  direction  fill-mode  play-state  name;
animation: 3s ease-in 1s 2 reverse both paused slidein;
```
