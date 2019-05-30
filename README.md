# `<myuw-drawer> and <myuw-drawer-link>`

A three-part slide out navigation drawer for use with the MyUW App Bar. Includes drawer, links, and optional subheaders with dividers.

## Development and contribution

To run the demo app locally and test the component, run the following commands:

```bash
$ npm install
$ npm start
```

## Getting Started

Add the following imports to your page's `<head>`:

```html
<script type="module" src="https://unpkg.com/@myuw-web-components/myuw-drawer@^1?module"></script>
<script nomodule src="https://unpkg.com/@myuw-web-components/myuw-drawer@^1"></script>
```

## Using the component

* Include script tag for component.
* Add custom html tag

```html
<myuw-drawer>
  <myuw-drawer-link
    slot="myuw-drawer-links"
    name="MyUW home"
    icon="mail"
    href="http://google.com">
  </myuw-drawer-link>
  <myuw-drawer-subheader
    slot="myuw-drawer-links"
    name="Subheader"
    divider>
  </myuw-drawer-subheader>
  <myuw-drawer-link
    slot="myuw-drawer-links"
    name="Browse apps"
    icon="explore"
    href="http://google.com">
  </myuw-drawer-link>
</myuw-drawer>
```

### Configuration / child components for the drawer

Use the named `<slot>` tags to include child components of the myuw-drawer:

**Available slots:**
- **myuw-drawer-links**: Insert the `<myuw-drawer-link>` or `<myuw-drawer-subheader>` component

### Drawer link configurable attributes

- **name:** Set the text of the link component
- **icon:** The name of a Material icon to appear next to the link
- **href:** The the URL of the link

### Subheader configurable attributes

- **name:** Set the text of the subheader
- **divider:** Display a dividing line above the subheader (will display if attribute is present, no value required)


Cross-browser testing provided by:<br/>
<a href="https://www.browserstack.com/"><img width="160" src="https://myuw-web-components.github.io/img/Browserstack-logo.svg" alt="BrowserStack"/></a>
