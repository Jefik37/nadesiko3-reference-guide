## RUNNING PROGRAMS

### cnako3 Command Options

```bash
# Execute a .nako3 file
cnako3 program.nako3

# Execute one-liner code
cnako3 -e "「Hello World」と表示"

# Compile to JavaScript (output to file)
cnako3 -o output.js program.nako3

# The -o option was fixed in v3.6.43
```

**Note**: Based on documentation, cnako3 primarily supports `-e` for one-liners. Other flags may be limited compared to full-featured CLI tools.

### Browser Execution

**Method 1: CDN**

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <script src="https://nadesi.com/v3/cdn.php?v=3.6.0"></script>
</head>
<body>
  <script type="なでしこ">
    「Hello from Browser」を表示
  </script>
</body>
</html>
```

**Method 2: Local Build**
Use `npm start` in the nadesiko3 repository to start a local web server with the editor.

### File Extensions

- `.nako3` - Nadesiko3 source files (current version)
- `.nako` - Legacy Nadesiko v1 files (NOT compatible with v3)
