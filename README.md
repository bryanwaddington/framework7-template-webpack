<em>**I have updated this repo to the latest package versions in order to add to an existing project, without the changes and understanding required to use framework7-cli.**</em>

# Framework7 Webpack App Template

A full-featured Framework7 with Webpack setup with hot-reload.

## Usage

### 1. Download this repository
```
git clone https://github.com/framework7io/framework7-template-webpack my-app
```

Repository will be downloaded into `my-app/` folder

### 2. Instal dependencies

Go to the downloaded repository folder and run:
```
npm install
```

This will download latest version of Framework7 and required icon fonts (to `/src/fonts/`)

### 3. Run the app

```
npm run dev
```

App will be opened in browser at `http://localhost:8080/`

### 4. Build app for production

```
npm run build-prod
```

The output will be at `www/` folder

## Use with cordova
Cordova is not enabled by default, so make sure to remove the comment tags around the `<script src="cordova.js"></script>` line in [projectroot]/src/index.html
```
<body>
  <div id="app"></div>

  <!-- Cordova -->

  <script src="cordova.js"></script>

  <!-- built script files will be auto injected -->
</body>
```
It will be added during the build process to Android/iOS.

Just put the contents of `www` folder in your cordova's project root `www` folder

## One command install

```
git clone https://github.com/framework7io/framework7-template-webpack my-app &&
cd my-app &&
npm install &&
npm run dev
```

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for development
npm run build-dev

# build for production with minification
npm run build-prod
```

## Project Structure

* `src/index.html` - main app HTML
* `src/assets` - folder with static assets (images)
* `src/css` - put custom app CSS styles here. Don't forget to import them in `main.js`
* `src/pages` - app `.f7.html` pages
* `src/app.js` - main app file where you include/import all required libs and init app
* `src/routes.js` - app routes
* `/static/` - folder with extra static assets that will be copied into output folder
