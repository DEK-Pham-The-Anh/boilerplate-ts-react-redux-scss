# DEV GUIDE

## Basic setup

1. Install the basic TypeScript React skleleton `npx create-react-app _YOUR_PROJECT_NAME_ --template typescript`
    - If you get an error like this: `npm ERR! Could not install from "_YOUR_SYSTEM_USERNAME_\AppData\Roaming\npm-cache\_npx\19748" as it does not contain a package.json file.`, it means your `_YOUR_SYSTEM_USERNAME_` contains spaces. To solve this problem, execute `npm config set cache "C:\_YOUR_PATH_\_YOUR_SYSTEM_MODIFIED_USERNAME_\AppData\Roaming\npm-cache" --global`, where `_YOUR_SYSTEM_MODIFIED_USERNAME_` is your system username containing `~1` instead of spaces.
2. Install Redux with TS type definitions `npm install --save redux @types/redux`
3. Install React-Redux `npm install --save react-redux @types/react-redux`
4. Install Sass support `npm install --save sass`

## Project structure

When it comes to app's `src` directory, it's recommended to use superior Angular-like structure i.e. something like this:
```
- /src
    - /components
        - /ComonentName
            - index.scss
            - index.test.tsx
            - index.tsx
    - /styles
        - base.scss
        - index.scss
        - layout.scss
    - /images
        - logo.svg
    - index.tsx
    - setupTests.ts
```