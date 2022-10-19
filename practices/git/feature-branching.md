# Feature Branching

*The core idea behind the Feature Branch Workflow is that all feature development should take place in a dedicated branch instead of the main branch. This encapsulation makes it easy for multiple developers to work on a particular feature without disturbing the main codebase.* - [Git Feature Branch Workflow | Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow)


## Example

A basic workflow for git when completing a new piece of work:

1. Clone a repo (or update local copy via fetch/pull)
2. Create feature branch from development branch, our source to start from.
3. Development work
4. Stage Changes
5. Commit
6. Repeat 3-5 until complete
7. Check for conflicts, when multiple developers share a repo this makes it pretty simple to identify when a merge conflict will occur.
   1. With all feature branch changes committed or stashed
   2. Checkout development branch and update fetch/pull, now you are back up to date with the current. You will see if any changes were `pull`ed down by this  
   3. If there are no changes, you pre-check is done. If there are changes, our next step is to ensure any conflicts are resolved.
   4. Checkout your feature branch again.
   5. Now we accept the changes that have happened in our source since we started work. That we also make the appropriate changes to resolve those conflicts in our Pull Request.
8.  Raise Pull Request
9.  The review process is done, if not approved repeat 3-7 again, you do not need to execute step 8 because the pull request will continue to be the contents of your feature branch.
10. On approval, the PR will either be auto-merged or available to be merged.
11. Once merged, this scenario is complete.


The source repository is setup in this scenario. There is are some existing feature branches already in the repository which contain other changes and conflicts with the changes we will make to take a direct example through 3 scenarios.

__Scenarios__
 1. Happy Path - Merge
 2. Conflict resolution
 3. Happy Path - Rebase
 4. Happy Path - Squash Commit

Scenario 1:

```
git clone https://perficient-devops-training@dev.azure.com/perficient-devops-training/DeveloperExperience/_git/examples-feature-branching


```
