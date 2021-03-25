# Module Bundler im Frontend - das Warum und Wie.

## Konzepte

- Wofür benötigt man Module Bundler?
- Wie laden Webbrowser traditionell Assets?
- Abhängigkeiten auflösen:

  - manuell
    - https://pbs.twimg.com/media/CkjFUyTXEAEysBY.jpg
    - script Tags
    - globaler Namespace - IIFE
  - Tool-gestützt (browserify, webpack ...)
  - ES Module https://caniuse.com/es6-module
  - Extremfall: buildless https://buildless.site/

  ## Aufgaben eines Module Bundlers heute

  - Abhängigkeiten auflösen (dependency tree)
  - Transpilieren (transpile)
    - Typescript
    - Babel
    - SASS, PostCSS
  - Dateien bündeln (bundle)
  - Statische Assets (z.B. Bilder) verwalten
  - Development Tooling für den Entwickler
    - dev server (möglichst schnell)
    - source maps
    - Codeanalyse (Linter)
  - Optimierungen, meistens für Produktion
    - minification
    - tree shaking
    - code splitting
    - dynamische Importe
    - optimierte Builds für moderne und legacy Browser
    - Sicherheit verbessern, z.B. https://developer.mozilla.org/en-US/docs/Web/Security/Subresource_Integrity
    - Bauen einer PWA automatisieren (ServiceWorker erstellen, Manifest + Icons generieren ...)
