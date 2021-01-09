<p align="center">
  <a href="https://freezy.dev/">
    <img src="https://kepkuldes.com/images/adbad50b5c360138e05feb95c215f4e0.png" alt="dCSS logo" width="200" height="220">
  </a>
</p>

<h3 align="center">dCSS</h3>

<p align="center">
  Discord inspired mini front-end framework with sleek and clean components.
  <br>
  <br>
  <a href="mailto:freezy0001w@gmail.com">Report bug</a>
  ·
  <a href="mailto:freezy0001w@gmail.com">Request feature</a>
  ·
  <a href="soon.tm">Discord</a>
</p>

## Table of contents

- [Install](#install)
- [Documentation](#documentation)
- [Creator](#creator)
- [Copyright and license](#copyright-and-license)


## Install

Several install options are available:

- Clone the repo: `git clone https://github.com/freezy0001/dcss.git`
- Link with [cdn](https://www.jsdelivr.com/): `<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/freezy-0001/dcss/dist/css/d.min.css" integrity="sha384-qtoT/TpmVai9KuwydVBbrjfX5dNmeqnmieuS5cx5jB+hYl+Z8RZnCYUbon1BVPfz" crossorigin="anonymous">`


## Documentation

### Components

- [Colors](#colors)
- [Text](#text)
- [Buttons](#buttons)
- [Embeds](#embed)
- [Checks and radios](#checks_and_radios)
- [Select](#select)
- [Range](#range)

### Colors

dCSS is supported by Discord's extensive color system that themes our styles and components. This enables more comprehensive customization and extension for any project.

#### Theme colors

We use a subset of all colors to create a smaller color palette for generating color schemes.

<img src="https://kepkuldes.com/images/fe93d81710acbf7d7d2b769d4b58b8c3.png" alt="dCSS logo" width="400" height="36">

`.*-primary` `.*-secondary` `.*-success` `.*-danger`

#### Text-only colors

These color classes are only can be used on texts.

<img src="https://kepkuldes.com/images/2e401b1b4203c81d5244eb5e8f56d937.png" alt="dCSS logo" width="400" height="26">

`.dcolor-blue` `.dcolor-red` `.dcolor-green` `.dcolor-grey` `.dcolor-dark` `.dcolor-darkr` `.dcolor-black` `.dcolor-white`

### Text

Documentation and examples for common text utilities to control style and weight.

#### Font weight and italics

Quickly change the `font-weight` or `font-style` of text with these utilities. `font-style` utilities are abbreviated as `.dfst-*` and `font-weight` utilities are abbreviated as `.dfw-*`.

<img src="https://kepkuldes.com/images/a696cd901514755ccd0a6504a71006eb.png" alt="dCSS logo" width="400" height="330">

```
<p class="dfw-bold">Bold text.</p>
<p class="dfw-normal">Normal weight text.</p>
<p class="dfw-light">Light weight text.</p>
<p class="dfst-italic">Italic text.</p>
<p class="dfst-normal">Text with normal font style</p>
```

### Buttons

Use dCSS's custom button styles for actions in forms, dialogs.

#### Examples 

dCSS includes several predefined button styles, each serving its own semantic purpose.

<img src="https://kepkuldes.com/images/1b9687fbd1269611ffa9271e476f39f0.png" alt="dCSS logo" width="400" height="38">

```
<button class="dbtn dbtn-primary">Primary</button>
<button class="dbtn dbtn-secondary">Secondary</button>
<button class="dbtn dbtn-success">Success</button>
<button class="dbtn dbtn-danger">Danger</button>
```

#### Outline buttons

In need of a button, but not the hefty background colors they bring? Replace the default modifier classes with the `.dbtn-*-outlined` ones to remove colors on any button.

<img src="https://kepkuldes.com/images/58d99b6af82fe4cb38ef8a34bb8f192d.png" alt="dCSS logo" width="650" height="39">

```
<button class="dbtn dbtn-primary-outlined">Primary Outlined</button>
<button class="dbtn dbtn-secondary-outlined">Secondary Outlined</button>
<button class="dbtn dbtn-success-outlined">Success Outlined</button>
<button class="dbtn dbtn-danger-outlined">Danger Outlined</button>
```

### Embeds
If you have been around on Discord for a bit, chances are you have seen these special messages, often sent by bots. They can have a colored border, embedded images, text fields, and other fancy properties.

<img src="https://kepkuldes.com/images/5cea7c0f74de56885372a8d86e2e2f4c.png" alt="dCSS logo" width="450" height="600">

```
<div class="embed embed-primary">
    <div class="embed-heading">
            Heading
    </div>
        Description
    <div class="embed-img">
            <img src="https://res.cloudinary.com/mozilla-foundation/image/upload/c_fit,f_auto,q_70,w_736/v1587581349/foundationsite/buyersguide/discord_kjuoiq.jpg" alt="">
    </div>
    <div class="embed-footer">
          Footer
    </div>
</div>
```

Also, you can set the color of the embeds.

### Checks and radios

Create consistent cross-browser and cross-device checkboxes and radios with our completely rewritten checks component.

#### Radios

<img src="https://kepkuldes.com/images/5bd9a7c521fc3700991a882b386da379.png" alt="dCSS logo" width="650" height="195">

```
<label class="dradio">
    <input type="radio" checked="checked" name="radio">
    <span class="dcheckmark"></span>
    <span class="dradio-text">Radio 1</span>
</label>
<label class="dradio">
    <input type="radio" name="radio">
    <span class="dcheckmark"></span>
    <span class="dradio-text">Radio 2</span>
</label>
<label class="dradio">
    <input type="radio" name="radio">
    <span class="dcheckmark"></span>
    <span class="dradio-text">Radio 3</span>
  </label>
<label class="dradio">
    <input type="radio" name="radio">
    <span class="dcheckmark"></span>
    <span class="dradio-text">Radio 4</span>
</label>
```

#### Switches
Switch uses the `.dswitch` and `.dtoggle` classes to render a toggle switch.

<img src="https://kepkuldes.com/images/1df67c80bab015ec02eefee8b441925f.png" alt="dCSS logo" width="50" height="80">

```
<input type="checkbox" class="dswitch" id="switch1"/>
<label class="dtoggle" for="switch1"></label>
<input type="checkbox" class="dswitch" id="switch2"/>
<label class="dtoggle" for="switch2"></label>
```

### Select
Customize the native `<select>`s with custom CSS that changes the element's initial appearance.

#### Default
Custom `<select>` menus need only a custom class, `.dselect` to trigger the custom styles. Custom styles are limited to the `<select>`s initial appearance and cannot modify the `<option>`s due to browser limitations.

<img src="https://kepkuldes.com/images/7036a101308a738dff4dfc040a6c3ddd.png" alt="dCSS logo" width="370" height="280">

```
<select name="select" class="dselect">
    <option value="option1">Option 1</option>
    <option value="option2">Option 2</option>
    <option value="option3">Option 3</option>
</select>
```

### Range
Use our custom range inputs for consistent cross-browser styling and built-in customization.

#### Overview

Create custom `<input type="range">` controls with `.dslider`. The track (the background) and thumb (the value) are both styled to appear the same across browsers.

<img src="https://kepkuldes.com/images/9688633fc86c59df6f2fda96313c4924.png" alt="dCSS logo" width="570" height="180">

```
<input type="range" min="1" max="100" value="25" class="dslider dslider-primary">
<input type="range" min="1" max="100" value="50" class="dslider dslider-secondary">
<input type="range" min="1" max="100" value="75" class="dslider dslider-success">
<input type="range" min="1" max="100" value="100" class="dslider dslider-danger">
```


## Creator

**Brúnó Neszményi**

- <https://twitter.com/brunoneszmenyi>
- <https://github.com/freezy-0001>



## Copyright and license

Code and documentation copyright 2021–2022. Code released under the [MIT License](https://github.com/twbs/bootstrap/blob/main/LICENSE).