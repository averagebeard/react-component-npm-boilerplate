# React Component `npm` Boilerplate

## Setup

```bash
git clone git@github.com:averagebeard/react-component-npm-boilerplate.git
```

## Usage

In `package.json` change:

-   name
-   repository
-   author

and update `keywords` to accurately reflect your package.

Install any dependencies you need.

Fill out the `src` directory with code for your component.

### Testing Locally

```bash
yarn build
# the build will now exist in lib

yarn link
# your package is now locally linked
```

In another terminal window, `cd` to the project/app you want to test your package. In the new window run:

```bash
yarn link <your_package_name>
# your package is now linked in your app
# you can view it in your app's node_modules folder
```

You can now import your project as though it were installed as a dependency.

### Live Updating

If you want live updates of your package that you've linked to your app, run your app and in your package terminal run:

```bash
yarn build:watch
```

Every change made to your package will now live update in your app.

### Deploying to `npm`

In your package terminal run:

```bash
yarn publish
```

You will get a series of responses from `npm` with the final response reading:

```bash
+ <your_package_name>@<current_version>
```

Make sure that you update the version of your package in your `package.json` every time you publish. Follow [npm's guide](https://docs.npmjs.com/about-semantic-versioning) to versioning to best align your package with `npm`.
