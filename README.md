# enlive-selector-from-css

Tiny CSS parser to translate CSS selectors like
`div.big ul:last-of-type input.xyz[type=text]` into selector vectors
like `[:div.big [:ul html/last-of-type] [:input.xyz (html/attr= :type "text")]`,
as used by [Enlive](https://github.com/cgrand/enlive).

No guarantees of robustness or usefulness are provided.
For such concerns, use a mature CSS parsing library — it won't
guarantee anything either, but that's the way it goes.

This has mostly been a practice exercise in Clojure (parsing, quoting)
and regexes, which keep you young or something, or at least regular.

## License

Copyright (c) 2015 Ben Cook
Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted, provided that the above copyright notice and this permission notice appear in all copies.
THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
