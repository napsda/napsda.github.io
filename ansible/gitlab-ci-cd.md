{::options parse_block_html="true" /}
<div class="collapse">
<details><summary markdown="span">GitLab CI/CD - Advanced</summary>
<br>

  <span style="color:#black">**NOTE:**</span>

  ---
  This demo is intended for advanced audiences. Familiarity with git, CI/CD, and/or IaC is higly recommended.

  ---

  <span style="color:#0000CD">**This CI/CD Demo Consists of:**</span>

  1.  Customer or internal entity initiates a change/feature request.
  2.  A developer pushes change to the git repository
  3.  CI starts running, first with a lint pipeline to run syntax checking (this is a unit test)
  4.  After linting succeeds, the **`quality-test`** pipeline is launched from GitLab CI
  5.  In turn, this launches the corresponding workflow job in Ansible Tower
  6.  (GitLab CI then waits for Tower to finish)
  7.  The "Dev" environment is provisioned with the recently added changes.

  -  `(optional)` A merge request is initiated to accept the original change request.
  -  `(optional)` An approver uses the successful pipelines (or manually checks the dev environment) to approve the MR.
  -  `(optional)` Changes are accepted into master and production is ready to deliver.
  -  `(optional)` Using Tower, the production environment is updated via **`master`** branch.

  <span style="color:#228B22">**Takeaways:**</span>

  -  Each change pushed (proposed) by developers is integrated into a **`Dev`** environment where it can be tested.
  -  Credentials are stored securely in Tower or another credential store  ensuring no **`manual`** intervention or configuration drift with the Dev environment.
  -  Devs cannot directly access the Dev environment and can only make changes through  git.
  -  Approvers are optional if human-in-the-loop is desired, otherwise the entire process can be automated
  -  CI/CD with OCP is much cleaner, but ansible allows legacy technology to participate, E.g. *`network`*

  <span style="color:#a50000">**Video Demonstration:**</span>

  [![DEMO](http://img.youtube.com/vi/w6hx4Ph0wJw/0.jpg)](http://www.youtube.com/watch?v=w6hx4Ph0wJw "Elk Post Provisioning"){:target="_blank"}

</details>
</div>
{::options parse_block_html="false" /}