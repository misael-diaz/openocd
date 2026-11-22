# Building openocd with GNU Make

First thing you have to do is to get the dependencies sorted out via

```sh
git submodules init && git submodules update
```

If that succeeds you will now have the header files along other files needed to
build the project with handmade Makefiles. If you don't well you won't be able to
compile `src/flash/common.c` because it needs the definitions in the header `jim.h`.

## Patches

Had to patch the `replacements.h` to include header files for low-level IO in GNU/Linux;
otherwise the compilation would fail because it cannot find typical definitions from
`fcntl.h`.
