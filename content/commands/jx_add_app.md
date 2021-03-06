---
date: 2019-01-10T15:03:59Z
title: "jx add app"
slug: jx_add_app
url: /commands/jx_add_app/
---
## jx add app

Adds an app

### Synopsis

Adds an app

```
jx add app [flags]
```

### Options

```
      --alias string        An alias to use for the app (available when using GitOps for your dev environment)
  -b, --batch-mode          In batch mode the command never prompts for user input
      --helm-update         Should we run helm update first to ensure we use the latest version (available when NOT using GitOps for your dev environment) (default true)
  -h, --help                help for app
  -n, --namespace string    The Namespace to install into (available when NOT using GitOps for your dev environment) (default "jx")
      --password string     The password for the repository
  -r, --release string      The chart release name (available when NOT using GitOps for your dev environment)
      --repository string   The repository from which the app should be installed (default specified in your dev environment)
  -s, --set stringArray     The chart set values (can specify multiple or separate values with commas: key1=val1,key2=val2) (available when NOT using GitOps for your dev environment)
      --username string     The username for the repository
  -f, --value stringArray   List of locations for values files, can be local files or URLs (available when NOT using GitOps for your dev environment)
      --verbose             Enable verbose logging
  -v, --version string      The chart version to install
```

### SEE ALSO

* [jx add](/commands/jx_add/)	 - Adds a new resource

###### Auto generated by spf13/cobra on 10-Jan-2019
