## **Old overview**
Keep UI projects as clean as possible. Do not include things that are not going to be used: styles, libraries, components, etc.


### UI framework
Framework to be used: Angular. Advantages:

- Documentation.
- Community.
- Support. 
- Roadmap
- Typescript.
- Speed and Performance.
- Large size of applications.

### Angular good practices:

- Respect modular development structure.
- Adhere To Key Angular Coding Standards
  - The code should also not exceed 75 lines for each function.
  - The code should not exceed the limit of 400 lines per file.
  - There should be an empty line between imports and modules.
- Variables with constant values should be declared with ‘const.’
- Single responsibility principle: It is important to not create more than one instance of any component, directive, or service within a single file.
- Split large components into smaller sizes
- Proper utilization of lazy loading.
- Use Angular in strict mode. I think it's now the default one. This makes you have good practices and have everything typed. 
- The Angular CLI is (command-line interface tool) is welcome.
- Use the lint recommended by Angular. Currently, Angular works great with ESLint. Just running ng lint will create a basic configuration. It's recommended to install ES Lint, on visual studio code, so it shows you the error while working. This is just a suggestion, but it's mandatory to run the ng lint command every time before pushing changes to make sure everything is properly written.
- Angular encourages you to have everything up to date. It has 2 major releases per year. We should try to update the projects at least one a year.

Preferably include external libraries per UI project. 

For external libraries, if possible, selectively include the modules that are going to be used.


### UI Components

Library to be used: PrimeNG.
We need to try to solve our views with offered components by the library. 
Custom components should be placed at the project level. The idea is to avoid huge shared libraries (old common-ui for example). Also, avoid including unnecessary components by transitive. So in some cases you might have the same component implemented in two different projects. 
If we implement wrappers or composed components we need to respect the offered API by PrimeNG API. This is to avoid custom properties for very specific cases. 
We will have different components for app runtime. This means that these components can not be used in other components. External developers might use these components.


### Style
Icons: We are going to be working with the free version of font awesome and primeng.
Ideally from the builder it should be possible to configure themes. For this, you need to have variables in the color configuration.
It is forbidden to use the style tag in HTML.
For styles, we should use scss as default in every component.


### Layout
Use options offered by the library or standard ones like Bootstrap. 
Responsive support is mandatory
