# really-small-backpack-example

This is a small tutorial on the very basics of the Backpack module system.

It requires [cabal-install 2.2](https://www.haskell.org/cabal/download.html). 

It is a [multi-package project](https://www.haskell.org/cabal/users-guide/nix-local-build.html#developing-multiple-packages). You can build all the packages from this folder using:

```
cabal v2-build all
```

Any corrections welcome!

# Further resources for learning Backpack

## User guides

- A detailed description in the GHC user guide of [what can be put in a module
signature](https://downloads.haskell.org/ghc/latest/docs/html/users_guide/separate_compilation.html#module-signatures).
This is Backpack seen from the language side.

- [The Cabal user
guide](https://www.haskell.org/cabal/users-guide/nix-local-build-overview.html),
in particular the sections about
[signatures](https://www.haskell.org/cabal/users-guide/developing-packages.html?highlight=backpack#pkg-field-library-signatures)
and
[mixins](https://www.haskell.org/cabal/users-guide/developing-packages.html?highlight=backpack#pkg-field-mixins).
This is Backpack seen from the package manager side.

## The theory behind Backpack

- Edward Z. Yang's [thesis](https://github.com/ezyang/thesis/releases) is quite
readable and gives a good account of the motivations for Backpack.

- Edward Z. Yang's [blog](http://blog.ezyang.com/category/haskell/backpack/).

- Scott Kilpatrick's
[thesis](https://www.reddit.com/r/haskell/comments/e7gopg/new_haskell_phd_thesis_on_backback_foundations/).
Not as directly applicable to the current implementation of Backpack as Edward
Z. Yang's thesis, but useful insights can be gleaned here.

## Other stuff

- The [Backpack](https://wiki.haskell.org/Backpack) and [Module
Signature](https://wiki.haskell.org/Module_signature) entries in the
Haskellwiki.

- I wrote a few Backpack tips & tricks
[here](https://medium.com/@danidiaz/backpacking-tips-3adb727bb8f7) and
[here](https://medium.com/@danidiaz/backpacking-tips-ii-47fa86e5bf2).

- [Example of an abstract package on Hackage which uses
signatures](http://hackage.haskell.org/package/unpacked-containers). Discussed
[here](https://www.reddit.com/r/haskell/comments/8a5w1n/new_package_unpackedcontainers/).

- [A signature for streaming libraries](https://github.com/danidiaz/streamy)

- [picnic: put containers into a backpack](https://kowainik.github.io/posts/2018-08-19-picnic-put-containers-into-a-backpack) [reddit](https://www.reddit.com/r/haskell/comments/98jegn/blog_post_picnic_put_containers_into_a_backpack/) Features an interesting example of abstracting over classes. (See also lesson 5 of this tutorial.)

