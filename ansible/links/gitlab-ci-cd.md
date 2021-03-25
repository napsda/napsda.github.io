# CI/CD Demo

This demo is intended for advanced audiences. If they aren't already familiar with git, CI/CD, or IaC concepts they will likely just be confused.

The CI/CD demo consists of:
1. Customer or internal entity initiates a change/feature request.
1. A developer pushes change to the git repository
1. CI starts running, first with a lint pipeline to run syntax checking (this is a unit test)
1. After linting succeeds, the `quality-test` pipeline is launched from GitLab CI
1. In turn, this launches the corresponding workflow job in Ansible Tower
1. (GitLab CI then waits for Tower to finish)
1. The "Dev" environment is provisioned with the recently added changes.

- (optional) A merge request is initiated to accept the original change request.
- (optional) An approver uses the successful pipelines (or manually checks the dev environment) to approve the MR.
- (optional) Changes are accepted into master and production is ready to deliver.
- (optional) Using Tower, the production environment is updated via `master` branch.

## Takeaways
1. Each change pushed (proposed) by developers is integrated into a "Dev" environment where it can be tested.
1. Credentials are stored securely in Tower or another credential store  ensuring no "manual" intervention or configuration drift with the Dev environment.
1. Devs cannot directly access the Dev environment and can only make changes through  git.
1. Approvers are optional if human-in-the-loop is desired, otherwise the entire process can be automated
1. CI/CD with OCP is much cleaner, but ansible allows legacy technology to participate, E.g. network equipment, edge gear, non-contained infra

## Demo
Check out the video demonstration:

  [![DEMO](http://img.youtube.com/vi/w6hx4Ph0wJw/0.jpg)](http://www.youtube.com/watch?v=w6hx4Ph0wJw "Elk Post Provisioning"){:target="_blank"}