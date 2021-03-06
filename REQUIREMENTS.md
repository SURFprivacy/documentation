# Requirements privacy.surf.nl
------------------------------
## 0. General project requirements
### 0.1 Transparancy
* The privacy documentation of SURF is transparent to the public.
* The rights of data subjects are transparent and easily invoked.
* All SURF privacy related information is easily accessible on one website.

### 0.2 Control
* All content and information is exclusively and directly controlled by the responsible privacy officer(s).
* All content mutations/changes will be transparently and safely (no later manipulation) recorded. In this case git (specifically GitHub) is being used for this.
* In the future, the GitHub can easily be swapped out by another git wrapper with similar properties. Most Content Management Systems (like Wordpress, Drupal, Joomla etc.) don't have a true Version Control System and are no fitting replacement to this.
* All content mutations/changes can be managed (only) by the responsible privacy officer(s).

### 0.3 Personal data
* The website does not contain *any* tracker or other privacy narrowing technologies. Data subjects should be able to receive all SURF privacy related information without giving up personal data.
* The website only logs personal data that is strictly neccesary for the purpose of the transparent information provision about privacy at SURF. This means that limited logging of for example (parts of) IP addresses for ensuring the availability and/or security of the website would be proportional, but that no other information will be logged.

### 0.4 Social responsibility
* All creations (logo's, trademarks, icons etc. are excluded) will be open source/free software.
* All code will be easily reusable by others, for example to create their own transparent privacy register or to improve upon.

---------------------
## 1. Hugo-surf-theme
### 1.1 Folder structure
The folder structure is open for debate.
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

### 1.2 Layout
The lay-out is open for debate.
```
> HEAD
> HEADER/NAVIGATION
> PAGE CONTENT
> FOOTER
```

### 1.3 Look and feel
* The styling follows the house theme of surf.nl.
* Different menu/header layouts are used throughout surf.nl, the one we choose is shared with the developer.
* The styling on surf.nl is followed as closely as possible.

### 1.3 Requirements
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
* There is only one file (i.e. `main.css`).
* The CSS file only contains entries that are really used.
* The CSS is responsive on different screen formats and resolutions.

#### 1.3.3 JS
* Will be kept to a absolute minimum.
* The theme and website is fully functional without javascript. This requirement may bite with `1.3.5`'s elements like accordions, expansion tabs etc. The proper fix can be discussed after it has been deemed impossible or too hard.

#### 1.3.4 Resources
* No external resources will be used.
* No options or references for or to external resources (CDN's, trackers etc.) will exist.
* fonts will be locally hosted.
* css will be locally hosted.
* html will be locally hosted.
* js will be locally hosted.
* images will be locally hosted.

#### 1.3.5 Page features
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

#### 1.3.6 Menu header
* Submenu functionality
* Search functionality with pre-defined tags that link to a specific part of a page.

#### 1.3.7 Picture header
* Header image can be added to page (after menu header, before content)

#### 1.3.8 Footer
* Footer supports configurable links (internal and external).

#### 1.3.9 Hugo
* Hugo asset minification is possible.

---------------
## 2. webserver
### 2.1 Requirements
* Compatible with general purpose webservers like Apache and Nginx.
* Uses strong TLS configuration.
* Uses restrictive security headers.
* Exclusively static serving.
* OS is hardened.
* SSH is hardened and not exposed the the internet.
* OS has incoming and outgoing firewall.
