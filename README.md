# nionui-launcher
[![Travis CI](https://travis-ci.org/meyer9/nionui-launcher.svg?branch=master)](https://travis-ci.org/meyer9/nionui-launcher)
[![Appveyor](https://ci.appveyor.com/api/projects/status/96y4nd192p1j779y?svg=true)](https://ci.appveyor.com/project/meyer9/nionui-launcher)

Nion Launcher can launch Python applications based on the [nionui](https://github.com/nion-software/nionui) framework.

What is Nion UI Launcher?
-------------------------
Launch Python GUI apps.

Write to a Python based user interface API.

This is primarily a desktop application framework.

Getting Started
---------------
End users must have a compatible Python version already installed.

Releasing
---------
Specify a git tag by running:
```
git tag -a v1.x.x -m "Description of release"
```

The release will be automatically uploaded to GitHub releases under the specified release version and tag.

## Travis and Appveyor
### Setup
1. Update the GitHub API key in Travis CI by [encrypting the API key](https://docs.travis-ci.com/user/encryption-keys/) and then setting the `deploy.api_key.secure` setting in .travis.yml.
2. Update the Github API key in Appveyor by [encrypting the API key](https://ci.appveyor.com/tools/encrypt) and setting the `deploy.api_key.secure` settting in appveyor.yml.
3. Turn on Travis builds for the nionui-launcher repository by flicking the switch next to the repo name in the Travis account settings.
4. Turn on Appveyor builds for the nionui-launcher repository by clicking the **New Project** button and selecting the repo.

### Notes
- If the PYTHONHOME variable is edited in the xcconfig, make sure to update the sed command in .travis.yml
- [Pre-installed software for Appveyor](https://www.appveyor.com/docs/installed-software/)
