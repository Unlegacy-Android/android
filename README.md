Getting Started
---------------

To get started with Android, you'll need to get
familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

To initialize your local repository using theese trees, use a command like this:

    repo init -u git://github.com/Unlegacy-Android/android.git -b aosp-9.0

Then to sync up:

    repo sync


The following additional flags can be used to optimize repo sync, saving bandwidth and disk space:

    --no-clone-bundle     disable use of /clone.bundle on HTTP/HTTPS
    -c, --current-branch  fetch only current branch from server
    --no-tags             don't fetch tags
    -j JOBS, --jobs=JOBS  projects to fetch simultaneously (default 4)
