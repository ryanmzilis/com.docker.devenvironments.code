This page gives you all the necessary information in order to contribute to the Firefox Design System.

## Clone the repository

The first step as a contributor is to either [clone or fork the repository](https://github.com/bwinton/StyleGuide). If you are part of the Firefox Design System team simply clone it. If you are an external contributor first fork the repository to your account and then clone it. Full instruction available on the [getting started page](https://github.com/bwinton/StyleGuide/wiki/Developing).

If you are a developer make sure to check the [developing guidelines](https://github.com/bwinton/StyleGuide/wiki/Developing) before filing a pull request. Same thing if you are an editor or a content creator, check the [writing guidelines](https://github.com/bwinton/StyleGuide/wiki/Writing).

## Create a branch

Once you have the repository or the fork up and running on your machine create a branch out of `master`. We usually name branches after the page or the feature we are currently working on. To create a branch with Terminal.app do:

```bash
$ git checkout -b new-branch-name
```

If you use the GitHub Desktop app follow [these simple steps](https://help.github.com/desktop/guides/contributing/creating-a-branch-for-your-work/).

## Create a pull request

Once you are happy with the changes create a pull request in order to publish them online. You can create pull requests from Terminal.app or the GitHub Desktop app thou the [GitHub web interface](https://github.com/bwinton/StyleGuide/compare/master...) gives you a great experience, highly recommended!

At the moment of writing our master branch is `bwinton/master`, make sure that this base is selected when you create a pull request. As a compare branch select the branch that you created before starting to contribute.

### Title and description

When you create a pull request give it a title and a brief description that explains the changes that you are submitting. If you know who is the Content Owner make sure to mention him or her in the description.

### Reviewers

Add a reviewer from the Design System team. Reviewers help us double-check changes that we intend to publish. Current reviewers are: aminalhazwani, brassy, bwinton, designakt, ericawright, FlyTori, pwalm, tinahsieh and TLHuang.

### Assignees

Add an assignee as a responsible person for merging the pull request. Current assignees are aminalhazwani for content changes. For development changes bwinton or ericawright. 

### Labels

Add a `needs: editorial` label if you need an editor to check your changes. Editing changes are non-blocking for the merge of the pull request. Add a `needs: visual` label if you need visual assets for your changes, also visual changes are non-blocking. Make sure to Cc TLHuang in your pull request description in order to help her understand what visual assets you may need.
