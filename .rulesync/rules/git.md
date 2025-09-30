---
root: false
targets: ["*"]
description: "Rules for working git"
globs: ["**/*"]
---

# Git

* Anytime a task is completed, a Git commmit should be made to track changes.
* Any Umbraco specific changes should be done on a develop branch (i.e. "/develop/featureABC").
  * If the current branch is main/master, create and checkout a new develop branch before executing anything that affects Umbraco.