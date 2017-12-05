# Air Horner

This is an implementation of [Airhorner](https://github.com/PaulKinlan/air-horner) by [PaulKinlan](https://github.com/PaulKinlan)
View that repo for tag/component details

## What is different from PaulKinlans implamentation then? 
This implementations dependencies are checked in, so the component can be called from another domain across the web directly from the repository.

## FAQ

### How do I include this?

There are two ways.

1. `<link rel="import" href="https://rawgit.com/ltomes/air-horner/master/air-horner.html">`
2. `<script src="https://rawgit.com/ltomes/air-horner/master/air-horner.js"></script>`

The element name is already defined in the script as `<air-horner>`.

### Is it possible to change the horn sound?
Yes. You can change the src attribute on the element. Note, if you want the
audio to loop you need to define a `loopStart` and `loopEnd` attribute. Finding
a good loop point is left to the reader ;)

<!--
```
<custom-element-demo>
  <template>
    <link rel="import" href="air-horner.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<air-horner src="test/sounds/yo.mp3" loopStart="0.616" loopEnd="1.078"></air-horner>
```

By default the `airhorn.mp3` is used.
