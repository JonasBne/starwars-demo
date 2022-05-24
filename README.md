# State Proof of Concept with React Query and Jotai

The purpose of this PoC is to create a demo application that uses React Query to handle server side state and Jotai to handle client side state.
Please note that I deliberately stored certain information in 'global state' for the sake of the example. The main idea of this application is that 
React Query and Jotai can perfectly work together in a React application.

## Verdict

### Pro

- Easy to use
- State is globally accessible without having to think about providers or consumers
- Syntax is similar to React useState (which in turns makes it easier to use)
- Documentation is clear
- Adoption of Jotai is increasing
- Jotai offers out of the box support for React Query (although in this demo I did not encounter a use case for it)

### Cons
- State is globally accessible (hence, state can be accessed an updated from any component)
- It provides less structure than other libraries (e.g. Redux)

In the end I would argue that the pros outweigh the cons. The combination between React Query and Jotai works great and is very easy to use.
It also forces the developer to think critically about state in general and where it belongs (i.e. client or server side state, should it be made globally available or not).


## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).
