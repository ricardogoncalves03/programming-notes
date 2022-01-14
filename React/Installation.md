# React + Router
---
Website: https://create-react-app.dev/docs/getting-started/


## Installing create-react-app

```bash
npx create-react-app <project_name>

cd <project_name>

npm start
```

If you got an error such as:

```bash
You are running `create-react-app` 4.0.3, which is behind the latest release (5.0.0).

We no longer support global installation of Create React App.
```

Try running this first:

```bash
npx clear-npx-cache
```
source: https://stackoverflow.com/questions/70358643/you-are-running-create-react-app-4-0-3-which-is-behind-the-latest-release-5-0

If you got several errors during installation, such as:

```bash
npm ERR! code ERR_SOCKET_TIMEOUT
npm ERR! errno ERR_SOCKET_TIMEOUT
npm ERR! network Invalid response body while trying to fetch https://registry.npmjs.org/@types%2fhtml-minifier-terser: Socket timeout
npm ERR! network This is a problem related to network connectivity.
npm ERR! network In most cases you are behind a proxy or have bad network settings.
npm ERR! network 
npm ERR! network If you are behind a proxy, please make sure that the
npm ERR! network 'proxy' config is set properly.  See: 'npm help config'
```

Try to clean npm cache first:
```
npm cache clean --force
```

# React-router
```bash
npm install react-router-dom
```
