Loewenstark_Head
============================================================

This module adds a version tag to JS/CSS files in HTML header, so that browsers properly reload changed asset files like Stylesheets and JavaScripts.

Before:
```javascript
<link rel="stylesheet" type="text/css" href="https://www.demo.de/js/example.css" />
```

After:
```javascript
<link rel="stylesheet" type="text/css" href="https://www.demo.de/js/example.css?v2" />
```

# Howto raise the version tag
**Optimal:** Use a setup script in your project module and change the system config variable (Path: design/head/meta_version_tag)
**Manually:** Backend > System > Configuration > Design > HTML Head > "Version Tag for JS/CSS Files in Header"

# Module not working?
Check for rewrites of block class `page/html_head` (`Mage_Page_Block_Html_Head`)
