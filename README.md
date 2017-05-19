# git-commit-info

Get all information about a specific commit.

## Installation

```sh
$ npm i git-commit-info --save
```
or
```sh
$ yarn add git-commit-info
```

## Usage

**Available parameters:**
- `cwd`: Specify the path. Default: `process.cwd()`
- `commit`: The hash of the commit. Default: latest

```js
const gitCommitInfo = require('git-commit-info');

// information of process.cwd() and the latest commit
gitCommitInfo();

// information of the latest commit in ./my_repo
gitCommitInfo({
  cwd: './my_repo',
});

// information of the specified commit in process.cwd()
gitCommitInfo({
  commit: '82442c2405804d7aa44e7bedbc0b93bb17707626', // any hash
});

// information of the specified commit in ./my_repo
gitCommitInfo({
  cwd: './my_repo',
  commit: '82442c2405804d7aa44e7bedbc0b93bb17707626', // any hash
});
```

## LICENSE

MIT © [Jan Peer Stöcklmair](https://www.jpeer.at)