### flexslider
---
https://github.com/woocommerce/FlexSlider

```js
(function(){
  var $window = $(),
      flexsilder = { vars:{} };
  function getGridSize(){
    return (window.innerWidth < 600) ? 2 :
           (window.innerWidth < 900) ? 3 : 4;
  }
  $(function(){
    SyntaxHighlighter.all();
  });
  $window.load(function(){
    $().flexslider({
      animation: "slide",
      animationLoop: false,
      itemWidth: 210,
      itemMargin: 5,
      minItems: getGridSize(),
      maxItems: getGridSize()
    });
  });
  $window.resize(function(){
    var gridSize = getGridSize();
    flexslider.vars.minItems = gridSize;
    flexslider.vars.maxItems = gridSize;
  });
}());
```

```js
$(window).load(function(){
  $('.flexslider').flexsider({
    animation: "slide"
  });
});

$(window).load(function(){
  $('.flexslider').flexslider({
    animation: "slide",
    controlsContainer: $(".custom-controls-container"),
    customDirectionNav: $(".custom-navigation a")
  });
});
```

```js
//https://github.com/woocommerce/FlexSlider#examples
$(window).load(function(){
  $('.flexslider').flexslider({
    animation: "slide"
    animationLoop: false,
    itemWidth: 210,
    itemmargin: 5
  });
});
```

```
$(window).load(function() {
  $(window).load(function() {
    $('.flexslider').flexslider();
  });
});
```
