Chocolatey Eexport
=================

Export a ps1 script to re-install everything you've installed via chocolatey.

Running ```cex.ps1``` will iterate through your CHOCOLATEY-INSTALL\lib folder, remove duplicates and version numbers, and output a script prepented with ```cinst```

A lib folder with the following:
```
ConEmu.13.12.25.0
ConEmu.13.7.8.0
curl.7.28.1
git.install.1.9.0.20140303
gitextensions.2.47.3
heroku-toolbelt.0.1.0
```

will export a script named ```choco-export.ps1``` to your home directory containing

```
cinst ConEmu
cinst curl
cinst git.install
cinst gitextensions
cinst heroku-toolbelt
```

The inital script came from https://gist.github.com/jongalloway/5f31f9dfaa11e0637868
