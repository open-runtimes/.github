# Contributing

We would ❤️ for you to contribute to Open Runtimes and help make it better! We want contributing to Open Runtimes to be fun, enjoyable, and educational for anyone and everyone. All contributions are welcome, including issues, new docs as well as updates and tweaks, blog posts, workshops, and more.

## How to Start?

If you are worried or don’t know where to start, check out our next section explaining what kind of help is needed and where you can get involved. You can reach out with questions on our [Discord](https://discord.gg/fP6W2qEzfQ) server. You can also submit an issue and a maintainer can guide you!

## Code of Conduct

Help us keep Open Runtimes open and inclusive. Please read and follow our [Code of Conduct](/CODE_OF_CONDUCT.md).

## Submit a Pull Request 🚀

Branch naming convention is as following

`TYPE-ISSUE_ID-DESCRIPTION`

example:

```
doc-548-submit-a-pull-request-section-to-contribution-guide
```

When `TYPE` can be:

- **feat** - is a new feature
- **doc** - documentation only changes
- **cicd** - changes related to CI/CD system
- **fix** - a bug fix
- **refactor** - code change that neither fixes a bug nor adds a feature

**All PRs must include a commit message with the description of the changes made!**

Start by forking the project and use the `git clone` command to download the repository to your computer. A standard procedure for working on an issue would be to:

1. Before creating a new branch, pull the changes from upstream to make sure your default branch is be up to date.

```
$ git pull
```

2. Create a new branch from the default branch. For example `doc-548-submit-a-pull-request-section-to-contribution-guide`

```
$ git checkout -b [name_of_your_new_branch]
```

3. Work - commit - repeat ( be sure to be in your branch )
4. Push changes to GitHub

```
$ git push origin [name_of_your_new_branch]
```

6. Submit your changes for review. If you go to your repository on GitHub, you'll see a `Compare & pull request` button. Click on that button.
7. Start a Pull Request (PR) by clicking on `Create pull request`. Make sure to update the PR description following the template provided.
8. Wait for a code review.
9. If you need to make changes based on feedback, make sure to re-request a review from your reviewer after you've made the necessary changes.

![Re-Request a Review](https://docs.github.com/assets/cb-4714/images/help/pull_requests/request-re-review.png)

10. After approval, your PR will be merged.
11. You can delete your branch after it has been merged.

## Installation

To install a working development environment follow these instructions:

1. Fork or clone the open-runtimes/open-runtimes repository.

2. Install Composer dependencies using one of the following options:

**Composer CLI**

```bash
composer update --ignore-platform-reqs --optimize-autoloader --no-plugins --no-scripts --prefer-dist
```

**Docker (UNIX)**

```bash
docker run --rm --interactive --tty --volume "$(pwd)":/app composer update --ignore-platform-reqs --optimize-autoloader --no-plugins --no-scripts --prefer-dist
```

**Docker (Windows)**

```bash
docker run --rm --interactive --tty --volume "%cd%":/app composer update --ignore-platform-reqs --optimize-autoloader --no-plugins --no-scripts --prefer-dist
```

4. Build the runtimes you want to test using the docker build command:

```
docker build -t {{Image Tag Name}} ./runtimes/{{Folder of your runtime}}
```

5. [Follow our contribution guide to learn how you can add support for more runtimes.](https://github.com/open-runtimes/open-runtimes/blob/main/docs/add-runtime.md)

## Introducing New Features

We would 💖 you to contribute to Appwrite, but we would also like to make sure Open Runtimes is as great as possible and loyal to its vision and mission statement 🙏.

For us to find the right balance, please open an issue explaining your ideas before introducing a new pull request.

This will allow the Open Runtimes community to have sufficient discussion about the new feature value and how it fits in the product roadmap and vision.

This is also important for Open Runtimes maintainers to discuss the feature's design and architecture to help the contribution fit in organically in the Appwrite codebase.

## Other Ways to Help

Pull requests are great, but there are many other areas where you can help Open Runtimes.

### Blogging & Speaking

Blogging, speaking about, or creating tutorials about any of Open Runtimes’s many usages are great ways to contribute and help our project grow.

### Presenting at Meetups

Presenting at meetups and conferences about your Open Runtimes projects. Your unique challenges and successes in building things with Open Runtimes can provide great speaking material. We’d love to review your talk abstract/CFP, so get in touch with us if you’d like some help!

### Sending Feedbacks & Reporting Bugs

Sending feedback is a great way for us to understand your different use cases of Open Runtimes better. If you had any issues, bugs, or want to share about your experience, feel free to do so on our GitHub issues page or at our [Discord channel](https://discord.gg/fP6W2qEzfQ).

### Improving Documentation

Submitting documentation updates, enhancements, designs, or bug fixes. Spelling or grammar fixes will be very much appreciated.

### Helping Someone

Searching for Open Runtimes on Discord, GitHub, or StackOverflow and helping someone else who needs help. You can also help by teaching others how to contribute to Open Runtime's repo!
