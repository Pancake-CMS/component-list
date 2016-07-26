# component-list

This is an element developed using Polymer for the pancake project. The main purpose of this element is to display a list of components and their README files based in a component object. The example of component object is below.

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

You can use the following `html` tag to use this element

```html
<component-list components="[[data]]"></component-list>
```

where `data` is the `component object` defined above

### Attributes

| name | type | example value |
|------|------|---------------|
| components | Array | ___Refer section What is Component Object___ |