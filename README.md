# Minimal Electron + React + Typescript Starter Kit

This is a fork from [basic-electron-react-boilerplate](https://github.com/pbarbiero/basic-electron-react-boilerplate)

I download that repo and change javascript to typescript. It changes a lot and the git has missing, so I create a new repo, not just fork from that repo.

### To get started:

```
yarn && yarn build
```

##### Development
* Run `yarn dev` to start webpack-dev-server. Electron will launch automatically after compilation.

##### Production
_You have two options, an automatic build or two manual steps_

###### One Shot
* Run `yarn package` to have webpack compile your application into `dist/bundle.js` and `dist/index.html`, and then an electron-packager run will be triggered for the current platform/arch, outputting to `builds/`

###### Manual
_Recommendation: Update the "postpackage" script call in package.json to specify parameters as you choose and use the `yarn add package` command instead of running these steps manually_
* Run `yarn build` to have webpack compile and output your bundle to `dist/bundle.js`
* Then you can call electron-packager directly with any commands you choose

If you want to test the production build (In case you think Babili might be breaking something) after running `yarn build` you can then call `yarn prod`. This will cause electron to load off of the `dist/` build instead of looking for the webpack-dev-server instance. Electron will launch automatically after compilation.


