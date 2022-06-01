<img width=250px src="https://atsign.dev/assets/img/@platform_logo_grey.svg?sanitize=true">

# Contributing to Priv@tfit

Hi there!
Thanks for your interest in contributing to Priv@tefit.

We 💙 and accept [Pull Requests](https://help.github.com/articles/about-pull-requests/)
for fixing issues or adding features.

Please read our [code of conduct](code_of_conduct.md), which is based on
[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)](code_of_conduct.md)


### Housekeeping🧹

→ Check existing issues to verify that the bug or feature request has not already been submitted.

→ Open a pull request for any issue labelled help wanted or good first issue.

→ For small changes, especially documentation, you can simply use the "Edit" button
to update the Markdown file, and start the
[pull request](https://help.github.com/articles/about-pull-requests/) process.

→ Use the preview tab in GitHub to make sure that it is properly
formatted before committing.

→ A pull request will cause integration tests to run automatically, so please review
the results of the pipeline and correct any mistakes that are reported.

**❕Important:** *If you plan to contribute often or have a larger change to make, it is best to
setup an environment for contribution, which is what the rest of these guidelines
describe.*


## How can I contribute?

### For Developers - Developer environment setup
  
**Prerequisites**

  * Install Dart: https://dart.dev/get-dart
  * Install Flutter: https://docs.flutter.dev/get-started/install
  
**GitHub Repository Clone**

To prepare your dedicated GitHub repository:

1. Fork in GitHub https://github.com/atsign-foundation/REPO
2. Clone *your forked repository* (e.g., `git clone git@github.com:yourname/REPO`)
3. Set your remotes as follows:

    ```sh
   cd REPO
   git remote add upstream git@github.com:atsign-foundation/REPO.git
   git remote set-url upstream --push DISABLED
   ```
   
 Running `git remote -v` should give something similar to:

   ```text
   origin  git@github.com:yourname/REPO.git (fetch)
   origin  git@github.com:yourname/REPO.git (push)
   upstream        git@github.com:atsign-foundation/REPO.git (fetch)
   upstream        DISABLED (push)
   ```

   The use of `upstream --push DISABLED` is to prevent those
   with `write` access to the main repository from accidentally pushing changes
   directly. 
  
 **Development Process**

1. Fetch latest changes from main repository:

   ```sh
   git fetch upstream
   ```

2. Reset your fork's `trunk` branch to exactly match upstream `trunk`:

   ```sh
   git checkout trunk
   git reset --hard upstream/trunk
   git push --force
   ```

   **IMPORTANT**: Do this only once, when you start working on new feature as
   the commands above will completely overwrite any local changes in `trunk` content. 

3. Edit, edit, edit, and commit your changes to Git:

   ```sh
   # edit, edit, edit
   git add *
   git commit -m 'A useful commit message'
   git push
   ```

 4. Open a new Pull Request to the main repository using your `trunk` branch 
  
**Branching Strategy** 

In general, contributors should develop on branches based off of main.

-

### For Designers🎨

You may reference this [issue](https://github.com/atsign-foundation/privatefit/issues/5).

Please take a look at the Design System when suggesting features, and you are welcome to use our [Google Docs Template]() to suggest designs under the issue as a comment.

-

### For Technical, UX, Business Writers✍️ 

Do you want to contribute to the Privatefit documentation? Please read through the docs [contributing guides]() and design systems.

-

### Create yours… 🖱🪄

→ Find a bug, report it.

→ Find a typo, help us fix it.

→ Got ideas for a feature, open an issue to propose a change.

→ Find other ways that you can contribute to our projects by reading [this article](https://opensource.guide/how-to-contribute/).

**Please avoid:**

→ Opening pull requests for any issue marked core. These issues require additional context from the core team at Priv@teFit and any external pull requests will not be accepted. 

## Discussions

#PrivateFit channel on our discord community is a great place to ask questions, provide feedback that isn't a bug complaint or feature request, and learn about best practices. There's even a search button to discover if your question has already been answered!

## 📚Resources

→ [A guide to making open source contributions](https://opensource.guide/how-to-contribute/).

→ [About Pull Requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).

→ [Github Help](https://docs.github.com/en).

---

Priv@tefit is possible because of you and other volunteers. We encourage you to pitch in and join the team! 

Thanks for Contributing❕

with 💙 

Priv@teFit Team
