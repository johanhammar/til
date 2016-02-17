# Roundup - Unit testing shell scripts

Got a few shell scripts you want to unit test? [Roundup](https://github.com/bmizerany/roundup) Is the right tool.

## Install it

```
$ curl -L https://github.com/bmizerany/roundup/tarball/v0.0.5 | tar xvzf -
$ cd bmizerany-roundup-<sha>
$ ./configure # see --help for options
$ make
$ make install # you may need sudo
```

or if you're on OS X

```
$ brew install roundup
```

## Use it

```
#!/usr/bin/env roundup

describe "tests for foo"

before() {
  #
}

after() {
  #
}

it_should_print_hello_world() {
  test "hello world" "=" "hello world"
}
```
