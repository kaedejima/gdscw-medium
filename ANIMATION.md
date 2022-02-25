# Gradient animation
[Gradient Animation Codepen](https://codepen.io/kaedejima/pen/QWqeGBG)

1. Set a gradient background.
2. Use background-clip to clip the background to the text fill
3. Expand the background size
4. Define a `@keyframe`
5. Set keyframe to animation

### Set a gradient background.
```css
h1{
  /* STEP1 */
  background: radial-gradient(circle, #F48FB1 0%,  #CE93D8 20%, #B2EBF2 40%, #A5D6A7 60%, #B39DDB 100%); 
  /* STEP2 */
  -webkit-background-clip: text;
  /* STEP3 */
  background-size: 400%;
  /* STEP5 */
  animation: gradient 5s linear infinite alternate;
}

/* STEP4 */
@keyframes gradient {
  0% {
    background-position: 0%;
  }
  100% {
    background-position: 100%;
  }
}
```