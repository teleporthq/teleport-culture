## What is this?
A set of guidelines and practices we gathered along the way that ensure that our codebases are clean and consistent. We don't pretend that these are best practices in any way, but we prefer to adhere to a standard way of writing, organizing and structuring code.

Most of the rules can be enforced by tooling, hence we have a strict working environment from this perspective:
* We use **prettier** to format code with a standard configuration
* We use **eslint** to enforce additional rules in TypeScript/JavaScript
* We have a standard **tsconfig** across all projects
* We are relying on a **precommit-hook** to validate all the rules before each git commit

Further details about the setup can be studied in our starter pack (link coming soon). In the following sections, we have lists of practices which cannot be enforced by tooling and which are under continuous improvement

### TypeScript

* Relevant **constants** (eg: SCREEN_WIDTH) should be extracted and named with UPPER_SNAKE_CASE
* Split the class/functions definition and the type definition into `index.ts` and `types.ts` in a folder with the name of the module/component
* Classes should implement Interfaces to avoid importing the class export directly in other files when only the type is needed.
* **Default exports** should rarely (if not never) be used. **Named exports** ensure consistent naming and [favor tree-shaking](https://blog.neufund.org/why-we-have-banned-default-exports-and-you-should-do-the-same-d51fdc2cf2ad)
* **Fail fast** - put the finish conditions for a function first and don't indent the whole function body if possible
* When creating a type, don't use optional/undefined and null for the same field. The field is either **optional** "?" OR **nullable**
* Dependency Injection - coming soon

### React
coming soon

### Node
coming soon

### CSS
* styled-jsx split
