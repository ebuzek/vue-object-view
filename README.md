## vue-object-view

> Vue.js component for displaying arbitrary JavaScript values (supporting circular references)

See the [live demo](http://emanuelbuzek.eu/vov-demo/) to try it out. *([demo app](https://github.com/ebuzek/vue-object-view-demo) on github)*

## About
The main purpose of this component is to display complex JavaScript values that may contain **circular references**. The component renders the value as a *tree* that can be manually expanded to display nested values.

The experience is very similar to inspecting JavaScript objects using the browser developer tools. The component was created to build the in-browser **JavaScript debugger** for the [PARAPPLE](http://emanuelbuzek.eu/parapple/#/) project.

## Usage
```bash
# Install the component
npm install --save vue-object-view
```

Use it just like any other Vue.js component. The value to display is passed as `v-model`.

```html
<VueObjectView v-model="object" />
```
