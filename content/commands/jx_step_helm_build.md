---
date: 2019-01-10T15:03:59Z
title: "jx step helm build"
slug: jx_step_helm_build
url: /commands/jx_step_helm_build/
---
## jx step helm build

Builds the helm chart in a given directory and validate the build completes

### Synopsis

Builds the helm chart in a given directory. 

This step is usually used to validate any GitOps Pull Requests.

```
jx step helm build [flags]
```

### Examples

```
  # builds the helm chart in the env directory
  jx step helm build --dir env
```

### Options

```
  -b, --batch-mode                    In batch mode the command never prompts for user input
      --clone-https git@foo/bar.git   Clone the environment Git repo over https rather than ssh which uses git@foo/bar.git (default true)
  -d, --dir string                    The directory containing the helm chart to apply (default ".")
      --git-provider string           The Git provider for the environment Git repository (default "github.com")
      --headless                      Enable headless operation if using browser automation
  -h, --help                          help for build
      --install-dependencies          Should any required dependencies be installed automatically
      --log-level string              Logging level. Possible values - panic, fatal, error, warning, info, debug. (default "info")
      --no-brew                       Disables the use of brew on macOS to install or upgrade command line dependencies
      --pull-secrets string           The pull secrets the service account created should have (useful when deploying to your own private registry): provide multiple pull secrets by providing them in a singular block of quotes e.g. --pull-secrets "foo, bar, baz"
  -r, --recursive                     Build recursively the dependent charts
      --skip-auth-secrets-merge       Skips merging a local git auth yaml file with any pipeline secrets that are found
      --verbose                       Enable verbose logging
```

### SEE ALSO

* [jx step helm](/commands/jx_step_helm/)	 - helm [command]

###### Auto generated by spf13/cobra on 10-Jan-2019
