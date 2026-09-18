# Rayfield Gen2

Get Started
[Sirius Developer Suite - Rayfield Gen2](https://docs.sirius.menu/rayfield-gen2)

## Load from this GitHub fork

Once this repository has a GitHub Release containing `bundled.luau`, load the
latest stable build directly from GitHub:

```luau
local Rayfield = loadstring(game:HttpGet("https://github.com/errored-app/rayfield-gen2/releases/latest/download/bundled.luau"))()
```

To publish the first bundle, open **Actions**, select **Release Bundle**, choose
**Run workflow**, and run it on `main`. Later stable releases are created when
`version.txt` is changed on `main`. The repository must be public so Roblox can
download the bundle and its image assets without GitHub authentication.

The rolling `dev` build is available after the **Preview Bundle** workflow has run:

```luau
local Rayfield = loadstring(game:HttpGet("https://github.com/errored-app/rayfield-gen2/releases/download/preview/bundled.luau"))()
```


## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for local setup, required checks, and pull-request guidance.

Run `make ci` before opening a pull request. The gate runs formatting, linting, type analysis, tests, and the enforced coverage threshold.

## License

Mozilla Public License 2.0. See [LICENSE](LICENSE).

Copyright (c) 2026 Corridon Capital.
