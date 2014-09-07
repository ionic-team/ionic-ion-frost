Ionic Contrib: Frosted Glass
===================

A reusable frosted-glass effect for adding this cool iOS effect to your Ionic apps. (this is an updated and more generic version of our old [Ionic Frosted Glass Header](https://github.com/driftyco/ionic-contrib-frosted-glass) contrib). It looks like this:


<p data-height="266" data-theme-id="3572" data-slug-hash="pmBch" data-default-tab="result" data-user="ionic" class='codepen'>See the Pen <a href='http://codepen.io/ionic/pen/pmBch/'>Ionic Contrib: Frost</a> by Ionic (<a href='http://codepen.io/ionic'>@ionic</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//codepen.io/assets/embed/ei.js"></script>

<img src="http://ionicframework.com.s3.amazonaws.com/contrib/frost2.png" style="width: 319px; background-size: 100%">

### Use

To use, add the attribute `frost` to the element you want to blur. Then, you'll want to add an overlay to give a nice faded effect for content on top. The demo has a dark overlay you can use:

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
```

See `demo/index.html` for an example.

### Updating the Frost

When the content changes underneath, you need to update the frosted effect. To do that in a controller (for example), inject the `$ionicFrostedDelegate` and call `update()` on it:

```javascript
controller('MyCtrl', function($scope, $ionicFrostedDelegate) {
  $scope.contentChanged = function() {
    $ionicFrostedDelegate.update();
  };
});
```

