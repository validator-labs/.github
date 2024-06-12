Contributing
============

All contributions are welcome to this project!

How to contribute
-----------------

-  **File an issue** - if you found a bug, want to request an
   enhancement, or want to implement something (bug fix or feature).
-  **Send a pull request** - if you want to contribute code. Please be
   sure to file an issue first.

Pull request best practices
---------------------------

We want to accept your pull requests! Please follow these steps:

## Step 1: File an issue

Before writing any code, please file an issue stating the problem you
want to solve or the feature you want to implement. This allows us to
give you feedback before you spend any time writing code. There may be a
known limitation that can't be addressed, or a bug that has already been
fixed in a different way. The issue allows us to communicate and figure
out if it's worth your time to write a bunch of code for the project.
If changes are trivial, use the PR message to write why we need the patch, 
and the motivations behind it.

- All issues must be labeled with one of
    - 🐛 (`:bug:`, patch and bugfixes)
    - ✨ (`:sparkles:`, feature additions)
    - 🌱 (`:seedling:`, enhancements)
    - :knife: ( `:knife`, spikes)
    - :art: ( `:art`, refactoring )
    - 📖 (`:book:`, documentation)
    - :robot: (`:robot:`, CI/tests changes)
    - :building_construction: (`:building_construction:`, epics)
    - :shield: (`:shield:`, security changes)

## Step 2: Fork this repository in GitHub

This will create your own copy of our repository.

## Step 3: Add the upstream source

The upstream source is the project under the Box organization on GitHub.
To add an upstream source for this project, type:

```
git remote add upstream git@github.com:validator-labs/<forked-repo>.git
```

Create a branch with a descriptive name, such as ``fix/ensure-resource-cleanup``.

## Step 5: Push your feature branch to your fork

If working on an issue, signal to other contributors that you are actively working on it by commenting on the issue.

All commits and pull requests must adhere to the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) specification.

If your PR has multiple commits, they must be [squashed into a single commit](https://kubernetes.io/docs/contribute/new-content/open-a-pr/#squashing-commits) before your PR is merged.

All changes must be code reviewed. Expect reviewers to request that you avoid common [go style mistakes](https://github.com/golang/go/wiki/CodeReviewComments) in your PRs.

Keep a separate feature branch for each issue you want to address.

## Step 6: Rebase

Before sending a pull request, rebase against upstream, such as:

```bash
git fetch upstream
git rebase upstream/main
```

This will add your changes on top of what's already in upstream,
minimizing merge issues.

## Step 7: Run the tests

Make sure that all tests are passing before submitting a pull request.

You can run the tests locally with:

```bash
make test
```

## Step 8: Send the pull request

Send the pull request from your feature branch to us, ensuring your PR title follows the conventional commits spec. For example:
```
"feat: add support for signature verification"
```

Be sure to also include a description that lets us know what work you did and also a link to the issue you're addressing.

Keep in mind that we like to see one issue addressed per pull request,
as this helps keep our git history clean and we can more easily track
down issues.
