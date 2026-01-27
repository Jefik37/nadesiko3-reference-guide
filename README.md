# Nadesiko3 Complete Reference Guide

**Nadesiko3** is a Japanese programming language that compiles to JavaScript/TypeScript. It runs in browsers, Node.js, and any environment where JavaScript can execute.

**Official Site**: https://nadesi.com/  
**GitHub**: https://github.com/kujirahand/nadesiko3  
**License**: MIT

Made with AI, take it with a grain of salt.

---

## TABLE OF CONTENTS

1. [Installation](01_installation.md)
2. [Running Programs](02_running-programs.md)
3. [Core Syntax](03_core-syntax.md)
4. [Data Types](04_data-types.md)
5. [Operators](05_operators.md)
6. [Control Flow](06_control-flow.md)
7. [Functions](07_functions.md)
8. [String Operations](08_string-operations.md)
9. [File I/O](09_file-io.md)
10. [DOM/Web Features](10_dom-web-features.md)
11. [Advanced Features](11_advanced-features.md)
12. [Built-in Commands](12_built-in-commands.md)
13. [Plugins & Extensions](13_plugins--extensions.md)
14. [Complete Examples](14_complete-examples.md)
15. [Tips & Best Practices](15_tips--best-practices.md)
16. [Common Pitfalls](16_common-pitfalls.md)
17. [Standard Library Reference](17_standard-library-reference.md)

---

## RESOURCES

### Official

- Main Site: https://nadesi.com/
- Documentation: https://nadesi.com/v3/doc/
- Tutorial: https://nadesi.com/v3/doc/go.php?997
- GitHub: https://github.com/kujirahand/nadesiko3
- npm: https://www.npmjs.com/package/nadesiko3

### Community

- Discord: https://discord.com/invite/WkaQAxbDaE
- Issues: https://github.com/kujirahand/nadesiko3/issues

### Learning

- Online Editor: https://nadesi.com/v3/start
- Program Storage: https://n3s.nadesi.com/
- Examples: https://github.com/kujirahand/nadesiko3/tree/master/demo

### Related Projects

- Nadesiko3 Deno: https://github.com/kujirahand/nadesiko3deno
- Nadesiko3 PHP: https://github.com/kujirahand/nadesiko3php
- Nadesiko3 Electron: https://github.com/kujirahand/nadesiko3electron
- Nadesiko3 WebKit: https://github.com/kujirahand/nadesiko3webkit

---

## VERSION HISTORY

### Major Versions

- **Nadesiko v1** (2005-2017) - Windows only, Delphi-based
- **Nadesiko v3** (2017-present) - Cross-platform, JavaScript/TypeScript

### v3.x Notable Changes

- **v3.0.x** (2017) - Initial release with custom parser
- **v3.1.5** (2018) - Inline indent support (`:`)
- **v3.2.1** (2020) - Async function support, ESModule structure
- **v3.3.x** (2022) - Migration to TypeScript
- **v3.4.19** (2023) - BigInt support
- **v3.4.21** (2023) - Async file operations
- **v3.6.x** (2024) - Plugin API overhaul, esbuild adoption
- **v3.6.2** (2024) - Variable management: Object → Map
- **v3.6.21** (2024) - Multi-loop 対象/回数 restoration
- **v3.6.41** (2024) - MAX, MIN, CLAMP functions added
- **v3.6.43** (2025) - Fixed `-o` option for cnako3
- **v3.7.1** (2025) - Boolean values: 0/1 → true/false
- **v3.7.2** (2025) - **Major**: Unicode surrogate pair fixes (emoji handling)
- **v3.7.3** (2025) - **Breaking**: 足す changed to numeric only; added 合計
- **v3.7.4** (2025) - 配列要素作成 accepts arrays
- **v3.7.7** (2025) - 文字始まる/文字終わる commands, TOML plugin
- **v3.7.8** (2025) - Fixed 尋ねる command input bug after 20k lines
- **v3.7.9** (2025) - Canvas API 描画クリップ added, JSON inline indent fixes
- **v3.7.10** (2025) - Camera auto-cleanup, 数列判定 empty string handling
- **v3.7.11** (2025) - テーブル更新 header fix, array+object property syntax
- **v3.7.12** (2025) - Discord link updated, audio error messages improved
- **v3.7.13** (2025) - ファイル命令 fixes, DOM和属性 property reflection fix

### Breaking Changes

- **v3.6.2**: Variable management changed (Object → Map)
- **v3.7.1**: Boolean representation (0/1 → true/false)
- **v3.7.2**: String length calculations may differ (emoji now 1 char)
- **v3.7.3**: 足す command now numeric only (use 連結 for strings)

---

## QUICK REFERENCE

```
# Comments: # // /* */
# Variables: name = value OR name は value
# Output: 表示(value) OR valueを表示
# If: もし condition ならば ... 違えば ... ここまで
# Loop: N回 ... ここまで OR arrayを反復 ... ここまで
# Function: ●(args)nameとは ... valueで戻る ここまで
# Array: arr=[1,2,3] Access: arr[0] or arrの0
# Dict: obj={「key」:value} Access: objの「key」
# String: 「text」or "text" Interpolation: 「{variable}」
# Execute: cnako3 file.nako3
# One-liner: cnako3 -e "code"
```

---

**Based on**: Nadesiko3 v3.7.13 documentation and release notes
