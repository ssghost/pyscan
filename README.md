<h1 align="center"> 🐍 Pyscan </h1>

![CI](https://github.com/aswinnnn/pyscan/actions/workflows/CI.yml/badge.svg) ![Liscense](https://img.shields.io/github/license/aswinnnn/pyscan?color=ff64b4) [![PyPI](https://img.shields.io/pypi/v/pyscan-rs?color=ff69b4)](https://pypi.org/project/pyscan-rs) [![](https://img.shields.io/crates/v/pyscan?color=ff64b4)](https://crates.io/crates/pyscan) [![GitHub issues](https://img.shields.io/github/issues/aswinnnn/pyscan.svg?color=ff69b4)](https://GitHub.com/aswinnnn/pyscan/issues/) [![Top Language](https://img.shields.io/github/languages/top/aswinnnn/pyscan?color=ff69b4)](https://img.shields.io/github/languages/top/aswinnnn/pyscan)

<h4 align="center"> 

<img src="https://media.discordapp.net/attachments/1002212458502557718/1107648562004758538/pyscan.png?width=779&height=206">

</h4>

<h5 align="center"> <i>A dependency vulnerability scanner for your python projects, straight from the terminal.</i> </h5>

+ 🚀 blazingly fast and efficient scanner that can be used to scan large projects fairly quickly.
+ 🤖 automatically uses `requirements.txt`, `pyproject.toml` or straight from the source code (though not reccomended)
+ 🧑‍💻 easy to use, and can be integrated into existing build processes.
+ 💽 In its very early alpha stage, so some features may not work correctly. PRs and issue makers welcome.

## 🕊️ Install

```bash
pip install pyscan-rs
```
look out for the "-rs" part
or

```bash
cargo install pyscan
```

or check out the [releases](https://github.com/aswinnnn/pyscan/releases).

## 🐇 Usage

Go to your python source directory (or wherever you keep your requirements.txt/pyproject.toml) and run:

```bash
pyscan
```
or
```bash
pyscan -d path/to/src
```

that should get the thing going.
Here's the order of precedence for a "source" file:

+ requirements.txt
+ pyproject.toml
+ your python source code (.py) [highly not reccomended]

Any dependencies without a specified version defaults to its latest stable version. **Make sure you version-ize your requirements** and use proper [pep-508 syntax](https://peps.python.org/pep-0508/).

## 🦀 Note

pyscan uses [OSV](https://osv.dev) as its database for now. There are plans to add a few more.

pyscan doesn't make sure your code is safe from everything. Use all resources available to you like Dependabot and other github features.

## 🐰 Todo

- [x] get it working.
- [ ] add  tests.
- [ ] more advisory databases.
- [x] query individual dependencies. [v0.1.1]
- [ ] perfomance optimizations.
- [ ] scan docker images
- [ ] scan code quality. 

## 🐹 Sponsor

While not coding, I am a broke high school student with nothing else to do. I appreciate all the help I'm worthy of.
