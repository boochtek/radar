Web
===

* Build on top of other services
    * [Split](https://www.split.io/) - feature flags as a service
* [Quasar](https://quasar-framework.org/) - framework to build cross-platform web apps
    * Server-rendered, SPA, progressive, mobile (Cordova), Electron
    * Uses Vue
* Optimizations (from https://github.com/thedaviddias/Front-End-Performance-Checklist)
    * Don't need `type` attribute for CSS and JS references in HTML 5
    * Always reference CSS before JavaScript
    * Use Font Squirrel to ensure WOFF 2.0 font files
    * Use `<link rel="preconnect" href="https://other.site" crossorigin>` to pre-fetch DNS
    * Use `async` or `defer` on JS references
        * Use `async` if the script don't rely on other scripts
        * Use `defer` if the script relies upon or is relied upon by an async script
* Benchmarking web server performance
    * [wrk](https://github.com/wg/wrk)
* Metrics
    * Record number of times each page is hit (and by whom)
        * Because then you'll know if you can get rid of an unused page
        * Do this as early as possible
* Auth
    * Auth0
    * Google Auth
    * Okta
