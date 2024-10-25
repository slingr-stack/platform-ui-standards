## **Old overview**
Ensure UI projects only contain essential elements. Ensure UI projects only contain essential elements and avoid including unused styles, libraries, components, etc.

### UI framework

**Framework to be used: Angular**.

### Advantages:
- Comprehensive documentation
- Community support
- Extensive roadmap
- TypeScript integration
- Speed and performance optimization
- Large-scale applications

### Best practices for Angular:

- Respect modular development structure.
- Adhere to key Angular coding standards:
  - Limit code to 75 lines per function.
  - Limit files to a maximum of 400 lines of code.
  - Leave an empty line between imports and modules.
- Variables with constant values should be declared with `const.`
- Apply the **Single Responsibility Principle:** Do not create more than one instance of any component, directive, or service within a single file.
- Split large components into smaller sizes.
- Proper utilization of lazy loading.
- Enable strict mode in Angular (this is now the default) to enforce good practices and ensure everything is typed.
- Use the Angular CLI (Command-Line Interface tool).
- Use the lint recommended by Angular. Angular works great with ESLint. Running `ng lint` will create a basic configuration. It’s recommended to install ESLint in Visual Studio Code to show errors while working. This is just a suggestion, but it’s mandatory to run `ng lint` before pushing changes to ensure everything is properly written.
- Angular encourages you to stay up to date. With two major releases per year, updating projects at least once annually is recommended.
- Preferably, include external libraries per UI project. Only import the necessary modules to reduce bundle size and improve performance.

### UI Components

**Library to be used: PrimeNG**. 

We should try to solve our views with the components provided by the library. 

- Place custom components at the project level to avoid large shared libraries (e.g., the old common-ui).
Also, avoid including unnecessary components by transitive dependencies. In some cases, the same component might be implemented in two different projects.
- When creating wrappers or composed components, we need to respect the API offered by PrimeNG. This helps avoid custom properties for very specific cases.
- Designate specific components for application runtime, which should not be reused in other components. These components are also available for external developers.

### Style

**Icons**: We will work with the free version of Font Awesome and PrimeNG.
Ideally, the builder should allow theme configuration, achieved by including variables in the color configuration.

- Avoid using the <style> tag directly in HTML; instead, prefer SCSS for all styling needs.
- SCSS should be the default styling approach in every component.

### Layout

Use options provided by the library or standard ones like Bootstrap.
Responsive design support is mandatory.
