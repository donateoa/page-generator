# Angular schematics Page Generator

## Install by npm

    npm i --save-dev ng-page-schematics

## Create a new page

    ng generate ng-page-schematics:page name-of-page --spec=false

Will create the following component

- \*.page.html
- \*.page.ts
- \*.page.css
- \*.module.ts
- \*.routing.ts
- \*.spec.ts

and update the parent routing that contains the key `routes`;

see the list of parameter [here](src/page-generator/schema.json)
--spec=false
