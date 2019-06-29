# Git Achievements

> Git-Achievements records all of the achievements you acquire while using Git. There are over 40 achievements, most with different levels to be achieved.

> If a new achievement is unlocked after a git command is executed, git-achievements will display a message on the console for your enjoyment:

```
********************************************************************************
                            Git Achievement Unlocked!
                                    Caretaker
                    Added a .gitignore file to a repository.
********************************************************************************
```

## GitHub Pages

A log of all of your achievements is kept locally, but you can also publish it to GitHub pages so you can share your achievements (and there is an RSS feed so people can track your achievements).

For example, the original project creator's achievements page is at:

[http://icefox.github.io/git-achievements/][1]

If you are viewing a forked version of git-achievements you want to replace icefox with the GitHub user account you want to see like so:

[http://**skeptycal**.github.com/git-achievements][2]

To push your achievements to GitHub first fork the project on GitHub, create a branch called `gh-pages`, clone _your_ repository and set the following config to true:

```
git config --global achievement.upload "true"
```

When an achievement is unlocked the index.html file will be overwritten, committed, and then a `git push origin gh-pages` will be executed.

## Install

Add git-achievements to your path and alias git to git-achievements. For example add the following to the end of your `~/.bash_profile`

```
export PATH="$PATH":~/git/git-achievements
alias git="git-achievements"
```

You can get your first achievement by running

```
git achievements --help
```

[1]: https://icefox.github.io/git-achievements/
[2]: https://skeptycal.github.io/git-achievements/
