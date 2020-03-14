# Quickstart

To get started the `<MobileMenuWrapper/>` component, which detects the gestures, needs to be placed high in the dom so that it wraps the entirety of your app's content on which the gestures need to be detected. From this component you can then yield a toggle and menu component to which you can pass a block of content. An extended `<LinkTo/>` component is available which closes the menu on click.

```handlebars
<MobileMenuWrapper as |mmw|>
  <mmw.Toggle>Menu</mmw.Toggle>

  <mmw.MobileMenu as |mm|>
    <mm.LinkTo @route="index">Home</mm.LinkTo>
  </mmw.MobileMenu>
</MobileMenuWrapper>
```