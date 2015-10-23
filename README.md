## Getting Started ##
---------------

To get started with this ROM, you'll need to get
familiar with [Git and Repo](https://source.android.com/source/using-repo.html).

To initialize your local repository use a command like this:

    repo init -u git://github.com/Unlegacy-Android/android.git -b aosp-6.0

Then to sync up:

    repo sync

## Submitting Patches ##
------------------
Our ROM is open source, and patches are always welcome!
You can send patches by using these commands:

    cd <project>
    <make edits>
    git add -A
    git commit -m "commit message"
    git push ssh://<username>@gerrit.unlegacy-android.cf:29418:29418/<project> HEAD:refs/for/android-6.0

Register at gerrit.unlegacy-android.cf and use the username that you registered there in the above command

Commit your patches in a single commit. Squash multiple commit using this command: git rebase -i HEAD~<# of commits>

If you are going to make extra additions, just repeat steps (Don't start a new patch), but instead of git commit -m
use git commit --amend. Gerrit will recognize it as a new patchset.

To view the status of your and others patches, visit [Unlegacy-Android Code Review](http://gerrit.unlegacy-android.cf)
