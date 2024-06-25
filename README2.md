Introduction:
- Contact List allows users to add their contacts as a backup incase something goes wrong with their phone. They can also delete unneeded contacts.

Features:
- Create contacts and input information via modal
- Delete contacts

Technologies Used:
- HTML
- CSS
- JavaScript
- React
- React Router
- Context

Requirements:
- Make sure you are using node version 10

1. Install the packages:
```
$ npm install
```
2. Create a .env file:
```
$ cp .env.example .env
```
3. Start coding! And the webpack dev server with live reload, for Windows, Mac, Linux or Gitpod:

```bash
$ npm run start
```

Styles:
- You can update the `styles/index.css` or create new `.css` files inside `styles/` and import them into your current scss or js files depending on your needs.

Components:
- Add more files into your `./src/js/components` or styles folder as you need them and import them into your current files as needed.

**Note (New changes)**: Components have been converted into functions to support the use of hooks:
- Instead of a class component, we're using a `const` function.
- Class `constructor` and `state` have been replaced by `useState()` hooks.
- `componentDidMount()` was replaced by `useEffect({}, [])` - It runs at mount thanks to the second parameter (`[]`).
- `Actions` and `Store` still work the same way.

```jsx
// Previous "Class Oriented"
export class Demo extends React.Component {
	constructor(props) {
		super(props);

		this.state = getState('code here');
	}
}

// New "Functional Oriented"
export const Demo = () => (
	const [state, setState] = getState('code here'); //using the state (if needed)
  const { store, actions } = useContext(Context); // using the context (if needed)

);
```

Note: There is an example using the Context API inside `views/demo.js`;

Views (Components):
- Add more files into your `./src/js/views` and import them in `./src/js/layout.jsx`.

Contributors:
- Truitt Janney (https://github.com/truittjanney)

We welcome contributions from the community! How to contribute:
- Search existing issues before creating a new issue. Please check to see if it has already been reported. This helps us avoid duplicates.
- If you cannot find an existing issue, you can create a new one. Please provide detailed information about the problem, including steps to reproduce, expected behavior, and any relevant screenshots.

Making Changes:
- 1) Fork the repository - Start by forking the repository to your GitHub account.
- 2) Clone the repository - Clone your forked repository to your local machine using 'git clone https://github.com/your-username/your-repo-name.git
- 3) Create a new branch - Create a new branch for your changes. Use a descriptive name for your branch to identify the feature or fix you are working on.
- 4) Use the command 'git checkout -b your-branch-name'
- 5) Make your changes - Make your changes to the codebase. Ensure your code follows the project's coding standards and passes all tests.

Committing & Pushing Changes:
- 1) Commit your changes - Once you have made and tested your changes, commit them with a clear and concise commit message. Then push your changes to your forked repository.
- 2) Use the command 'git add .'
- 3) Use the command 'git commit -m "Description of the changes"'
- 4) Use the command 'git push origin your-branch-name'

Creating a Pull Request:
- 1) Navigate to the original repository - Go to the original repository where you want to submit your changes.
- 2) Create a pull request - Click on the "New Pull Request" button. Ensure your branch is compared with the correct branch in the original repository (usually "main" or "master").
- 3) Describe your changes - Provide a detailed description of your changes in the pull request. Mention any related issues and explain why the changes are necessary.
- 4) Submit the pull request - Submit your pull request and wait for the maintainers to review it.

Code Review & Feedback:
- Respond to feedback - The maintainers may request changes to your pull request. Be sure to respond to feedback promptly and make the necessary updates.
- Merge approval - Once your pull request is approved, it will be merged into the main codebase.

Best Practices for Contributing:
- Write clear commit messages - Make sure your commit messages are clear and descriptive.
- Follow coding standards - Adhere to the coding standards and guidelines specified in the repository.
- Test your changes - Ensure that your changes do not break existing functionality and pass all tests.
- Document your changes - Update any relevant documentation to reflect your changes.

Thank you for your interest in contributing to our project!
