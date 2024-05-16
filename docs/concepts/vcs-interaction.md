# VCS interaction

When you interact with the version control system, such as Git, Kasama tracks different stats for you.
These can help you to improve your habits, for example if you aim for smaller, more frequent commits.

!!! note

    Currently, Kasama VCS interaction tracking only supports Git.
    If you are working with a different version control system, please consider opening a [feature request](https://github.com/spark-teams/kasama-intellij-support/issues/new?assignees=&labels=&projects=&template=feature_request.md&title=){:target="_blank"}.


## VCS Commits

Commits you are performing in the IDE (using the IntelliJ **Commit dialog**) are tracked by Kasama.

!!! note

    Git commits executed directly on the command line are not monitored.

The commits and related stats are shown in the **VCS Commits** diagram view.

## VCS Branches

Kasama keeps track in which branches you are active.

Kasama uses snapshots to detect the branches you are active in.
If you are active in a certain branch for a very short timespan (i.e. a few seconds), its activity might not be detected.

VCS branch stats can be viewed in the Kasama View under **VCS Branches** as a list or diagram view.

In the list view, different actions can be performed.

- **View Branch Timeline:** Display a detail view on the branch timeline, including commits and logged work durations
- **Edit Branch Type:** Set or change the branch type. If a type is set for a branch, you can filter by type in the diagram view. The following branch types are currently available:
    - *Feature* 
    - *Bugfix*
    - *Hotfix*
    - *Refactoring*
    - *Main*
    - *Testing*
    - *Experimenting*
    - *Maintenance*
    - *Documentation*
    - *Release*
    - *Integration*<br/>
  Depending on the branch name, Kasama tries to infer the branch name automatically when encountering a new branch.
- **Combine Branches** Kasama does not track branch renamings. 
If a branch is being renamed, the new branch might appear as a different branch.
To address this issue, utilize this function by specifying the old branch to be incorporated into the desired new branch.
All stats for the old branch (commits, durations) are being transferred to the new branch.
