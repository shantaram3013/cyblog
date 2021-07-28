# cyblog

Cybernetically enhanced static site generation.

### Installing

You'll need `deno` installed. Then:

```
$ git clone https://github.com/shantaram3013/cyblog
$ cd cyblog
$ make install
```

### Usage

Cyblog operates on either single pages or entire directories, converting the
Cyblog markup into HTML.

[Read the spec](SPEC.md) to learn more about Cyblog markup!

You can invoke Cyblog with:

```
cyblog {SOURCEDIR|SOURCEFILE.cyblog} [options]
```

#### Options:

- `-o`, `--output` The name of the output directory or file.\
  If this is not supplied, Cyblog will use a name from:
  - `SOURCEFILE-dist.html` (in case of a file)
  - `SOURCEDIR-dist` (in case of a directory)
- `-a`, `--apply-style` The name of a stylesheet to include into the final
  document that will be built. Functions the same as the `apply-style`
  declaration.

### Contributing

Feel free to fork the repo and open a PR. Cyblog is written in TypeScript and
all documentation is written in Markdown.

### License

```
The MIT License (MIT)

Copyright © 2021 Siddharth Singh

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the “Software”), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
of the Software, and to permit persons to whom the Software is furnished to do
so, subject to the following conditions:
    * The above copyright notice and this permission notice shall be included
    in all copies or substantial portions of the Software.
THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Acknowledgements

`getConfigDir()` taken from https://github.com/justjavac/deno_data_dir under the
MIT license. Copyright © justjavac.
