
# Template

You can use the `template` query parameter to specify a template to automatically fill the issue or pull request body. The `template` query parameter works with templates stored in an `ISSUE_TEMPLATE` or `PULL_REQUEST_TEMPLATE` subdirectory within the root, `docs/` or `.github/` directory in a repository.

## Table of Contents

* [Pull Requests Template](#pr-template)
* [Issues Template](#issues-template)
* Try it
    - [New issue](../../../issues/new/choose)


### In the file name field:

To make your pull request template visible in the repository's root directory, type the name of your pull request template. For example, `pull_request_template.md`.

To make your pull request template visible in the repository's docs directory, type `docs/`, then the name of your pull request template. For example, `docs/pull_request_template.md`.

To store your file in a hidden directory, type `.github/`, then the name of your pull request template. For example, `.github/pull_request_template.md`.


<a name="pr-template"/>

## Pull Request Template
When you add a pull request template to your repository, project contributors will automatically see the template's contents in the pull request body.

### Example from [airbnb/lona](https://raw.githubusercontent.com/airbnb/Lona/master/.github/PULL_REQUEST_TEMPLATE.md):

```
## What

I added a new button / fixed this bug / added this endpoint. It looks like this
<screenshot / endpoint url / whatever>

## Why

I did this change in order to...

## Major Changes

* I added the modules for this change…
* And this other thing too!

## Requirements for Merging

- [ ] It should do this
- [ ] It should edit this file
- [ ] It should look like this

## Testing Plan

- [ ] Tested this change locally
- [ ] Checked that existing features work

## Feedback

I'm looking for feedback on:

* <this important decision>
* <this design>
* <this code style>

<!-- Tag relevant people for example -->
cc: @someone

```

<a name="issues-template"/>

## Issues Template

When you add a issue template to your repository, project contributors will automatically see the template's contents in the issue body.

#### Example from [googlesamples/google-services](https://github.com/googlesamples/google-services/blob/master/ISSUE_TEMPLATE.md)

```
### Step 1: Are you in the right place?

  * For issues or feature requests related to the code **in this repository** file a Github issue.
  * For general technical questions, post a question on [StackOverflow](http://stackoverflow.com/) tagged appropriately.

### Step 2: Describe your environment

  * Device: _____
  * OS version: _____
  * SDK version: _____
  * [Android] Google Play Services version: _____
  
### Step 3: Describe the problem:

#### Steps to reproduce:

  1. _____
  2. _____
  3. _____
  
#### Observed Results:

  * What happened?  This could be a description, log output, etc.
  
#### Expected Results:

  * What did you expect to happen?
  
#### Relevant Code:

  // TODO(you): code here to reproduce the problem
```

<a name="pr-template"/>