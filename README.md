# Angular Material Starter Website

This project helps evelopers to get started with building websites with [Angular](https://angular.io/) using [Material Design](https://material.io/).

![angular-material-starter-website-preview](https://user-images.githubusercontent.com/902972/84209324-822e6780-aa7b-11ea-825e-336820947cda.png)

# Why?

Angular comes with several tools, but one part that misses is a sample website. Although the team leaves on developers to build sites.

1. The `ng new <project>` command does create all the boilerplate code but does not come with a sample website and related components, page structure. 

2. The other complexity with Angular is that it being an opiniated framework, files and directories need to be in certain specific structure.

3. There are not many active starter projects that has a pre-built sample website built with Angular and using only Material design components. There are several such projects exist but most of them use some 3rd party framework or addtional code to build the website.

# What's Included

The project has a sample website home page with:
- Header
- Left sidebar
- Body
  - Split into a grid
- Footer

# Architecture

## Technical Stack
The project is built with the following:

### Angular
Angular is an application design framework and development platform for creating efficient and sophisticated single-page apps.

### Material Design components for Angular
Material design is one of the most used design systems and Angular team also has developed a comprehensive list of Angular components using Material, called as the "Material Design Components for Angular". 

## Key Wirings Angular with Material

- `<project-root>`
  - `<project-root>/package.json` 
    - Includes 
      `"@angular/cdk": "^9.2.4"` and `"@angular/material": "^9.2.4"`
  - `<project-root>/angular.json`
    - Includes the default layout as 
      ```
       "styles": [
        "./node_modules/@angular/material/prebuilt-themes/deeppurple-amber.css",
        "src/styles.scss"
       ],
      ```
- `<project-root>/src/`
  - `<project-root>/src/styles.scss`
    - Includes the default styles used across the project.
  - `<project-root>/src/index.html`
    - Is the primary binding file for Angular projects. The key to observe here is the usage of Material typography.

      `<body class="mat-typography">`
- `<project-root>/src/app`
   - `<project-root>/src/app/app.routing.module.ts` primary routing module for the project. 
   - `<project-root>/src/app/app.component.html` primary entry html file that has all code for building the website.
   - `<project-root>/src/app/app.component.scss` empty.
   - `<project-root>/src/app/app.component.ts` primary component, also includes `MatSideNav`.
   - `<project-root>/src/app/app.module.ts` primary module. Also incudes only required material components.

# Build

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Production

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

# Contribute

I started this as an Open Source by Default project and will always be free.

We'd love your contribution and appreciate it. We need support to make this a bigger, better project. Of all be more helpful to users.
