# holding-fire

<p align="center">
  <img alt="holding-fire" src="HoldingFire400.png" width="300">
</p>

<p align="center">
A simple way to create a holding page
</p>

<p align="center">
  <a href="https://webcomponents.org/element/convoo/holding-fire"><img src="https://img.shields.io/badge/webcomponents.org-published-blue.svg"></a>
  <a href="https://gitter.im/convoo/general"><img src="https://img.shields.io/badge/gitter-join%20chat-brightgreen.svg"></a>
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
```html
<holding-fire app-name="demo" path="users/" logo="images/logo.png" text="Website coming soon! Subscribe to find out when we launch!" email="hello@convoo.me"></holding-fire>
```


### Styling

Style the element with CSS as you would a normal DOM element. 

The following custom properties and mixins are available for styling:

| Custom property | Description | Default |
| --- | --- | --- |
| `--holding-fire-background-image` | The background image | `url(images/background.jpg)` |
| `--holding-fire-background-color` | The background color of the element | `black` |
| `--holding-fire-text-color` | The color for the text  | `white` |
| `--holding-fire-button-color` | The color for the subscribe button | `#60b559` |
| `--holding-fire-button-text-color` | The color for button text | `white` |
| `--holding-fire-email-color` | The text color for the email | `white` |
| `--holding-fire-logo-width` | The logo width | `300px` |
| `--holding-fire-logo-height` | The logo height | `80px` |
| `--holding-fire-overlay-color` | The color of the overlay | `black` |
| `--holding-fire-overlay-opacity` | The opacity of the overlay | `0.6` |
| `--holding-fire-shadow-color` | The color of the box shaddow | `black` |

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
