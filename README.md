# windows-polish-keyboard-layout-with-working-tilde
This repository contains keyboard layout with modified "Polish (programmers)" to contain working tilde

Microsoft in its infinite wisdom decided to make the tilde key on the Polish keyboard layout useless.

This repository contains a modified version of the Polish (programmers) keyboard layout that removes "dead key" functionality from the tilde key, making it suitable for development.

## Installation

Download the msi installer and dll, run the installer.

## Usage

After installing, go to Settings -> Time and Language -> Language and region -> <click ellipsis on your desired language> -> Language options -> Add keyboard -> "Polish (programmers) - tilde"

## Additional information

### Code signing

DLLs and installers are signed with my personal certificate, so you can be sure that they are not malicious.

The setup.exe is not, because for some reason signtool complains it is not a correct PE32 file. [PE Bear](https://github.com/hasherezade/pe-bear) disagrees. You are not required to use setup.exe.

### ARM64 support

I don't know about arm64 support, msklc generates ia64, but not arm64 ¯\_(ツ)_/¯.

There is some recent information about it here: https://learn.microsoft.com/en-us/answers/questions/2151451/microsoft-keyboard-layout-creator-(msklc)-for-wind, but I haven't pursued it.

## Contributing

I do not expect anyone to contribute to this repository. Feel free to fork it and make your own changes.

To build, you will need MSKLC 1.4: https://www.microsoft.com/en-us/download/details.aspx?id=102134

Source file for the layout is included, but you can easily recreate it by loading the "Polish (programmers)" keyboard, selecting "Shift state", selecting the tilde key, then removing "Dead key?" from the properties.

## License

Copyright (c) 2025 Michał Janiszewski

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
