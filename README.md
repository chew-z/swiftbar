![go-bitbar logo](images/logo.svg)


[![Travis Badge]][Travis]
[![Go Report Card Badge]][Go Report Card]
[![GoDoc Badge]][GoDoc]

This repo contains a package for creating [SwiftBar](https://github.com/swiftbar/SwiftBar) plugins in Go.

It is forked by me [chew-z](https://github.com/chew-z) from [go-bitbar](https://github.com/johnmccabe/go-bitbar) and all credits should go there. I have just added logic for Swiftbar's WebView component. And in the future I hope to add some more logic (Swiftbar has some extended capabilities over original Bitbar and xbar (Bitbar reboot)) and push PR.

## Usage

Creating a BitBar plugin is as simple as (see the [godocs](https://godoc.org/github.com/johnmccabe/go-bitbar) for more details):

```go
package main

import "github.com/johnmccabe/go-bitbar"

func main() {
    app := bitbar.New()
    app.StatusLine("Hello")

    submenu := app.NewSubMenu()
    submenu.Line("World!")

    app.Render()
}
```

## Examples

- [vmpooler-bitbar](https://github.com/johnmccabe/vmpooler-bitbar) is used to monitor and manage VMs running on [Puppetlabs vmpooler](https://github.com/puppetlabs/vmpooler)
- [openfaas-bitbar](https://github.com/johnmccabe/openfaas-bitbar) is used to monitor and manage functions running on [OpenFaaS](https://github.com/openfaas/faas)
- *If you are using [go-bitbar](https://github.com/johnmccabe/go-bitbar) please reach out to be added to this list*

[Travis]: https://travis-ci.org/johnmccabe/go-bitbar
[Travis Badge]: https://travis-ci.org/johnmccabe/go-bitbar.svg?branch=master
[Go Report Card]: https://goreportcard.com/report/github.com/johnmccabe/go-bitbar
[Go Report Card Badge]: https://goreportcard.com/badge/github.com/johnmccabe/go-bitbar
[GoDoc]: https://godoc.org/github.com/johnmccabe/go-bitbar
[GoDoc Badge]: https://godoc.org/github.com/johnmccabe/go-bitbar?status.svg
# swiftbar
