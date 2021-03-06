**This project does not accept GitHub Pull Requests**. This is done intentionally,
as it allows us to maintain the entire history of submitted patches in SIT itself. Any
opened Pull Requests will be closed. The contributors will be asked to use our
own merge request procedure (see below).

Our goal is to encourage frictionless contributions to the project. In order to
achieve that, we use Unprotocols' [C4 process](https://rfc.unprotocols.org/spec:1/C4)
as an inspiration. Please read it, it will answer a lot of questions. Our goal is to
merge patches as quickly as possible and make new stable releases regularly.

In a nutshell, this means:

* We merge patches rapidly (try!)
* We are open to diverse ideas
* We prefer code now over consensus later

It is highly recommended to watch [Pieter Hintjens' talk on building open
source communities](https://www.youtube.com/watch?v=uzxcILudFWM) as well as
read his [book on the same
matter](https://www.gitbook.com/book/hintjens/social-architecture/details).

# Submitting an issue

According to C4's [development process](https://rfc.unprotocols.org/spec:1/C4#24-development-process),
the issue should describe a documented and provable. What this means is that an
issue should strive to have a clear, understandable problem statement. Just like
a patch, it SHOULD be titled "Problem: ..." and have a detailed description
describing evidence behind it, be it a bug or a feature request, or a longer
term "exploratory" issue.

Unlike C4, we're not using GitHub (or any other well-known platform) for issues.
Instead, we're using SIT itself. Please refer to [README](https://github.com/sit-it/sit#open-an-issue)
section that covers this process.

# Preparing a patch

According to [patch requirements](https://rfc.unprotocols.org/spec:1/C4#23-patch-requirements),
the patch should be a minimal and accurate answer to exactly one identified and
agreed problem. A patch commit message must consist of a single short (less
than 50 characters) line stating the problem ("Problem: ...") being solved,
followed by a blank line and then the proposed solution ("Solution: ...").

```
Problem: short problem statement

Optional longer explanation of the problem that this patch
addresses, giving necessary details for the reader to be
able to understand it better.

Solution: explanation of the solution to the problem. Could
be longer than one line.
```

# Preparing a merge request

Once you have a branch (BRANCH) with your patch ready:

Run `./scripts/prepare-merge-request <BRANCH>` script 
and either use the suggested text as is or edit it.
Please keep in mind that currently it expects the first
line of your commit to be a one-line problem statement
(it will copy it to the summary), the second line to be
empty and the rest to be a description (you can see
an example right above).

Then, at the end, it will give you a command line
to copy-paste to push the request out.

<img src="https://github.com/sit-it/sit/raw/master/doc/merge_request.gif">
