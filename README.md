# i3lockmore

<div align="center"><img src="https://raw.githubusercontent.com/SammysHP/i3lockmore/readme-assets/i3lockmore.png" /></div>

This is a wrapper for i3lock that adds additional functionality:

<dl>
    <dt>--pixelate [scalefactor]</dt>
    <dd>
        <p>Uses the pixelated screen content as the background of the lockscreen.</p>
        <p>The optional value "scalefactor" controls the size of the pixels. A value
        of 1 results in large pixels while a value of 100 has no effect.
        (It scales down the background to "scalefactor" percent of the original
        screen content).</p>
    </dd>
    <dt>--grayscale</dt>
    <dd>
        <p>Convert the background into grayscale. Requires --pixelate.</p>
    </dd>
    <dt>--resize-image /path/to/image</dt>
    <dd>
        <p>simply use a big image and resize it to the current screen size</p>
    </dd>
    <dt>--dpms timeout</dt>
    <dd>
        <p>Uses DPMS to turn the screen off after "timeout" seconds of inactivity.</p>
        <p>CAUTION: This sets --nofork (see "man i3lock") to restore the previous
        value of the DPMS timeout after the screen was unlocked.</p>
    </dd>
</dl>

All other arguments are passed to i3lock.


## Installation

### Dependencies

Following programs must be installed:

- i3lock
- bash
- imagemagick
- xset

### Package

There is a package available for Arch Linux in the [PKGBUILD branch](https://github.com/SammysHP/i3lockmore/tree/PKGBUILD) of this repository.


## License

MIT License

Copyright (c) 2016 Sven Karsten Greiner

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
