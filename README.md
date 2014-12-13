eleven-manifest
===============

**This is currently only to be used by Eleven developers with access to the GitLab server.**

At the moment, repo is Linux-only. Once you have your SSH key set up in GitLab, run the following commands:

```bash
curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
chmod a+x ~/bin/repo
echo PATH=\"~/bin:$PATH\" >> ~/.bashrc

mkdir eleven && cd eleven
repo init -u https://github.com/VShell/eleven-manifest
repo sync
```

To fetch updates, simply run `repo sync` again.
