# Contributing to Omek

> Note: Some of the guide is inspired by the Angular project, adapted to our need.

Here are the guidelines we would like you to follow when contributing to Omek:

## Content Table

* [Found a Bug?](#bug)
* [Feature Requests](#feature)
* [Workflow](#workflow)
* [Commit Message Guidelines](#commit)

## <a name="bug"></a> Found a Bug?
If you found a bug or a user approach you with a bug just follow thus steps:

1. Open Issue in GitLab using the "Bug" template, set the issue milestone according to the project.
1. Start a discussion, is the bug critical? who should fix it? when we should fix it?
1. A team member is selected to be in-charge of the bug, speaking to the users, checking up on the bug fix and knowing where the issue stand.
1. Fix the bug.
1. Notify the relevant users about the bug fix.

## <a name="feature"></a> Feature Requests
If you or a user have a feature request just follow thus steps:

1. Open Issue in GitLab using the "Feature Requests" template.
1. Start a discussion, is the feature needed? who should create it? when we should create it? is it require a new milestone?
1. A team member is selected to be in-charge of the feature, speaking to the users, checking up on the feature and knowing where the issue stand.
1. Update the issue accordantly
1. Notify the relevant users about the decision.
1. Create the new feature.

## Workflow

Read more at [WORKFLOW.md](WORKFLOW.md).

## <a name="commit"></a> Commit Message Guidelines

We have very precise rules over how our git commit messages can be formatted.  This leads to **more
readable messages** that are easy to follow when looking through the **project history**.

### Commit Message Format

Each commit message consists of a **header**, a **body** and a **footer**.  The header has a special
format that includes a **type** and a **subject**:

```
<type>: <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

The **header** is mandatory.

Any line of the commit message cannot be longer 100 characters! This allows the message to be easier
to read on GitLab as well as in various git tools.

The footer should contain a closing reference to an issue if any.

For Example:

```
fix: Animation not working in IE 11

Fixed animation in the Occupation page not working in IE 11.
Found new bug in report page, #1112

Resolved #1111
```

### Revert

If the commit reverts a previous commit, it should begin with `revert: `, followed by the header of the reverted commit. In the body it should say: `This reverts commit.`.

### Type

Must be one of the following:

* **build**: Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)
* **ci**: Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs)
* **docs**: Documentation only changes
* **feat**: A new feature
* **fix**: A bug fix
* **perf**: A code change that improves performance
* **refactor**: A code change that neither fixes a bug nor adds a feature
* **style**: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
* **test**: Adding missing tests or correcting existing tests

### Subject

The subject contains a succinct description of the change:

* Use the imperative, present tense: "change" not "changed" nor "changes"
* Capitalize the first letter
* No dot (.) at the end

### Body

Just as in the **subject**, use the imperative, present tense: "change" not "changed" nor "changes".
The body should include the motivation for the change and contrast this with previous behavior.

#### Reference Issue

To reference an issue just write the issue symbol (`#`) and id, for example:

### Footer

The footer it the place to reference GitLab issues that this commit **Closes**.

To close an issue write in the footer on of the following things:

```
Resolved #1111
# OR
Fixed #1111
# OR
Done #1111
```