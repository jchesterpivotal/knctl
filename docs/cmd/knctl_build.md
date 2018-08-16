## knctl build

Build source code into image

### Synopsis

Build source code into image

```
knctl build [flags]
```

### Examples

```

  # Build Git repository into an image in namespace 'ns1'
  knctl build -b build1 --git-url github.com/cppforlife/simple-app --git-revision master/head -i docker.io/cppforlife/simple-app -n ns1
```

### Options

```
  -b, --build string             Specified build
  -d, --directory string         Set source code directory
      --generate-name            Set to generate name
      --git-revision string      Set Git revision (examples: https://git-scm.com/docs/gitrevisions#_specifying_revisions)
      --git-url string           Set Git URL
  -h, --help                     help for build
  -i, --image string             Set image URL
  -l, --local-registry           Use local registry
  -n, --namespace string         Specified namespace ($KNCTL_NAMESPACE)
      --service-account string   Set service account name for building
      --template string          Set template name
      --template-arg strings     Set template argument (format: key=value) (can be specified multiple times)
      --template-env strings     Set template environment variable (format: key=value) (can be specified multiple times)
```

### Options inherited from parent commands

```
      --column strings      Filter to show only given columns
      --json                Output as JSON
      --kubeconfig string   Path to the kubeconfig file ($KNCTL_KUBECONFIG) (default "/Users/pivotal/.kube/config")
      --no-color            Disable colorized output
      --non-interactive     Don't ask for user input
      --tty                 Force TTY-like output
```

### SEE ALSO

* [knctl](knctl.md)	 - knctl controls Knative resources (annotate, build, create, curl, delete, deploy, install, list, logs, open, route, tag, uninstall, untag, version)

