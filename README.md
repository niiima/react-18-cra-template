# Introducing React 18

> React 18 is now available on npm!

This React App is created using of the official CRA template by default with version 18. For more information you can visit:

- [Create React App](https://github.com/facebook/create-react-app).
- [React 18 Blog](https://reactjs.org/blog/2022/03/29/react-v18.html "React v18.0 March 29, 2022 by The React Team")
- [How to Upgrade to React 18](https://reactjs.org/blog/2022/03/08/react-18-upgrade-guide.html "A gradual adoption strategy for existing applications")
## Out-of-the-box improvements
React 18 will include out-of-the-box improvements:

- [Automatic batching for fewer renders](https://github.com/reactwg/react-18/discussions/21 "Automatic batching for fewer renders in React 18")
- [SSR support for Suspense](https://github.com/reactwg/react-18/discussions/22 "Upgrading to React 18 on the server")
- [Fixes for Suspense behavior quirks](https://github.com/reactwg/react-18/discussions/7 "Behavioral changes to Suspense in React 18")

## Upgrade to React 18
For client apps, upgrading to React 18 is straightforward:

Upgrade to the latest React 18 release
Switch to the [New root API](https://github.com/reactwg/react-18/discussions/5 "Replacing render with createRoot")

> Note: React 18 is a major version of React. As any major version will have, there are semantic changes that may impact your app

    // Before
	import { render } from 'react-dom';
	const container = document.getElementById('app');
	render(<App tab="home" />, container);

	// After
	import { createRoot } from 'react-dom/client';
	const container = document.getElementById('app');
	const root = createRoot(container);
	root.render(<App tab="home" />);''
	

## Troubleshooting
If the app is significantly broken after switching to `createRoot`, see if you have `<StrictMode>` on. If you do, try removing it and see if that fixes it. If it does, a library you're using (or, less likely, you app code) is not compatible with Strict Effects.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)