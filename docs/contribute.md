# Contribute

The NAPS DA Project welcomes contributions!  Please contribute and help in expanding the breadth and depth of content we showcase to customers!

## Table of Contents

* [Pull Requests ](#pull-requests)
   * [Create a fork!](#create-a-fork)
   * [Stay in Sync](#stay-in-sync)
      * [Configuring Your Remotes](#configuring-your-remotes)
      * [Rebasing Your Branch](#rebasing-your-branch)
      * [Updating your Pull Request](#updating-your-pull-request)
   * [Create a pull requests](#create-a-pull-request)

# Pull Requests

We take pull requests!  What is a pull request?

>Pull requests let you tell others about changes you've pushed to a branch in a repository on GitHub. Once a pull request is opened, you can discuss and review the potential changes with collaborators and add follow-up commits before your changes are merged into the base branch

More info on PRs: [https://help.github.com/en/articles/about-pull-requests](https://help.github.com/en/articles/about-pull-requests)

## Create a fork!

Create a fork on your own Github project (or your personal space)

[Github Documentation on Forking a repo](https://help.github.com/articles/fork-a-repo/)

## Stay in Sync

It is important to know how to keep your fork in sync with the upstream napsda project.

### Configuring Your Remotes

Configure `napsda/napsda.github.io` as your upstream so you can stay in sync

```bash
git remote add upstream https://github.com/napsda/napsda.github.io.git
```

### Rebasing Your Branch

Rebase the branch on your fork

```bash
git pull --rebase upstream devel
```

Check your status

```bash
git status
```

### Updating your Pull Request

```bash
git push --force
```

More info on docs.ansible.com: [Rebasing a Pull Request](http://docs.ansible.com/ansible/latest/dev_guide/developing_rebasing.html)

## Create a pull request

Make sure you are not behind (in sync) and then submit a PR to the napsda.
[Read the Pull Request Documentation on Github.com](https://help.github.com/articles/creating-a-pull-request/)

 - WHY? Why did you make the change?
 - WHO? Who is this for?  If this is something for a limited audience it might not make sense for all users.
 - CONTENT? What content are you providing?

Being more descriptive is better and will making merging into upstream easier and quicker!  Communication is key!  Just b/c the PR doesn't get accepted right away doesn't mean it is not a good idea. Thank you for contributing!