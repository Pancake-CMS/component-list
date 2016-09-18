# component-list

This is an element developed using Polymer for the pancake project. The main purpose of this element is to display a list of components (OPTIONAL : and their README files based in a component object). The example of component object is below.

### Installation

This element can be installed via bower.

```shell
bower install --save pancake-cms-component-list
```

### What is Component Object

As said earlier, this element uses a `component object`. The example of a `component object` is as follows.

```javascript
[
    {
        name: 'polymer',
        version: '1.6.0',
        repo: 'polymer',
        user: 'Polymer'
    },
    {
        name: 'github-readme',
        version: '0.1.0',
        repo: 'github-readme',
        user: 'Pancake-CMS'
    }
]
```

Each array object contains the ___name___ of the component along with the ___version___ number and its ___Username___ and ___Repository Name___ on Github.

## Usage

You can use the following `html` tag to use this element as just a plain list.

```html
<component-list components="[[data]]"></component-list>
```

To display this component along with a `README` section, use

```html
<component-list components="[[data]]" showcomponentinfo="true"></component-list>
```

where `data` is the `component object` defined above

### Attributes

| name | type | example value |
|------|------|---------------|
| components | Array | ___Refer section What is Component Object___ |
| showcomponentinfo | Boolean | true |

## Styling

To adjust the size of the component use the following css variable value

```css
component-list {
    --component-list--height: 700px;
}
```

The css variable `--component-list-height` with update the height of the component information section.