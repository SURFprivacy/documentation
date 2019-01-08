# privacy.surf.nl

## 1. hugo-surf-theme
### 1.1 folder structure
```
theme
├── images
├── layouts
│   ├── _default
│   |   └── single.html
│   ├── partials
│   |   ├── head.html
│   |   ├── header.html
│   |   ├── navigation.html
│   |   └── footer.html
│   ├── 404.html
│   └── index.html
├── static
│   ├── css
│   |   └── main.css
│   ├── fonts
│   ├── images
│   └── js
├── LICENSE.md
├── README.md
└── theme.toml
```

### 1.2 layout
```
> HEAD
> HEADER/NAVIGATION
> PAGE CONTENT
> FOOTER
```

### 1.3 requirements
#### 1.3.1 General
Speed, efficiency, accessibility, privacy and security are important aspects of privacy.surf.nl.

* No useless code will be used.
* No (other) framework will be used.
* All code follows best coding practices and conventions.
* All code has easy-to-read and usable comments.
* The theme works on all widely used operating systems/browsers. At least:
    * Chromium / Chrome
    * Firefox / Quantum
    * Opera
    * Vivaldi
    * Internet Explorer
    * Microsoft Edge
    * Safari
    * Mobile browsers Android

#### 1.3.2 CSS
* There is only one file (`main.css`).
* The CSS file only contains entries that are really used.
* The CSS is responsive on different screen formats and resolutions.

#### 1.3.3 JS
* Will be kept to a absolute minimum.
* The theme and website is fully functional without javascript.

#### 1.3.4 Resources
* No external resources will be used.
* No options or references for or to external resources (CDN's, trackers etc.) will exist.
* fonts will be locally hosted.
* css will be locally hosted.
* html will be locally hosted.
* js will be locally hosted.
* images will be locally hosted.

#### 1.3.5 Features
* All features are usable with basic syntax in content files. For additional features (outside default Markdown) easy to use syntax will be used.
* The standard GitHub-flavoured markdown features
    * headers / header underline
    * emphasis (bold, italic, strikethrough, combinations)
    * lists (ordered and unordered)
    * links
    * images
    * code
    * tables
    * blockquotes
    * horizontal rule
* [Accordion](https://en.wikipedia.org/wiki/Accordion_(GUI))
* [Accordion](https://en.wikipedia.org/wiki/Accordion_(GUI)) (nested)
* [Tabs](https://en.wikipedia.org/wiki/Tabbed_interface)
* [Tabs](https://en.wikipedia.org/wiki/Tabbed_interface) (nested)
* Expansion tab
* Expansion tab (nested)
* Privacy overview block

#### 1.3.6 Hugo
* Hugo asset minification is possible.

#### 1.3.7 Webserver
* Uses strong TLS configuration.
* Uses restrictive security headers.
* Exclusively static serving.
* OS is hardened.
* SSH is hardened and not exposed the the internet.
* OS has incoming and outgoing firewall.
