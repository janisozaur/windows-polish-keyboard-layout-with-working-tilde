# windows-polish-keyboard-layout-with-working-tilde
[This repository](https://github.com/janisozaur/windows-polish-keyboard-layout-with-working-tilde) contains keyboard layout with modified "Polish (programmers)" to contain working tilde

Microsoft in its infinite wisdom decided to make the tilde key on the Polish keyboard layout useless.

This repository contains a modified version of the Polish (programmers) keyboard layout that removes "dead key" functionality from the tilde key, making it suitable for development.

## Installation

Download the dll for your architecture, place it in `%SystemRoot%\System32` and import `pl-tilde.reg`.

See https://learn.microsoft.com/en-us/answers/questions/2151451/microsoft-keyboard-layout-creator-(msklc)-for-wind for more information.

## Usage

After installing, go to Settings -> Time and Language -> Language and region -> &lt;click ellipsis on your desired language&gt; -> Language options -> Add keyboard -> "Polish (programmers) - tilde"

## Additional information

### Code signing

DLLs and installers are signed with my personal certificate, so you can be sure that they are not malicious.

### ARM64 support

msklc generates ia64, but not arm64 ¯\\\_(ツ)\_/¯.

I followed steps outlined in https://learn.microsoft.com/en-us/answers/questions/2151451/microsoft-keyboard-layout-creator-(msklc)-for-wind to create arm64 version (not ARM64EC). Other versions were created with msklc itself.

### Changes to the layout

See repository history for changes to the source files, especially commit e519565.

## Contributing

I do not expect anyone to contribute to this repository. Feel free to fork it and make your own changes.

To build, you can use MSKLC 1.4: https://www.microsoft.com/en-us/download/details.aspx?id=102134

Alternatively, you can use the source code in this repository. There is GitHub Actions workflow that builds the DLLs for you.

Source file for the layout is included, but you can easily recreate it by loading the "Polish (programmers)" keyboard, selecting "Shift state", selecting the tilde key, then removing "Dead key?" from the properties.

## License

Copyright (c) 2025 Michał Janiszewski

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
