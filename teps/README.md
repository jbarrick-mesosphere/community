# Tekton Enhancement Proposals (TEPs)

A Tekton Enhancement Proposal (TEP) is a way to propose, communicate
and coordinate on new efforts for the Tekton project.  You can read
the full details of the project in
[TEP-1](0001-tekton-enhancement-proposal-process.md).

## What is a TEP

A standardized development process for Tekton is proposed in order to

- provide a common structure and clear checkpoints for proposing
  changes to Tekton
- ensure that the motivation for a change is clear
- allow for the enumeration stability milestones and stability
  graduation criteria
- persist project information in a Version Control System (VCS) for
  future Tekton users and contributors
- support the creation of _high value user facing_ information such
  as:
  - an overall project development roadmap
  - motivation for impactful user facing changes
- ensure community participants are successfully able to drive changes
  to completion across one or more releases while stakeholders are
  adequately represented throughout the process

This process is supported by a unit of work called a Tekton
Enhancement Proposal (TEP). A TEP attempts to combine aspects of the
following:

- feature, and effort tracking document
- a product requirements document
- design document

into one file which is created incrementally in collaboration with one
or more [Working
Groups](https://github.com/tektoncd/community/blob/master/working-groups.md)
(WGs).

This process does not block authors from doing early design docs using
any means. It does not block authors from sharing those design docs
with the community (during Working groups, on Slack, GitHub, ….

**This process acts as a requirement when a design docs is ready to be
implemented or integrated in the `tektoncd` projects**. In other words,
a change that impact other `tektoncd` projects or users cannot be
merged if there is no `TEP` associated with it.

This TEP process is related to

- the generation of an architectural roadmap
- the fact that the what constitutes a feature is still undefined
- issue management
- the difference between an accepted design and a proposal
- the organization of design proposals

This proposal attempts to place these concerns within a general
framework.

See [TEP-1](0001-tekton-enhancement-proposal-process.md) for more
details.

The TEP `OWNERS` are the **main** owners of the following projects:

- [`pipeline`](https://github.com/tektoncd/pipeline)
- [`cli`](https://github.com/tektoncd/cli)
- [`triggers`](https://github.com/tektoncd/triggers)
- [`dashboard`](https://github.com/tektoncd/dashboard)
- [`catalog`](https://github.com/tektoncd/catalog)
- [`hub`](https://github.com/tektoncd/hub)
- [`operator`](https://github.com/tektoncd/operator)

## Merging TEPs

- When creating a new TEP, pick a number for it, equal to the maximum
  TEP available in the repo and open PRs.
  A valid new number can be obtained via `./hack/tep-number.sh`. Note
  that the picked number is not "locked" until a PR is created.
  The TEP number shall be set
  in the TEP file name, TEP title and PR title:
  - file name in the format `teps/<XXXX>-<tep-title>.md`
  - title in the format `# TEP-XXXX: <tep-title>`
  - PR title in the format `TEP-XXXX: <tep-title>`
- TEP should be merge as soon as possible in the `proposed` state. As
  soon as a general consensus is reached that the TEP, as described
  (even if incomplete) make sense to pursue, the TEP can be
  merged. The authors can then update the missing part in follow-up
  pull requests and move it to `implementable`.
- TEP should be approved by ***at least two owners*** from different
  company. This should prevent a company to *force push* a TEP (and
  thus a feature) in the tektoncd projects.

## TEPs

This is the complete list of Tekton teps:

| TEP  | Title  | Status   | Last Updated  |
|------|--------|----------|---------------|
|[TEP-0001](0001-tekton-enhancement-proposal-process.md) | Tekton Enhancement Proposal Process | implemented | 2020-06-11 |
|[TEP-0002](0002-custom-tasks.md) | Custom Tasks | implementable | 2020-07-07 |
|[TEP-0003](0003-tekton-catalog-organization.md) | Tekton Catalog Organization | implementable | 2020-08-12 |
|[TEP-0004](0004-task-results-in-final-tasks.md) | Task Results in Final Tasks | implementable | 2020-07-16 |
|[TEP-0005](0005-tekton-oci-bundles.md) | Tekton OCI Bundles | implementable | 2020-08-13 |
|[TEP-0006](0006-tekton-metrics.md) | Tekton Metrics | proposed | 2020-07-13 |
|[TEP-0007](0007-conditions-beta.md) | Conditions Beta | implementable | 2020-11-02 |
|[TEP-0008](0008-support-knative-service-for-triggers-eventlistener-pod.md) | Support Knative Service for Triggers EventListener Pod | implementable | 2020-08-25 |
|[TEP-0009](0009-trigger-crd.md) | Trigger CRD | implementable | 2020-09-08 |
|[TEP-0010](0010-optional-workspaces.md) | Optional Workspaces | implemented | 2020-10-15 |
|[TEP-0011](0011-redirecting-step-output-streams.md) | redirecting-step-output-streams | implementable | 2020-11-02 |
|[TEP-0012](0012-api-spec.md) | API Specification | implementable | 2020-08-10 |
|[TEP-0014](0014-step-timeout.md) | Step Timeout | implementable | 2020-09-10 |
|[TEP-0016](0016-concise-trigger-bindings.md) | Concise Embedded TriggerBindings | implementable | 2020-09-15 |
|[TEP-0019](0019-other-arch-support.md) | Other Arch Support | proposed | 2020-09-30 |
|[TEP-0020](0020-s390x-support.md) | s390x Support | proposed | 2020-09-21 |
|[TEP-0022](0022-trigger-immutable-input.md) | Triggers - Immutable Input Events | proposed | 2020-09-29 |
|[TEP-0024](0024-embedded-trigger-templates.md) | Embedded TriggerTemplates | implementable | 2020-10-01 |
|[TEP-0025](0025-hermekton.md) | Hermetic Builds | implementable | 2020-09-11 |
|[TEP-0027](0028-task-execution-status-at-runtime.md) | task-exec-status-at-runtime | implementable | 2020-11-02 |
|[TEP-0027](0027-https-connection-to-triggers-eventlistener.md) | HTTPS Connection to Triggers EventListener | proposed | 2020-10-19 |
|[TEP-NNNN](XXXX-step-workspaces.md) | step-and-sidecar-workspaces | proposed | 2020-10-02 |
