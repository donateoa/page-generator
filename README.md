# Angular schematics Page Generator

Install by npm

    npm i --save-dev ng-page-schematics

To override the default collection, you need to add it in the angular.json file as a cli property in the main object.

    "cli": {
        "defaultCollection": "ng-page-schematics"
    }

Then in the same file, we need to provide default options, in the same way they are supplied for @angular/schematics:

    "schematics": {
        "@schematics/angular:component": {
            "style": "scss"
        },
        "ng-page-schematics:page": {
            "style": "scss"
        }
    },

Create a new page

    ng g p path-of-page
    // or
    ng generate page path-of-page

The following component will be created

- \*.page.html
- \*.page.ts
- \*.page.css
- \*.module.ts
- \*.routing.ts
- \*.spec.ts

see the list of parameter [here](src/page-generator/schema.json)
--spec=false
