## PLUGINS & EXTENSIONS

Nadesiko3 has a plugin system. Plugins are divided into built-in and external.

### Built-in Plugins

**plugin_system** - Core system functions

- Time/date, type conversions, JSON, random, math, strings, arrays

**plugin_browser** - DOM manipulation (browser only)

- HTML elements, events, canvas, AJAX, local storage

**plugin_node** - File system & OS (Node.js only)

- File I/O, directory operations, process execution

**plugin_turtle** - Turtle graphics

- Drawing commands, coordinate system

### External Plugins

Install via npm:

```bash
# Web server (Express)
npm install nadesiko3-server

# WebSocket
npm install nadesiko3-websocket

# Excel file manipulation
npm install nadesiko3-office

# SQLite3
npm install nadesiko3-sqlite3

# Command-line tools
npm install nadesiko3-tools

# MeCab (Japanese morphological analysis)
npm install nadesiko3-mecab

# HTML parsing/scraping
npm install nadesiko3-htmlparser

# Machine learning
npm install nadesiko3-ml

# Database connectors
npm install nadesiko3-odbc
npm install nadesiko3-mysql
npm install nadesiko3-postgresql
npm install nadesiko3-mssql
```

### Using Plugins

```nadesiko
# Import a plugin
!「nadesiko3-sqlite3」を取り込む

# Use plugin commands
「test.db」をSQLite開く
```

### Creating Custom Plugins

Create `myplugin.mjs`:

```javascript
export default {
  'meta': {
    type: 'const',
    value: {
      pluginName: 'plugin_custom',
      description: 'My custom plugin',
      pluginVersion: '1.0.0',
      nakoRuntime: ['wnako', 'cnako'],
      nakoVersion: '3.6.0'
    }
  },
  'カスタム関数': {
    type: 'func',
    josi: [['を'], ['と']],
    fn: function(a, b, sys) {
      return a + b;
    }
  }
}
```

Use it:

```nadesiko
!「./myplugin.mjs」を取り込む
5を10とカスタム関数して表示  # Output: 15
```
