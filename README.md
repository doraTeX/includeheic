# includeheic.sty

A LaTeX package that extends `\includegraphics` to support HEIC images on macOS (requires shell-escape).

## Overview

This package adds functionality to `\includegraphics` to support HEIC images on macOS. Internally, this package automatically converts HEIC images to JPEG, which provides seamless support for HEIC images in LaTeX.

## Requirements

* Uses macOS's native `sips` command for image conversion, so it's macOS only
* Requires `-shell-escape` for external command execution

## Usage

Simply include the package and use `\includegraphics` with HEIC files as you would with any other image format:

```tex
\usepackage{includeheic}
\begin{document}
\includegraphics{your-image.heic}
\end{document}
```

Remember to compile your document with the `-shell-escape` option enabled.

## More Details

See [my blog post (in Japanese)](https://doratex.hatenablog.jp/entry/20250415/1744706568).

## License

This package is provided under the [LaTeX Project Public License](https://www.latex-project.org/lppl/).

## Author

[Yusuke Terada](https://github.com/doraTeX)