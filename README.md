[update-readmes]   Mode: rewrite — migrating to template structure...
# typescriptify-golang-structs

[![Built with Ona](https://ona.com/build-with-ona.svg)](https://app.ona.com/#https://github.com/Interested-Deving-1896/typescriptify-golang-structs)

<!-- AI:start:what-it-does -->
_Description pending._
<!-- AI:end:what-it-does -->

## Architecture

<!-- AI:start:architecture -->
_Architecture documentation pending._
<!-- AI:end:architecture -->

## Install

<!-- Add installation instructions here. This section is yours — the AI will not modify it. -->

```bash
git clone https://github.com/Interested-Deving-1896/typescriptify-golang-structs.git
cd typescriptify-golang-structs
```

## Usage


Use the command line tool:

```
tscriptify -package=package/with/your/models -target=target_ts_file.ts Model1 Model2
```

If you need to import a custom type in Typescript, you can pass the import string:

```
tscriptify -package=package/with/your/models -target=target_ts_file.ts -import="import { Decimal } from 'decimal.js'" Model1 Model2
```

If all your structs are in one file, you can convert them with:

```
tscriptify -package=package/with/your/models -target=target_ts_file.ts path/to/file/with/structs.go
```

Or by using it from your code:

```golang
converter := typescriptify.New().
    Add(Person{}).
    Add(Dummy{})
err := converter.ConvertToFile("ts/models.ts")
if err != nil {
    panic(err.Error())
}
```

Command line options:

```
$ tscriptify --help
Usage of tscriptify:
-backup string
        Directory where backup files are saved
-package string
        Path of the package with models
-target string
        Target typescript file
```

## Configuration

<!-- Document configuration options here. This section is yours — the AI will not modify it. -->

## CI

<!-- AI:start:ci -->
_CI documentation pending._
<!-- AI:end:ci -->

## Mirror chain

<!-- AI:start:mirror-chain -->
This repo is maintained in [`Interested-Deving-1896/typescriptify-golang-structs`](https://github.com/Interested-Deving-1896/typescriptify-golang-structs) and mirrored through:

```
Interested-Deving-1896/typescriptify-golang-structs  ──►  OpenOS-Project-OSP/typescriptify-golang-structs  ──►  OpenOS-Project-Ecosystem-OOC/typescriptify-golang-structs
```

Changes flow downstream automatically via the hourly mirror chain in
[`fork-sync-all`](https://github.com/Interested-Deving-1896/fork-sync-all).
Direct commits to OSP or OOC are detected and opened as PRs back to `Interested-Deving-1896`.
<!-- AI:end:mirror-chain -->

## Contributors

<!-- AI:start:contributors -->
_Contributors pending._
<!-- AI:end:contributors -->

## Origins

<!-- AI:start:origins -->
_Original project — no upstream fork._
<!-- AI:end:origins -->

## Resources

<!-- AI:start:resources -->
_No additional resource files found._
<!-- AI:end:resources -->

## License

<!-- AI:start:license -->
[Apache-2.0](https://github.com/Interested-Deving-1896/typescriptify-golang-structs/blob/master/LICENSE.txt) © 2026 [Interested-Deving-1896](https://github.com/Interested-Deving-1896)
<!-- AI:end:license -->
