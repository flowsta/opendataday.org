Open Data Day is a gathering of citizens in cities around the world to write applications, liberate data, create visualizations and publish analyses using open public data to show support for and encourage the adoption of open data policies by the world's local, regional and national governments.

You're invited. Again. The next Open Data Day will take place on Saturday, 4 March 2017.

Check <http://opendataday.org/> for public website.

## Editing / contributing

This site is built with [Lektor](https://www.getlektor.com/).

It has a bunch of [dependencies](https://github.com/okfn/opendataday/blob/master/package.json), so do an `npm install`.

Before first building the site you will need to generate some files using `grunt sass`, `grunt icons`, `grunt plugins` and `grunt icons`.

`grunt` will watch for changes to your [SCSS files](https://github.com/okfn/opendataday/tree/master/assets/scss), and also [icons](https://github.com/okfn/opendataday/tree/master/assets/icons) (see [svgstore](https://github.com/FWeinb/grunt-svgstore)).

`lektor deploy` will deploy to the gh-pages branch, putting changes live.

### TODO

#### Map

Needs to be added [here](https://github.com/okfn/opendataday/blob/master/templates/home.html#L60). Then [this line](https://github.com/okfn/opendataday/blob/master/assets/scss/_home.scss#L271) can be removed.

#### Translations

To translate the site we need to duplicate the [contents.lr](https://github.com/okfn/opendataday/blob/master/content/contents.lr) file, and save with the language code in the file name, like [contents+de.lr](https://github.com/okfn/opendataday/blob/master/content/contents%2Bde.lr).

We also need to add translations to [global-content.ini](https://github.com/okfn/opendataday/blob/master/databags/global-content.ini) and [main-nav.ini
](https://github.com/okfn/opendataday/blob/master/databags/main-nav.ini).

If we are adding new language to the site we also need to:

- Add the new language to [languages.json](https://github.com/okfn/opendataday/blob/master/databags/languages.json)
- Add the language to [project.lektorproject](https://github.com/okfn/opendataday/blob/master/project.lektorproject).

## Previous version

The previous version of the site has been moved to the [v1](https://github.com/okfn/opendataday/tree/v1) branch.
