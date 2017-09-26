# pandoc-eqref

*pandoc-eqref* is a simple [pandoc][] [filter][] that in effect wraps all `\eqref{...}`
and `\ref{...}` calls in `$...$`, so that they can be recognized and properly
rendered by [MathJax][].

Additionally, it also replaces the [non-breaking space][tilde] `~` in a few
common LaTeX idioms by a simple space `0x20`.

The module [`pandocfilters`][pf] is embedded as a git submodule to make it
easier to embed *this* project as a submodule elsewhere.

[pandoc]: http://pandoc.org/index.html
[filter]: http://pandoc.org/scripting.html
[MathJax]: https://www.mathjax.org/
[tilde]: https://tex.stackexchange.com/a/41268
[pf]: https://github.com/jgm/pandocfilters
