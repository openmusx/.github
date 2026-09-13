# openmusx

Open-source tools for reading Finale `.musx` files and converting their contents
to open music notation formats.

Finale has been discontinued. These projects exist so that musicians, engravers,
and developers can continue to access their own scores and move them to other
software. Everything here reads Finale files; nothing writes them.

**This organization is not affiliated with or endorsed by Finale or its parent
company.** The projects contain no Finale source code and do not circumvent copy
protection on the Finale application. They were developed by analyzing the
EnigmaXML content of `.musx` files and other publicly available resources.

## Projects

| Repository | What it does |
| --- | --- |
| [denigma](https://github.com/openmusx/denigma) | Command-line converter and C++ libraries. Converts MUSX to MusicXML, MNX, EnigmaXML, MSS, and SVG. Also builds a WebAssembly module. [Docs](https://openmusx.github.io/denigma/) |
| [denigma-online](https://github.com/openmusx/denigma-online) | Static website that runs the Denigma WebAssembly module entirely in the browser. Your files never leave your machine. [Try it](https://denigma.robertgpatterson.com/) |
| [musxdom](https://github.com/openmusx/musxdom) | C++17 document object model for EnigmaXML, the format inside `.musx` archives. The foundation the other projects build on. [Docs](https://openmusx.github.io/musxdom/) |
| [smufl-mapping](https://github.com/openmusx/smufl-mapping) | C++ lookup tables for SMuFL glyph names, codepoints, and metadata, including mappings from legacy Finale music fonts. Bundled Bravura font data is under the SIL Open Font License. |
| [denigma-examples](https://github.com/openmusx/denigma-examples) | Standalone native and WebAssembly examples showing how to consume the Denigma libraries from your own CMake project. |

## Getting started

- **Just want to convert a file?** Use [Denigma Online](https://denigma.robertgpatterson.com/) in your browser, or download a `denigma` release for the command line.
- **Building a tool?** Start with [musxdom](https://openmusx.github.io/musxdom/) for direct access to the document model, or link the [denigma libraries](https://openmusx.github.io/denigma/) for ready-made conversion.

## Contributing

Bug reports with a sample `.musx` file are the most useful thing you can send.
Open an issue on the relevant repository. Pull requests are welcome.

Projects are MIT licensed unless a repository states otherwise.

## Related

MNX support is built on [mnxdom](https://github.com/mnx-works/mnxdom) from the
[mnx-works](https://github.com/mnx-works) organization.
