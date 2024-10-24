## **Old Overview**
Keep UI projects as clean as possible. Do not include things that are not going to be used: styles, libraries, components, etc.

### UI Framework
Framework to be used: Angular. Advantages:
- Documentation
- Community
- Support
- Roadmap
- TypeScript
- Speed and performance
- Large size of applications

### Angular Good Practices:

- Respect modular development structure.
- Adhere to key Angular coding standards:
  - The code should not exceed 75 lines per function.
  - The code should not exceed 400 lines per file.
  - There should be an empty line between imports and modules.
- Variables with constant values should be declared with `const.`
- **Single Responsibility Principle:** Do not create more than one instance of any component, directive, or service within a single file.
- Split large components into smaller sizes.
- Proper utilization of lazy loading.
- Use Angular in strict mode (it’s now the default). This enforces good practices and ensures everything is typed.
- The Angular CLI (Command-Line Interface tool) is recommended.
- Use the lint recommended by Angular. Angular works great with ESLint. Running `ng lint` will create a basic configuration. It’s recommended to install ESLint in Visual Studio Code to show errors while working. This is just a suggestion, but it’s mandatory to run `ng lint` before pushing changes to ensure everything is properly written.
- Angular encourages you to stay up to date. It has 2 major releases per year. We should aim to update projects at least once a year.

Preferably, include external libraries per UI project.

For external libraries, selectively include the modules that will be used.

### UI Components

Library to be used: PrimeNG.
We should try to solve our views with the components provided by the library. 

Custom components should be placed at the project level. The goal is to avoid large shared libraries (e.g., the old `common-ui`). Also, avoid including unnecessary components by transitive dependencies. In some cases, the same component might be implemented in two different projects.

If we implement wrappers or composed components, we need to respect the API offered by PrimeNG. This helps avoid custom properties for very specific cases.

We will have different components for app runtime. These components should not be used in other components. External developers may use these components.

### Style
Icons: We will work with the free version of Font Awesome and PrimeNG.
Ideally, the builder should allow theme configuration. To achieve this, variables must be present in the color configuration.

It is forbidden to use the `<style>` tag in HTML.

For styles, SCSS should be the default in every component.

### Layout
Use options provided by the library or standard ones like Bootstrap.
Responsive support is mandatory.
