# Angular 7-1 SCSS/Sass Architecture

This Angular project follows the 7-1 SCSS/Sass architecture for organizing and managing styles. Below are guidelines and instructions to help you understand and work with the code.

## Angular.json Configuration

In your `angular.json` file, make the following changes under the `architect > build > options` section:

```json
"styles": ["src/styles/global/styles.scss"], // Add this line
"stylePreprocessorOptions": {
  "includePaths": ["src/styles"]
}
```

## Reset Library

This project uses pure-start as the reset library. To install it, run the following command:

```bash
npm install pure-start
```

After installation, include the reset file in your angular.json file by adding it to the styles array:
```json
"styles": [
  "pure-start/pure-start.css", // Add this line
  "src/styles/global/styles.scss", // Add this line
  "path/to/other/styles.css"
],
```

## Adding Vendors
To include vendor styles or scripts, modify the angular.json file and add them to the scripts and styles arrays.
```bash
"styles": [
  "src/styles.scss",
  "path/to/vendor/style.css"
],
"scripts": [
  "path/to/vendor/script.js"
],
```
## Layout
Add layout-related styles in the core modules of your Angular application.

## Page Stylings
Add page-specific stylings in the respective component's styling file.
