<!-- ================== -->
<!-- ================== -->
<!-- ================== -->

# Start

<!-- ===================== -->
<!-- quick mkdir           -->
<!-- ===================== -->

## quick mkdir

![make surrealdb dir](/images/mkdir.png)

<!-- ===================== -->
<!-- quick add locally
 hosted code to github     -->
<!-- ===================== -->

## quick add code to github

to add locally hosted code to github see documentation
👇

[github docs](https://docs.github.com/en/get-started/importing-your-projects-to-github/importing-source-code-to-github/adding-locally-hosted-code-to-github)

<!-- ===================== -->
<!-- install surreal====== -->
<!-- ===================== -->

# installing SurrealDB on macOS

for other OS, see [installation](https://surrealdb.com/docs/start/installation)

```bash
# for macOS
brew install surrealdb/tap/surreal
```

check if installed

```bash
surreal help
```

![surreal help](/images/installok.png)

## quick source control

```bash
git status
&&
git add .
&&
git status
&&
# replace "a commit message"
git commit -m "a commit message"
&&
#push to origin, main branch.
git push -u origin main
```

# star the server

```bash
surreal start --log debug --user root --pass root memory
```

![surreal start](/images/start.png)

# insert and query data using the SurrealQL REST endpoint

Surreal queries are submitted as `HHTP POST`

`HTTP POST` is the most widely supported method of submitting data to a web server

The SurrealQL REST endpoint by default is

[http://localhost:8080/surrealql
](http://localhost:8080/surrealql)

## connect to SurrealDB

````bash
## insert data

use `cURL` on the command-line.

```bash
DATA="INFO FOR DB;"
curl --request POST \
	--header "Content-Type: application/json" \
	--header "NS: test" \
    # header "NS: test" means use the test namespace
	--header "DB: test" \ # header "DB: test" means use the test database
	--user "root:root" \ #root:root is the default user and password
	--data "${DATA}" \
    # data is the data to insert
	http://localhost:8000/sql
````

![surreal insert](/images/insertdata.png)

# inserting data shcemaless mode

> ["By default, SurrealDB doesn't need to have tables or fields defined before inserting data. Instead the database can be queried in schemaless mode, and tables are created ad hoc."](https://surrealdb.com/docs/start#inserting-data)

> SurrealDB allows you to traverse related records efficiently without needing to use JOINs.

<!-- ================== -->
<!-- ================== -->
<!-- ================== -->

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
<!--Terms======== -->
<!-- ===================== -->

# Concepta

1. Server side libraries vs client-side library
1. [RESPT API vs HHTP API](https://hevodata.com/learn/http-api-vs-rest-api/)

<!-- ===================== -->

github docs

<!-- ===================== -->

```bash
git status
&&
git add .
&&
git status
&&
git commit -m "a commit message"
&&
#push to origin, main branch.
git push -u origin main
```

[crate surrealdb](https://docs.rs/surrealdb/1.0.0-beta.7/surrealdb/)
