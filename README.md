# hawtio-typescript

> Slush scaffolding generator for a hawtio plugin


## Getting Started

Install `slush-hawtio-typescript` globally:

```bash
$ npm install -g slush-hawtio-typescript
```

### Usage

Create a new folder for your project:

```bash
$ mkdir my-plugin
```

Run the generator from within the new folder:

```bash
$ cd my-plugin && slush hawtio-typescript
```

Once the generator is finished, run gulp to build the example plugin and run it:

```bash
$ gulp
```

The example will be at http://localhost:2772

## Some details

Typescript files will be compiled to dist/my-plugin.js.  All template files will be concatenated and added to dist/my-plugin.js, they'll be added to $templateCache in a separate angularjs module 'my-plugin-templates'.

Definition files will be compiled into the `d.ts` directory.  The build will also add all of these files into `defs.d.ts`, which then makes it *very easy* to share definitions to other typescript plugins, as other plugins just need to include the top-level defs.d.ts file and they'll import all of the definitions for code in this plugin.

## Getting To Know Slush

Slush is a tool that uses Gulp for project scaffolding.

Slush does not contain anything "out of the box", except the ability to locate installed slush generators and to run them with liftoff.

To find out more about Slush, check out the [documentation](https://github.com/klei/slush).

## Support
If you have any problem or suggestion please open an issue [here](https://github.com/hawtio/slush-hawtio-typescript/issues).

## License 

The MIT License

Copyright (c) 2014, Stan Lewis

Permission is hereby granted, free of charge, to any person
obtaining a copy of this software and associated documentation
files (the "Software"), to deal in the Software without
restriction, including without limitation the rights to use,
copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the
Software is furnished to do so, subject to the following
conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.

