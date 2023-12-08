# A simple Spin HTTP component in Python

This project showcases how to do internal HTTP routing in a Spin Python application. It is similar to the [Spin JS router](https://developer.fermyon.com/spin/v2/javascript-components#routing-in-a-component) as well as the Django router.

If you are interested in _extrnal_ routing (where the routing table is declared in the `spin.toml`), the [Application Structure guide](https://developer.fermyon.com/spin/v2/spin-application-structure) covers this, as does [the documentation for Spin configuration](https://developer.fermyon.com/spin/v2/manifest-reference).

This uses the absolutely fantastic [http_router](https://pypi.org/project/http-router/) project. You will likely want to reference the API docs:

* https://github.com/klen/http-router

## Prerequisites

* [Spin](https://developer.fermyon.com/spin)
* [pipenv](https://pipenv.pypa.io/en/latest/index.html)

## Installing

* Install the dependencies with `pipenv update`
* Build with `spin build`

```
$ pipenv update
$ spin build
```

## Running

### Locally
```console
$ spin up
```

You can then try out some example queries:
* `curl localhost:3000/`
* `curl -XPOST -d "TEST" localhost:3000/post`
* `curl localhost:3000/queryparams\?foo=bar\&foo2=bar2`

### On Fermyon Cloud

```console
$ spin deploy
```

You can then adapt the above `curl` requests to the URL Fermyon Cloud returned to you.

