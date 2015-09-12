TableFilter [![Build Status](https://api.travis-ci.org/koalyptus/TableFilter.svg?branch=master)](https://travis-ci.org/koalyptus/TableFilter)
===========================

> A Javascript library making HTML tables filterable

TableFilter is a modernised version of the [HTML Table Filter generator](http://tablefilter.free.fr) javascript plugin.
This library adds to any html table a "filter by column" feature that enables
users to filter and limit the data displayed within a long table. By default, the script automatically adds a filter grid bar at the top of the desired table.

## Features
* Convert a regular HTML table into an advanced grid component providing:
    * Advanced columns filtering model
    * Sorting and pagination facilities
    * Complete selection model ([ezEditTable](http://codecanyon.net/item/ezedittable-enhance-html-tables/2425123) extension)
    * Extended keyboard navigation ([ezEditTable](http://codecanyon.net/item/ezedittable-enhance-html-tables/2425123) extension)
    * Inline cell or row editing ([ezEditTable](http://codecanyon.net/item/ezedittable-enhance-html-tables/2425123) extension)
    * Row insertion or deleting ([ezEditTable](http://codecanyon.net/item/ezedittable-enhance-html-tables/2425123) extension)
    * And even more behaviors...
* Attach to an existing HTML table
* Integration with any server-side technology as this is a pure client-side
solution
* Callbacks for all events, and delegates for most actions
* Exhaustive documentation and API
* Valuable support provided under a Premium request

## Getting started
Clone the repo using Git:
```shell
git clone --bare https://github.com/koalyptus/TableFilter.git
```

Alternatively you can [download](https://github.com/koalyptus/TableFilter/archive/master.zip) this repository.

## Setup
Copy the ``tablefilter`` directory under ``dist`` and place it at desired location in your project. Then include the main js file in your page:
```shell
<script src="path/to/my/scripts/tablefilter/tablefilter.js"></script>
```
Place the following snippet just under the HTML table and always define a ``base_path`` property in the configuration object to reflect the path to the script
```shell
<script>
var tf = new TableFilter('my-table-id', {
    base_path: 'path/to/my/scripts/tablefilter/'
});
tf.init();
</script>
```
If the ``base_path`` property is not specified, it will default to ``/tablefilter`` directory:
```shell
your-page.html
 |— tablefilter
``` 

## Development
This project requires node.js and Grunt to be installed:
- install [node.js](https://nodejs.org/)
- install [Grunt](http://gruntjs.com/getting-started) from the command line using npm (comes with node.js):
```shell
npm install -g grunt-cli
```
Once ``Grunt`` is sorted out you can follow the instructions below.
Start by installing any dependencies.

```shell
npm install
```
Use the Grunt ``dev`` task to launch a build / watch cycle and start the local
sever on port ``8080``:

```shell
grunt dev
```

Use the ``build`` task to generate a production build:

```shell
grunt build
```

The ``default`` Grunt task will create a production build, run the tests and finally generate the demos:

```shell
grunt
```

To run all the tests:

```shell
grunt test
```

and to run specific test(s):

```shell
grunt test-only:test.html
grunt test-only:test.html,test-sort.html
```

## Demos
Check out the online [examples](http://koalyptus.github.io/TableFilter/examples) or run the local webserver:
```shell
grunt server
```
then pick a demo from:
```shell
http://localhost:8080/demos/
```

## Documentation
Find exhaustive documentation on the configuration options in the [WIKI](https://github.com/koalyptus/TableFilter/wiki) section.

Autogenerated documentation of the ES6 javascript modules is available on the website: [docs](http://koalyptus.github.io/TableFilter/docs)

Run this task to generate the documentation in the ``docs/docs`` directory:
```shell
grunt esdoc
```


## Support
* GitHub for reporting bugs and feature requests.

## License
[MIT](LICENSE.md)





