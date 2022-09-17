## 1. Step:

cmd + space and type "terminal" and open it
cd to you `code` folder.
mkdir `surrealdb`
cd `surrealdb`
git clone this repo

Branch:
1.a push repo to github from the terminal git checkout -b `yourname`-`yourbranchname`
change master to main (optional, good practice)

## 1. Step: [install](https://surrealdb.com/docs/start/installation) SurrealDB

1.a cd `surrealdb` and `code .` to open new directory in VSCode
in vscode, shift + ctrl g to open

<!-- ============= -->

### quick

```bash
git init -b main
```

<!-- ===================== -->
<!-- view changes          -->
<!-- ===================== -->

to view changes to be commited

```bash
git status
```

<!-- ===================== -->
<!-- stage and commint     -->
<!-- ===================== -->

### stage and commint

```bash
git add .
```

`.` is for all files in the current directory

```bash
git commit -m "first commit"
```

`-m` is for message

<!-- ===================== -->
<!-- rename branch to main -->
<!-- ===================== -->

### rename branch to main (optional)

````bash

```bash
git branch -M main
````

`#-M` is for force rename

<!-- ===================== -->
<!-- publishg to github as surrealdb as a public repo
and MIT license            -->
<!-- ===================== -->

```bash
gh repo create surrealdb --public --license mit
```

<!-- ===================== -->

> <sup>👉 👀 note:</sup> ![github docs](/images/mkrepo.png) <sup>is this thrue?</sup>

<!-- ===================== -->
