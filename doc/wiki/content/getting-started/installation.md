Pre-requisite:

- [Stack](https://docs.haskellstack.org/en/stable/install_and_upgrade/)

- [Git](https://git-scm.com/)

## Installing Noc

If you're using Linux, macOS (or BSD) (*For the Windows users, use [WSL](https://docs.microsoft.com/en-us/windows/wsl/about)*)

**Get the latest version**

```sh
git clone https://github.com/noc-lang/noc && cd noc
```

**Get the Noc v0.1.0.0**

Download from this [release](https://github.com/noc-lang/noc/releases/tag/v0.1.0.0).

**Install Noc (for all versions)**

```sh
make install
```

## Building locally the Noc Manual (only the v0.1.0.0)

There is a tool written in Noc to generate the Noc Manual (includes noc and nocdoc documentation) ([nocdoc](https://github.com/noc-lang/nocdoc))

You can build the manual with the Makefile, but you have to install in the first place the pandoc tool to convert some Markdown snippets in HTML.

```sh
make build_doc
```

All HTML files are generated in a ``manual`` folder. The starting page is ``manual/index.html``

> You can also document your own functions, check the [nocdoc documentation](nocdoc/index.html) of this tool.

## Updating and Uninstalling

We can reinstall Noc with the latest version.

```sh
git clone https://github.com/noc-lang/noc && cd noc

# or if the repos is already cloned
git pull origin main
```

then

```sh
make update
```

To uninstall Noc.

```sh
make uninstall
```

## Troubleshooting

To check if we have Noc installed:

```sh
noc --version
```
