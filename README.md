test rebuild tools
==================

And by "tools" I mean "horrible shell scripts that explode in your face".

Copy `config.example` to `config` and edit.

Then:

```
./make-list > list
./run-rebuild
./print-status -q
```

For each package inspect the build log and run
```
./report-bug build/package_version.build
```

When you lost track of which packages you've already filed bugs against,
run `./hasbug` to filter those out.

