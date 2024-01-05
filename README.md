# Angular 7-1 SCSS/Sass Architecture

This Angular project follows the 7-1 SCSS/Sass architecture for organizing and managing styles. Below are guidelines and instructions to help you understand and work with the code.

## Angular.json Configuration

In your `angular.json` file, make the following changes under the `architect > build > options` section:

```json
"stylePreprocessorOptions": {
  "includePaths": ["src/styles"]
}
```

## Reset Library

This project uses pure-start as the reset library. To install it, run the following command:

```bash
npm install pure-start
```
