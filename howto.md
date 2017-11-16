# Git quick howto

## Setup

Some prep work first.

### Installation

Download and install git from https://git-scm.com/downloads

### Create a following directory structure

```
~/tmp/git-tutorial $ tree
.
└── my_project
    ├── config.yml
    ├── css
    │   └── main.css
    ├── index.php
    └── js
        └── scripts.js

```

### Populate the files

```yaml
# config.yml
---
database:
  host: 127.0.0.1
  user: root
  password: s3cr#t
  dbname: world
```


```php
// index.php
phpinfo();
```


```css
/* css/main.css */
.red {color: red;}
```


```js
// js/scripts.js
function noop() {
    return;
}
```

### Create Github.com account

Simple stuff. Once done, send me your username.

## Git

It'd really help if you read up on versioning history, or what its for. In a nutshell, it allows to track changes to files, like who did what to a file(s), and when; marks those changes by a commit hash (or version), and enables collaboration by providing branching mechanism, where different people can work on the same file independently, and merge their changes at some point.

Once you learn some basic git commands, we will use the above layout to exchange work - I will send you tasks, you will complete them, and submit your changes to central repository (github.com).

For now, just run following commands in cmd (I'm running in Linux, thus be sure to map that to your env)

```bash
cd my_project
git init
git config --global user.name "Azizbek Odinaev"
git config --global user.email "<your email>"
git status
git add .
git commit -m "initial commit"
git log
```
