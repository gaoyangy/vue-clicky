# vue-clicky
Handy debugging function for Vue. Right click any vue component, and it will show you neatly formatted info about it in the console.

```bash
npm install --save-dev vue-clicky
```

```javascript
if (process.env.NODE_ENV === 'development') {
  import 'vue-clicky';
}
```

### Screenshot
![screenshot](https://github.com/Herteby/vue-clicky/blob/master/screenshot.png)

Currently it shows:
* The Vue component object
* Current data, props and computed properties
* Parent component. Open the parent and it will display the same info about it.

### Changes in 1.2
* With Chrome version 60+, the "class hack" that I used before to get things to display nicely is no longer necessary.
* Now uses lodash.cloneDeep to fetch all the values so that you no longer see a bunch of (...) that you have to click on.