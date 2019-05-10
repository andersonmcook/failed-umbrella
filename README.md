# FailedUmbrella

Run
```sh
$ mix new ./apps/foo.bar --sup --module Bar --app bar
```

Result
```
* creating README.md
* creating .formatter.exs
* creating .gitignore
warning: redefining module FailedUmbrella.MixProject (current version defined in memory)
  /Users/my/path/failed-umbrella/mix.exs:1

Error while loading project :umbrella_check at /Users/my/path/failed-umbrella
* creating mix.exs
* creating config
* creating config/config.exs
* creating lib
* creating lib/bar.ex
* creating lib/bar/application.ex
* creating test
* creating test/test_helper.exs
* creating test/bar_test.exs

Your Mix project was created successfully.
You can use "mix" to compile it, test it, and more:

    cd ./apps/foo.bar
    mix test

Run "mix help" for more commands.
```

Run
```sh
$ iex -S mix
```

Result
```
** (Mix) Could not start application foo.bar: could not find application file: foo.bar.app
```

Tree
```
bar
├── elixir
└── logger
    └── elixir
```
