rdeps scans GOPATH for all reverse dependencies of a set of Go
packages.

# Installation

```
go get github.com/dominikh/go-rdeps
```

# Usage

Invoke `go-rdeps` with zero or more arguments that are Go packages to
print their reverse dependencies.

Alternatively, use the `-stdin` flag and provide a list of Go packages
on standard input.

See `go-rdeps -h` for all flags.

# Example

```
$ go-rdeps database/sql 2>/dev/null | head -5
github.com/GoogleCloudPlatform/golang-samples/docs/appengine/cloudsql
github.com/lxc/lxd/lxd
github.com/mattn/go-sqlite3/sqltest
github.com/mgutz/dat/sql-runner
github.com/mgutz/dat
```
