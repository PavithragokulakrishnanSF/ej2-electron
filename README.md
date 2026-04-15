# Electron application

Repository Description: Electron sample demonstrating integration of Syncfusion EJ2 Grid with a webpack-based build and Electron runtime.

## Project Overview

This repository contains a minimal Electron application that uses webpack to bundle a renderer process which includes the Syncfusion JavaScript Grid control. The example shows how to wire Syncfusion components into an Electron renderer, run the app locally, and produce a distributable bundle.

## Features

- Renderer bundled with webpack including Syncfusion EJ2 Grid
- Simple Electron main/renderer setup for desktop testing
- Instructions for installing dependencies and running locally

## Prerequisites

- Node.js v14.15.0 or higher
- npm or yarn
- Basic familiarity with Electron and webpack

For more details on Electron + Syncfusion setup see: https://ej2.syncfusion.com/development/documentation/getting-started/electron/

## Install

Install dependencies in the project root:

```bash
npm install
```

## Run (development)

Start the application in development mode:

```bash
npm start
```

This launches Electron and loads the webpack-built renderer. Watch the console for the port or local file used by the renderer.

## Build / Package

To produce a production bundle, run your configured webpack build (see `webpack.config.js`) or use any packaging script provided in `package.json`.

## How it works

Webpack compiles the renderer sources and outputs assets that Electron's renderer process loads. The Electron main process launches the window that points to the bundled renderer HTML. This keeps the application code modular while allowing desktop deployment.
