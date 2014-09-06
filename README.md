Ionic Contrib: Frosted Glass
===================

A reusable frosted-glass effect for adding this cool iOS effect to your Ionic apps. It looks like this:

<img src="http://ionicframework.com.s3.amazonaws.com/contrib/frost2.png" style="width: 319px; background-size: 100%">

### Use

To use, add the attribute `frost` to the element you want to blur. Then, you'll want to add an overlay to give a nice faded effect for content on top:

```html
<ion-pane frost>
</ion-pane>
<ion-pane class="my-overlay">
</ion-pane>
<style>
// Example dark overlay:
.my-overlay {
  background-color: #222;
  opacity: 0.8;
}
</style>

See `demo/index.html` for an example.
