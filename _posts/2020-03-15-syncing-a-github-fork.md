# Syncing a github fork.

Borrowed of https://github.com/BlockSigner/cove

1. TOC
{:toc}

### Configure a remote for a fork
https://help.github.com/en/articles/configuring-a-remote-for-a-fork

- open the Terminal
- list the remote for your fork
```
$ git remote -v
```
- specify a new remote `upstream`
```
$ git remote add upstream https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git
```
- verify the new `upstream`
```
$ git remote -v
```

### Syncing the fork
from https://help.github.com/en/articles/syncing-a-fork

- open the Terminal
- change to your local project
- fetch the branches from upstream
```
$ git fetch upstream
```
- check out your fork's local `master` branch
```
$ git checkout master
```
- merge changes from `usptream/master` into `master`
```
$ git merge upstream/master
```

<script src="https://utteranc.es/client.js"
        repo="op07n/fastpages"
        issue-term="pathname"
        theme="github-light"
        crossorigin="anonymous"
        async>
</script>
