# NPM Package Template

Template for NPM packages, incorporating TypeScript and Jest.

Included workflows:
- run tests on PRs
- publish package to GitHub on release*

*Enable in repo settings: Actions > General > Workflow permissions: Read and Write permissions

### Scripts

| Script | Description |
| ------ | ----------- |
| `build` | Compiles the TypeScript source code to JavaScript and places in `build/`. |
| `test` | Runs the Jest test suite. |

### Publishing

Version bump and create a new commit and tag: `npm version <major|minor|patch>`

Push the commit and tag to GitHub: `git push --follow-tags`

Open a PR to merge the commit into `main`.

Create a release on GitHub using the new tag. This triggers the action that will publish the package to GitHub.
