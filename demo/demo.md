# Button

The Auro Design System fully supports a wide range of buttons styles and use cases. The following examples illustrate common button uses followed up by code examples.

See [install instructions](https://www.alaskaair.com/components/auro/button/install) for more information as how to install and full API for the `auro-button` Auro base element.

Illustrated in this example is a stand-alone use of `auro-button`.

## Button use cases

The `auro-button` element should be used in situations where users may:

* submit a form
* begin a new task
* trigger a new UI element to appear on the page
* specify a new or next step in a process

## Buttons are not Hyperlinks

In cases were the action of the button would not fit the criteria above, it is most likely a Hyperlink. In that situation it is recommended that the [auro-hyperlink](https://www.alaskaair.com/components/auro/hyperlink) element be used.

## Default types

<div class="exampleWrapper">
  <auro-button>Primary</auro-button>
  <auro-button disabled>Primary</auro-button>
</div>

<auro-accordion lowProfile justifyRight>
  <span slot="trigger">See code</span>

  ```html
  <auro-button>Primary</auro-button>
  <auro-button disabled>Primary</auro-button>
  ```

</auro-accordion>

<div class="exampleWrapper">
  <auro-button secondary>Secondary</auro-button>
  <auro-button secondary disabled>Secondary</auro-button>
</div>

<auro-accordion lowProfile justifyRight>
  <span slot="trigger">See code</span>

  ```html
  <auro-button secondary>Secondary</auro-button>
  <auro-button secondary disabled>Secondary</auro-button>
  ```

</auro-accordion>

<div class="exampleWrapper">
  <auro-button tertiary>Tertiary</auro-button>
  <auro-button tertiary disabled>Tertiary</auro-button>
</div>

<auro-accordion lowProfile justifyRight>
  <span slot="trigger">See code</span>

  ```html
  <auro-button tertiary>Tertiary</auro-button>
  <auro-button tertiary disabled>Tertiary</auro-button>
  ```

</auro-accordion>

For default spacing of elements in a row, use the [.auro_containedButtons](https://alaskaairlines.github.io/WebCoreStyleSheets/#utility-auro-css-#{$scope}.auro_containedButtons) predefined selector in the [WC Style Sheets](https://auro.alaskaair.com/webcorestylesheets) lib.

<div class="exampleWrapper auro_containedButtons">
  <auro-button>Primary</auro-button>
  <auro-button secondary>Secondary</auro-button>
  <auro-button tertiary>Tertiary</auro-button>
</div>

<auro-accordion lowProfile justifyRight>
  <span slot="trigger">See code</span>

  ```html
  <div class="exampleWrapper auro_containedButtons">
    <auro-button>Primary</auro-button>
    <auro-button secondary>Secondary</auro-button>
    <auro-button tertiary>Tertiary</auro-button>
  </div>
  ```

</auro-accordion>

## Icon support

Adding icons to the auro-button component is as easy as nesting any other HTML. The [auro-icon component](https://www.alaskaair.com/components/auro/icon) has access to all the icons listed in the [Auro Icons library](https://www.alaskaair.com/icons/usage) for quick and easy use.

Be sure to use the `customColor` attribute on the auro-icon component to allow colors set in your parent element to pass through to the icon.


<div class="exampleWrapper auro_containedButtons">
  <auro-button>
    Activate WiFi
    <auro-icon customColor category="in-flight" name="wifi"></auro-icon>
  </auro-button>

  <auro-button secondary>
    <auro-icon customcolor category="interface" name="arrow-left"></auro-icon>
    Previous action
  </auro-button>

  <auro-button tertiary>
    Love this ...
    <auro-icon customcolor category="interface" name="heart-filled"></auro-icon>
  </auro-button>
</div>

<auro-accordion lowProfile justifyRight>
  <span slot="trigger">See code</span>

  ```html
  <auro-button>
    Activate WiFi
    <auro-icon customColor category="in-flight" name="wifi"></auro-icon>
  </auro-button>

  <auro-button secondary>
    <auro-icon customcolor category="interface" name="arrow-left"></auro-icon>
    Previous action
  </auro-button>

  <auro-button tertiary>
    Love this ...
    <auro-icon customcolor category="interface" name="heart-filled"></auro-icon>
  </auro-button>
  ```

</auro-accordion>

## Auro Button - fluid

<div class="exampleWrapper">
  <auro-button fluid>Primary</auro-button>
  <auro-button secondary fluid>Secondary</auro-button>
  <auro-button tertiary fluid>Tertiary</auro-button>
</div>

<auro-accordion lowProfile justifyRight>
  <span slot="trigger">See code</span>

  ```html
  <auro-button fluid>Primary</auro-button>
  <auro-button secondary fluid>Secondary</auro-button>
  <auro-button tertiary fluid>Tertiary</auro-button>
  ```

</auro-accordion>

## Auro Button - onDark

<div class="exampleWrapper--ondark auro_containedButtons">
  <auro-button ondark>Primary</auro-button>
  <auro-button ondark disabled>Primary</auro-button>
</div>

<auro-accordion lowProfile justifyRight>
  <span slot="trigger">See code</span>

  ```html
  <auro-button ondark>Primary</auro-button>
  <auro-button ondark disabled>Primary</auro-button>
  ```

</auro-accordion>

<div class="exampleWrapper--ondark auro_containedButtons">
  <auro-button secondary ondark>Secondary</auro-button>
  <auro-button secondary ondark disabled>Secondary</auro-button>
</div>

<auro-accordion lowProfile justifyRight>
  <span slot="trigger">See code</span>

  ```html
  <auro-button secondary ondark>Secondary</auro-button>
  <auro-button secondary ondark disabled>Secondary</auro-button>

  ```

</auro-accordion>

<div class="exampleWrapper--ondark auro_containedButtons">
  <auro-button tertiary ondark>Tertiary</auro-button>
  <auro-button tertiary ondark disabled>Tertiary</auro-button>
</div>

<auro-accordion lowProfile justifyRight>
  <span slot="trigger">See code</span>

  ```html
  <auro-button tertiary ondark>Tertiary</auro-button>
  <auro-button tertiary ondark disabled>Tertiary</auro-button>

  ```

</auro-accordion>

## Auro Button - pass function to button

<div class="exampleWrapper auro_containedButtons">
  <auro-button onclick="alert('YOU CLICKED ME!');">Primary</auro-button>
  <auro-button disabled onclick="alert('YOU CLICKED ME!');">Primary</auro-button>
</div>

<auro-accordion lowProfile justifyRight>
  <span slot="trigger">See code</span>

  ```html
  <auro-button onclick="alert('YOU CLICKED ME!');">Primary</auro-button>
  <auro-button disabled onclick="alert('YOU CLICKED ME!');">Primary</auro-button>

  ```

</auro-accordion>
