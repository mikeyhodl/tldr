# zipgrep

> Find patterns in files in a Zip archive using extended `regex` (supports `?`, `+`, `{}`, `()` and `|`).
> More information: <https://manned.org/zipgrep>.

- Search for a pattern within a Zip archive:

`zipgrep "{{search_pattern}}" {{path/to/file.zip}}`

- Print file name and line number for each match:

`zipgrep {{[-H|--with-filename]}} {{[-n|--line-number]}} "{{search_pattern}}" {{path/to/file.zip}}`

- Search for lines that do not match a pattern:

`zipgrep {{[-v|--invert-match]}} "{{search_pattern}}" {{path/to/file.zip}}`

- Specify files inside a Zip archive from search:

`zipgrep "{{search_pattern}}" {{path/to/file.zip}} {{file/to/search1}} {{file/to/search2}}`

- Exclude files inside a Zip archive from search:

`zipgrep "{{search_pattern}}" {{path/to/file.zip}} {{[-x|--line-regexp]}} {{file/to/exclude1}} {{file/to/exclude2}}`
