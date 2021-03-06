---
layout: app

permalink: /nOS/
description: Discover & build the web of the future.
license: MIT

icons:
  - nOS/icons/1024x1024/nos.png

screenshots:
  - nOS/screenshot.png

authors:
  - name: nos
    url: https://github.com/nos

links:
  - type: GitHub
    url: nos/client
  - type: Download
    url: https://github.com/nos/client/releases

desktop:
  Desktop Entry:
    Name: nOS
    Comment: Discover & build the web of the future.
    Exec: AppRun
    Terminal: false
    Type: Application
    Icon: nos
    StartupWMClass: nOS
    X-AppImage-Version: 0.5.1.5970
    Categories: Utility
    X-AppImage-BuildId: 1GAuIEM8F8I87xbkX7svsfgsrKk
  AppImageHub:
    X-AppImage-Signature: no valid OpenPGP data found. the signature could not be verified.
      Please remember that the signature file (.sig or .asc) should be the first file
      given on the command line.
    X-AppImage-Type: 2
    X-AppImage-Architecture: x86_64
    X-AppImage-Payload-License: MIT

electron:
  author: nOS
  homepage: https://nos.io
  version: 0.5.1
  private: true
  main: main.js
  license: MIT
  engines:
    node: "^8.10.0 || >=9.10.0"
  dependencies:
    "@cityofzion/neon-js": 3.11.9
    "@fortawesome/fontawesome-svg-core": 1.2.12
    "@fortawesome/free-regular-svg-icons": 5.6.3
    "@fortawesome/free-solid-svg-icons": 5.6.3
    "@fortawesome/react-fontawesome": 0.1.4
    "@ledgerhq/hw-transport-node-hid": 4.18.0
    "@nosplatform/react-copy-to-clipboard": 5.0.1
    about-window: 1.12.1
    bignumber.js: 8.0.2
    classnames: 2.2.6
    coingecko-api: 1.0.2
    connected-react-router: 5.0.1
    ejs: 2.6.1
    electron-context-menu: 0.10.1
    electron-is-dev: 0.3.0
    electron-json-storage: 4.1.5
    electron-localshortcut: 3.1.0
    electron-updater: 3.2.3
    es6-promisify: 6.0.1
    file-type: 10.7.0
    format-currency: 1.0.0
    history: 4.7.2
    lodash: 4.17.11
    mime-types: 2.1.21
    node-fetch: 2.3.0
    prop-types: 15.6.2
    qrcode.react: 0.9.2
    rc-tooltip: 3.7.3
    react: 16.7.0
    react-click-outside: 3.0.1
    react-dom: 16.7.0
    react-is: 16.7.0
    react-redux: 5.1.1
    react-router-dom: 4.3.1
    react-scroll: 1.7.10
    react-sticky: 6.0.3
    recharts: 1.4.2
    recompose: 0.30.0
    redux: 3.7.2
    redux-saga: 0.16.2
    redux-thunk: 2.3.0
    sifter: 0.5.3
    source-map-support: 0.5.10
    spunky: 1.3.1
    switch-tree: 0.2.2
    uuid: 3.3.2
    what-input: 5.1.3
    whatwg-url: 7.0.0
  jest:
    testMatch:
    - "**/__tests__/**/*.test.js"
    setupFiles:
    - "./__tests__/setupTests.js"
    - jest-canvas-mock
    setupTestFrameworkScriptFile: "./__tests__/setupFramework.js"
    transform:
      "^.+\\.jsx?$": babel-jest
    moduleNameMapper:
      "^.+\\.svg$": "<rootDir>/__mocks__/svgMock.js"
      "^.+\\.(css|scss|less)$": identity-obj-proxy
    moduleDirectories:
    - node_modules
    coverageDirectory: "./coverage/"
    collectCoverage: true
---
