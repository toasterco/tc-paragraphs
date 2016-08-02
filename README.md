# <tc-paragraphs\>

`tc-paragraphs`
tc-paragraphs is an element for inserting symantic paragraphs from a string 
which contains \n as line breaks. This is useful for inserting paragraph tags 
from a chunk of text from a json response.

### Sample usage

    <tc-paragraphs text="first line\nsecond line" paragraph-classnames="class-test"></tc-paragraphs>

    Exports:

    <p class="class-test">first line</p>
    <p class="class-test">second line</p>


    
    <tc-paragraphs text="first line\n\nsecond line"></tc-paragraphs>

    Exports:

    <p>first line</p>
    <span class="spacer"></span>
    <p>second line</p>


    <tc-paragraphs text="first line\nsecond line" tag-name="h1"></tc-paragraphs>

    Exports:

    <h1>first line</h1>
    <h1>second line</h1>


### Styling

`<tc-paragraphs>` provides the following custom properties and mixins for styling:

Custom property | Description | Default
----------------|-------------|----------
`--tc-paragraph` | Mixin applied to each paragraph | `{}`
`--tc-paragraph-spacer` | Mixin applied to the spacer | `{}`


## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.

## Viewing Your Application

```
$ polymer serve
```

## Building Your Application

```
$ polymer build
```

This will create a `build/` folder with `bundled/` and `unbundled/` sub-folders
containing a bundled (Vulcanized) and unbundled builds, both run through HTML,
CSS, and JS optimizers.

You can serve the built versions by giving `polymer serve` a folder to serve
from:

```
$ polymer serve build/bundled
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.
