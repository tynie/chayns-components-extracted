# CodeHighlighter

**Package:** `@chayns-components/code-highlighter` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { CodeHighlighter } from '@chayns-components/code-highlighter';

const Component: FC = () => {
    const code = `console.log("TEST")`;

    return <CodeHighlighter code={code} language="typescript" />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `code` | `string` | ✓ | The code that should be displayed. |
| `copyButtonText` | `string` |  | The text that should be displayed after the copy button. If not set, just the button is displayed without text. |
| `highlightedLines` | `HighlightedLines` |  | The lines of code that should be highlighted. Following lines can be highlighted: added, removed and just marked. |
| `language` | `CodeHighlighterLanguage` | ✓ | The language of the displayed code. |
| `onFormatError` | `(error: unknown) => void` |  | Function to be executed when the formatting of the code fails. |
| `shouldFormatCode` | `boolean` |  | Whether the code should be formatted with prettier. |
| `shouldShowLineNumbers` | `boolean` |  | Whether the line numbers should be displayed. |
| `shouldWrapLines` | `boolean` |  | Whether long lines should be wrapped. |
| `theme` | `CodeHighlighterTheme` |  | The theme of the code block. Decide between dark and light. |

## Types

### CodeHighlighterLanguage

```typescript
"" | "abap" | "abnf" | "actionscript" | "ada" | "agda" | "al" | "antlr4" | "apacheconf" | "apex" | "apl" | "applescript" | "aql" | "arduino" | "arff" | "asciidoc" | "asm6502" | "asmatmel" | "aspnet" | "autohotkey" | "autoit" | "avisynth" | "avroIdl" | "bash" | "basic" | "batch" | "bbcode" | "bicep" | "birb" | "bison" | "bnf" | "brainfuck" | "brightscript" | "bro" | "bsl" | "c" | "cfscript" | "chaiscript" | "cil" | "clike" | "clojure" | "cmake" | "cobol" | "coffeescript" | "concurnas" | "coq" | "cpp" | "crystal" | "csharp" | "cshtml" | "csp" | "cssExtras" | "css" | "csv" | "cypher" | "d" | "dart" | "dataweave" | "dax" | "dhall" | "diff" | "django" | "dnsZoneFile" | "docker" | "dot" | "ebnf" | "editorconfig" | "eiffel" | "ejs" | "elixir" | "elm" | "erb" | "erlang" | "etlua" | "excelFormula" | "factor" | "falselang" | "firestoreSecurityRules" | "flow" | "fortran" | "fsharp" | "ftl" | "gap" | "gcode" | "gdscript" | "gedcom" | "gherkin" | "git" | "glsl" | "gml" | "gn" | "goModule" | "go" | "graphql" | "groovy" | "haml" | "handlebars" | "haskell" | "haxe" | "hcl" | "hlsl" | "hoon" | "hpkp" | "hsts" | "html" | "http" | "ichigojam" | "icon" | "icuMessageFormat" | "idris" | "iecst" | "ignore" | "inform7" | "ini" | "io" | "j" | "java" | "javadoc" | "javadoclike" | "javascript" | "javastacktrace" | "jexl" | "jolie" | "jq" | "jsExtras" | "jsTemplates" | "jsdoc" | "json" | "json5" | "jsonp" | "jsstacktrace" | "jsx" | "julia" | "keepalived" | "keyman" | "kotlin" | "kumir" | "kusto" | "latex" | "latte" | "less" | "lilypond" | "liquid" | "lisp" | "livescript" | "llvm" | "log" | "lolcode" | "lua" | "magma" | "makefile" | "markdown" | "markupTemplating" | "markup" | "matlab" | "maxscript" | "mel" | "mermaid" | "mizar" | "mongodb" | "monkey" | "moonscript" | "n1ql" | "n4js" | "nand2tetrisHdl" | "naniscript" | "nasm" | "neon" | "nevod" | "nginx" | "nim" | "nix" | "nsis" | "objectivec" | "ocaml" | "opencl" | "openqasm" | "oz" | "parigp" | "parser" | "pascal" | "pascaligo" | "pcaxis" | "peoplecode" | "perl" | "phpExtras" | "php" | "phpdoc" | "plsql" | "powerquery" | "powershell" | "processing" | "prolog" | "promql" | "properties" | "protobuf" | "psl" | "pug" | "puppet" | "pure" | "purebasic" | "purescript" | "python" | "q" | "qml" | "qore" | "qsharp" | "r" | "racket" | "reason" | "regex" | "rego" | "renpy" | "rest" | "rip" | "roboconf" | "robotframework" | "ruby" | "rust" | "sas" | "sass" | "scala" | "scheme" | "scss" | "shellSession" | "smali" | "smalltalk" | "smarty" | "sml" | "solidity" | "solutionFile" | "soy" | "sparql" | "splunkSpl" | "sqf" | "sql" | "squirrel" | "stan" | "stylus" | "swift" | "systemd" | "t4Cs" | "t4Templating" | "t4Vb" | "tap" | "tcl" | "textile" | "toml" | "tremor" | "tsx" | "tt2" | "turtle" | "twig" | "typescript" | "typoscript" | "unrealscript" | "uorazor" | "uri" | "v" | "vala" | "vbnet" | "velocity" | "verilog" | "vhdl" | "vim" | "visualBasic" | "warpscript" | "wasm" | "webIdl" | "wiki" | "wolfram" | "wren" | "xeora" | "xmlDoc" | "xojo" | "xquery" | "yaml" | "yang" | "zig"
```

### CodeHighlighterTheme

```typescript
{ Light = "light", Dark = "dark" }
```

### HighlightedLines

```typescript
{ added?: Array; removed?: Array; marked?: Array; }
```

