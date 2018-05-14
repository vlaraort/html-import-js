# html-import-js

Small library, to import HTML webcomponents inside a JS ES6 file.

## Getting started

1. Add html-import-js to your project:

    ```npm i -S html-import-js```

2. Require the function

```js
    import { importHref } from 'html-import-js';
```    

3. Use it to require a HTML compomemt

```js
    importHref ('./bower_components/paper-input/paper-input.html');
```    

## Parameters

```importHref``` supports 4 parameters:

```href, onload, onerror, optAsync```

| Parameter | Description |
| --- | --- |
`href` | The relative url of the html file
`onload` |  Callback to notify when an import successfully loaded
`onerror` | Callback to notify when an import unsuccessfully loaded.
`optAsync` | True if the import should be loaded `async`, Defaults to `false`.

## Disclaimer

All this code is taken from the Polymer library, as they removed this functionality in the polymer 3 version,
this library allows to use it again