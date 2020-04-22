# Functional Programming workshops

## Haskell as a teaching language

Why?
- Purely functional
- Strongly typed

GHC - industry standard Haskell compiler.

## Install `stack`

Stack is a GHC tool used for building, running, testing, dependencies management and downloading.

http://docs.haskellstack.org/en/stable/install_and_upgrade/

Linux/macOS:
- `curl -sSL https://get.haskellstack.org/ | sh`

Windows:
- binary installer

## Create new project

Open terminal.
In your projects directory type:

`stack new fp`

It creates a subfolder `fp` with following structure:

```
fp
├── ChangeLog.md
├── LICENSE
├── README.md
├── Setup.hs
├── app
│   └── Main.hs
├── fp.cabal
├── package.yaml
├── src
│   └── Lib.hs
├── stack.yaml
└── test
    └── Spec.hs

3 directories, 10 files
```

Go inside: `cd exercises`.

Check the content of all files.

## Try `stack`

`stack setup`

- installs appropriate GHC version (may take a while - 260MB).

`stack build`

- builds (compile and link) current project. Will do the setup if previous step was omitted.

`stack exec -- exercises-exe`

- runs compiled applicaiton

`stack run`

- compiles and runs default executable

`stack ghci`

- runs REPL - interactive interpreter.

## REPL commands

```
:help (:h, :?)
:load (:l)
:reload (:r)
:type (:t)
:info (:i)
:quit (:q)
```

## Important links:

- https://www.haskell.org/ - home page
- https://hoogle.haskell.org/ - documentation
- https://www.stackage.org/ - curated list of compatible packages

## Further reading

[FP.md](docs/FP.md)
