# holding-fire

<p align="center">
  <img alt="holding-fire" src="Holding-Fire.png" width="300">
</p>

<p align="center">
A simple way to create a holding page
</p>

<p align="center">
  <a href="https://webcomponents.org/element/convoo/holding-fire"><img src="https://img.shields.io/badge/webcomponents.org-published-blue.svg"></a>
  <a href="https://gitter.im/convoo/general"><img src="https://img.shields.io/badge/gitter-join%20chat-brightgreen.svg"></a>
  <a href="http://waffle.io/convoo/roadmap"><img src="https://badge.waffle.io/convoo/holding-fire.svg?label=In%20Progress&title=In%20Progress"></a>
</p>

---

## Install 

```
bower install holding-fire --save
```

# \<holding-fire\>

An element that uploads files and provides download url from Firebase Storage. For images, it can resize and provide a placeholder as well.

```html
<link rel="import" href="/bower_components/holding-fire/holding-fire.html">
```

<!--
```
<custom-element-demo>
  <template>
    <link rel="import" href="holding-fire.html">
    <link rel="import" href="../polymerfire/firebase-app.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<firebase-app
    name="inline"
    api-key="AIzaSyAhoCXxkY-ffNwA_7L7HIwBVpASYj1btNE"
    auth-domain="convoo-login-demo.firebaseapp.com"
    database-url="https://convoo-login-demo.firebaseio.com">
</firebase-app>
<holding-fire
    app-name="inline"
    path="/subscribers"
    alt="Convoo"
    logo="images/lipsum.png"
    email="hello@example.com"
    sub-header="Sign up to find out when we launch!"
    sub-button="Sign up"
    thanks="Thank you for subscribing!"
    thanks-header=""
    twitter = "example"
>
    <p>A revolutionary new startup. Website coming soon!</p>
</holding-fire>
```

See the demos by clicking in the sidebar on [webcomponents.org](https://webcomponents.org/element/convoo/holding-fire) for more.

### Styling

Style the element with CSS as you would a normal DOM element. 

The following custom properties and mixins are available for styling:

| Custom property | Description |
| --- | --- |
| `--holding-fire-host` | Mixin for the host element |
| `--holding-fire-overlay` | Mixin for an overlay |
| `--holding-fire-container` | Mixin for the container |
| `--holding-fire-logo` | Mixin for the logo |
| `--holding-fire-inner-container` | Mixin for the inner container with content and form |
| `--holding-fire-content` | Mixin for the content section |
| `---holding-fire-subscribe-container` | Mixin for the subscribe container|
| `---holding-fire-subscribe-title` | Mixin for the subscribe title|
| `---holding-fire-subscribe-form` | Mixin for the subscribe form|
| `--holding-fire-input` | Mixin for the inputs |
| `---holding-fire-subscribe-button` | Mixin for the subscribe button|
| `--holding-fire-email` | Mixin for the email paragraph |
| `--holding-fire-email-link` | Mixin for the email text |
| `---holding-fire-thanks-container` | Mixin for the thanks container|
| `---holding-fire-thanks-title` | Mixin for the thanks title|
| `---holding-fire-thanks-section` | Mixin for the thanks section|
| `--holding-fire-twitter-link` | Mixin for the twitter link |
| `--holding-fire-twitter-button` | Mixin for the twitter button |
| `--holding-fire-animations` | Mixin for any animations you want to define. First one will not be registered. See demo. |


## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install


## Playing With Your Element

If you wish to work on your element in isolation, we recommend that you use
[Polyserve](https://github.com/PolymerLabs/polyserve) to keep your element's
bower dependencies in line. You can install it via:

    npm install -g polyserve

And you can run it via:

    polyserve

Once running, you can preview your element at
`http://localhost:8080/components/image-fire/`, where `image-fire` is the name of the directory containing it.
