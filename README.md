# Observable CLI

TODO

- ✅ statically render Markdown using markdown-it
- ✅ highlight fenced code blocks using highlight.js
- ✅ JavaScript fenced code blocks ```js
- ✅ JavaScript embedded expressions ${…}
- ✅ automatic reloading when the Markdown is edited
- ✅ viewof equivalent using Generators.input
- ✅ display errors
- vanilla Observable JavaScript
  - ✅ top-level declarations
  - ✅ unbound references (inputs)
  - ✅ awaits
  - ✅ display(…) function
  - ✅ implicit display(…) for expressions
  - ✅ better view shorthand for Generators.input(display(input))
  - ✅ top-level function declaration
  - ✅ top-level class declaration
  - ✅ top-level destructuring patterns (const [x, y] = [0, 0.10])
  - ✅ comprehensive tests for the compiler
  - ✅ static feature detection: files, databases, secrets
  - asynchronous reactive top-level assignment (let y; await; y = 1)
  - implicit declaration for unbound assignment (x = 1)
- ✅ more robust inline expressions
  - ✅ handle template strings `…` (code_inline)
  - ✅ handle backslashes (text_special)
- ✅ embedded JavaScript expressions behave like htl.html (no inspector)
- ✅ file attachments
- ✅ check that files exist before registering file attachments
- ✅ prevent parsing embedded expressions within script tags
- ✅ fix width definition when sidebar is open
- generate bootstrapped docs for the cli repo
- database clients (databases registered in YAML or observablehq.json)
- secrets (defined via environment variable?)
- proxied fetch (bypass CORS; registered in YAML or observablehq.json)
- data table display for tabular data (query results, CSV, _etc._)
- SQL fenced code blocks
- fenced code block options
  - echo to show code in output
  - output name for SQL cells
  - source database for SQL cells
- HTML fenced code blocks?
- TeX fenced code blocks?
- Graphviz/dot fenced code blocks?
- ✅ routing to different notebooks
- detect broken socket and reconnect
- detect server restart and reload
- HTTPS with self-signed certificate or something?
- show errors with line numbers on the console
- serve root (don’t assume /)
- snapshot cache
  - proxied fetch
  - database client queries
- static site generation (yarn build)
  - including file attachments
  - including database client query snapshots
  - including fetch snapshots
  - for secrets, use encrypted hash parameters?
- incremental update
  - when Markdown changes
  - when JavaScript changes (both expressions and code blocks)
  - when other live code changes (e.g., SQL, TeX)
  - when attached files change
- imports
  - ✅ dynamic imports of ES modules
  - ✅ static imports of ES modules
  - ✅ local ES modules detected as file attachments
  - ✅ parse imports from npm:module and generate the corresponding import map
  - ✅ npm packages
  - parallelize awaits when multiple static import statements
  - local Observable Markdown files
  - cloud Observable notebooks?
  - use ES module imports for recommended libraries
  - during build, download ES modules from jsDelivr
  - equivalent to version locking/integrity sha?
- standard library 2.0
  - remove deprecated features for standard library
  - Generators.asyncInput
- ✅ self-host Observable Runtime instead of jsDelivr CDN
- add tests for serverless (build) output, too
- better theme colors for highlight.js
- better logic for clearing display after invalidation
- Symbol.for("observablehq.display") for custom inspectors?
- header and footer (meta tags, last updated date)
- table of contents (right sidebar)
- ✅ parse title from first h1 and/or YAML title option
- ✅ generate title element
- ✅ cross-notebook navigation (left sidebar)
- footer has link to edit me on GitHub
- client-side search (minisearch)?
- generate preload link rel for file attachments, Plot, d3, etc.
- implicitly await ${…} expressions before calling display?
- promote img, video, audio, and picture elements to file attachments
- add rel="nofollow noindex" to external links by default
- ✅ automatic anchor links for heading elements
- themes
  - ✅ default light/dark theme
  - dashboard theme for wide layout
  - custom header and footer
