# Welcome!

If you are reading this document then you are interested in contributing to Islandora, and that's awesome! All contributions are welcome: use-cases, documentation, code, patches, bug reports, feature requests, etc. You do not need to be a programmer to speak up!

We also have an irc channel -- #islandora -- on freenode.net. Feel free to hang out there, ask questions, and help others out if you can.

## Workflows

Islandora Committers Calls happen every Thursday at 2PM EST. The meetings are generally held on Skype, and you can join the calls by sending a request to community@islandora.ca.

### Documentation

You can contribute documentation in two different ways. One way is to join the [Documentation Interest Group](https://github.com/islandora-interest-groups/Islandora-Documentation-Interest-Group). Another way is to [open an issue](https://jira.duraspace.org/secure/CreateIssue!default.jspa). You will need a JIRA account to do this. If you don't have one, you can sign up [here](https://jira.duraspace.org/secure/Signup!default.jspa). Set the Issue Type to "Documentation".

### Request a new feature (use cases).

To request a new feature you should [open an issue](https://jira.duraspace.org/secure/CreateIssue!default.jspa). You will need a JIRA account to do this. If you don't have one, you can sign up [here](https://jira.duraspace.org/secure/Signup!default.jspa). Set the Issue Type to "New Feature".

In order to help us understand the feature request, it would be great if you could provide us with a use case:

| Title (Goal)  | The title or goal of your use case                            |
--------------- |------------------------------------                           |
| Primary Actor | Repository architect, implementer, repository admin, user     |
| Scope         | The scope of the project. Example: architecture, access       |
| Level         | The priority the use case should be given; High, Medium, Low  |
| Story         | This is a [user story](http://en.wikipedia.org/wiki/User_story).


***

**Examples**:
* Bullet
* Listed
* Examples should you want to provide them.

**Remarks**:
* Bullet
* Listed
* Remarks should you want to provide them.

### Report a bug

To report a bug you should [open an issue](https://jira.duraspace.org/secure/CreateIssue!default.jspa) that summarizes the bug. Set the Issue Type to "Bug".

In order to help us understand and fix the bug it would be great if you could provide us with:

1. The steps to reproduce the bug. This includes information about e.g. the Islandora version you were using along with version of stack components.
2. The expected behavior.
3. The actual, incorrect behavior.

Feel free to search the issue queue for existing issues (aka tickets) that already describe the problem; if there is such a ticket please add your information as a comment.

**If you want to provide a pull along with your bug report:**

That is great! In this case please send us a pull request as described in section _Create a pull request_ below.

### Participate in a Release

Islandora releases occur twice yearly, at the end of April and October. Two to three months before a release, a Call for Volunteers will be issued across Islandora communication channels (website, Twitter, listservs). The Release team consists of both developers and end-users who fix bugs, test fixes, verify improvements and new features; update documentation; and review README and LICENSE files. A Release VM is issued with each release so that testers can have a stable, easy-to-deploy environment in which to work.

To join an Islandora Release Team, sign up for one or more modules in any of the following roles:

* **Component Manager** (Very familiar with module code; reviews commits)
* **Tester** (Tests JIRA tickets marked "Ready for test" and does a general workover of the module)
* **Documentor** (Reviews and updates existing documentation or writes new documentation for new modules)
* **Auditor** (Reviews and updates README and LICENSE files to ensure complaince with templates and standards)

### Contribute code

Before you set out to contribute code you will need to have completed a [Contributor License Agreement](http://islandora.ca/sites/default/files/islandora_cla.pdf) or be covered by a [Corporate Contributor Licencse Agreement](http://islandora.ca/sites/default/files/islandora_ccla.pdf). The signed copy of the license agreement should be sent to <mailto:community@islandora.ca>

_If you are interested in contributing code to Islandora but do not know where to begin:_

In this case you should [browse open issues](https://jira.duraspace.org/issues/?jql=project%20%3D%20ISLANDORA%20AND%20resolution%20%3D%20Unresolved%20ORDER%20BY%20priority%20DESC).

If you are contributing Drupal code, it must adhere to [Drupal Coding Standards](https://www.drupal.org/coding-standards); Travis CI will check for this on pull requests. You should also follow the Islandora community's [Git Guidelines and Best Practices](https://github.com/Islandora/islandora/wiki/Git-Guidelines-and-Best-Practices). 

Contributions to the Islandora codebase should be sent as GitHub pull requests. See section _Create a pull request_ below for details. If there is any problem with the pull request we can work through it using the commenting features of GitHub.

* For _small patches_, feel free to submit pull requests directly for those patches.
* For _larger code contributions_, please use the following process. The idea behind this process is to prevent any wasted work and catch design issues early on.

    1. [Open an issue](https://jira.duraspace.org/secure/CreateIssue!default.jspa) and assign it the label of "New Feature" or "Improvement", if a similar issue does not exist already. If a similar issue does exist, then you may consider participating in the work on the existing issue.
    2. Comment on the issue with your plan for implementing the issue. Explain what pieces of the codebase you are going to touch and how everything is going to fit together.
    3. Islandora committers will work with you on the design to make sure you are on the right track.
    4. Implement your issue, create a pull request (see below), and iterate from there.

Developer questions? We have a lot of excellent developer documentation that can be found [here](https://github.com/islandora/islandora/wiki#documentation-for-developers).

#### Issue / Topic Branches

All JIRA issues should be worked on in separate git branches. The branch name should be the same as the JIRA issue number, including all-caps, so ISLANDORA-153, ISLANDORA-118, etc.

Example: `git checkout -b 7.x-ISLANDORA-977` or `git checkout -b 7.x-1.4-ISLANDORA-977`


### Create a pull request

Take a look at [Creating a pull request](https://help.github.com/articles/creating-a-pull-request). In a nutshell you
need to:

1. [Fork](https://help.github.com/articles/fork-a-repo) a given Islandora Foundation component repository at [https://github.com/islandora](https://github.com/islandora) to your personal GitHub account. See [Fork a repo](https://help.github.com/articles/fork-a-repo) for detailed instructions.
2. Commit any changes to your fork.
3. Send a [pull request](https://help.github.com/articles/creating-a-pull-request) to the Islandora GitHub repository that you forked in step 1. If your pull request is related to an existing JIRA issue -- for instance, because you reported a bug/issue earlier -- then prefix the title of your pull request with the corresponding issue number (e.g. `ISLANDORA-123: ...`). The branch name should also correspond to the JIRA issue number.

You may want to read [Syncing a fork](https://help.github.com/articles/syncing-a-fork) for instructions on how to keep your fork up to date with the latest changes of the upstream (official) `islandora` repository.

Community members who have push/merge permissions on a repository should **never** push directly to a repo, nor merge their own pull requests. 

#### Release branch pull requests

The pull request process will roughly look like this:

1. fork from Islandora repo if that has not already been done
2. `git remote add islandora git@github.com:Islandora/islandora_checksum.git`
3. `git pull islandora 7.x`
4. Make changes, commit
5. `git push origin 7.x` and issue a pull request on 7.x
6. `git fetch --all`
7. `git checkout 7.x-1.4` if that does not work, `git checkout islandora/7.x-1.4` then `git checkout -b 7.x-1.4`
8. Make changes/cherry pick/copy changes from earlier, commit
9. `git push origin 7.x-1.4` and issue a pull request on 7.x-1.4

## License Agreements

The Islandora Foundation requires that contributors complete a [Contributor License Agreement](http://islandora.ca/sites/default/files/islandora_cla.pdf) or be covered by a [Corporate Contributor License Agreement](http://islandora.ca/sites/default/files/islandora_ccla.pdf). The signed copy of the license agreement should be sent to <a href="mailto:community@islandora.ca?Subject=Contributor%20License%20Agreement" target="_top">community@islandora.ca</a>. This license is for your protection as a contributor as well as the protection of the Foundation and its users; it does not change your rights to use your own contributions for any other purpose. A list of current CLAs is kept [here](https://github.com/Islandora/islandora/wiki/Contributor-License-Agreements).
