# Contribute

The NAPS DA Project welcomes contributions!  Please contribute and help in expanding the breadth and depth of content we showcase to customers!

## Table of Contents

* [Content Template](#Content-Template)
* [Pull Requests ](#pull-requests)
   * [Create a fork!](#create-a-fork)
   * [Stay in Sync](#stay-in-sync)
      * [Configuring Your Remotes](#configuring-your-remotes)
      * [Rebasing Your Branch](#rebasing-your-branch)
      * [Updating your Pull Request](#updating-your-pull-request)
   * [Create a pull requests](#create-a-pull-request)

# Content Template
```html
{::options parse_block_html="true" /}
<div class="collapse">*
<details><summary markdown="span">**TITLE**</summary>
<br>

  <span style="color:#0000CD">**Overview:**</span>

  The multi-cloud demo (workflow) consists of:
  1. Provision VMs in (1) Azure and (2) AWS
  2. In AWS configure an Apache server, in Azure an IIS server.
  3. Post in slack channel that multi-cloud workflow has finished.
  4. If any of the process fails (for example if the cloud availability is full) tear down in that cloud.

  <span style="color:#228B22">**Takeaways:**</span>

  1. Vendor-agnostic infrastructure-as-code
  2. Ansible used to provision **`and`** post-provision across clouds
  3. All infra is exposed as yml variable so it's human-friendly to use while still being flexible and powerful
  4. Can leverage the input and ouput of Tower. E.g. we kick it off from hosted services catalog to trigger and post to slack after it's finished but could also be kicked off from any CMDB and integrated with other Chatops.

  <span style="color:#a50000">Video Demonstration:</span>

  [![DEMO](http://img.youtube.com/vi/YOUTUBE_VIDEO_ID.jpg)](http://www.youtube.com/watch?v=YOUTUBE_VIDEO_ID "**TITLE**"){:target="_blank"}

</details>
</div>
{::options parse_block_html="false" /}
```
1. Edit:
   - *Line 3* - `TITLE`
   - *Line 8+* - `Define Overview`
   - *Line 14+* - `Define Takeaways`
   - *Line 23* - `Replace YOUTUBE_VIDEO_ID x 2 with youtube video id`
2. Add `<name>.md` file to appropriate technology folder {`ansible`, `openshift`, `acm`}
3. Add `{% include_relative <name>.md %}` to `<technology>.md` starting line 9
   - See ansible directory for reference
```
{% include_relative multi-cloud.md %}
{% include_relative network-report.md %}
{% include_relative snow-integration.md %}
{% include_relative infra-as-code.md %}
{% include_relative gitlab-ci-cd.md %}
{% include_relative elk-provisioning.md %}
{% include_relative f5-configuration.md %}
```

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