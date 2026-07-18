<p align="center">
  <a href="README.md"><img src="https://img.shields.io/badge/English-0969da?style=flat-square" alt="English"></a>
  <a href="README.zh-CN.md"><img src="https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-c8102e?style=flat-square" alt="简体中文"></a>
  <a href="README.ja.md"><img src="https://img.shields.io/badge/%E6%97%A5%E6%9C%AC%E8%AA%9E-8250df?style=flat-square" alt="日本語"></a>
</p>

# Python Basic

An introductory Python learning archive containing 100 numbered scripts and nine Chinese-language reference documents.

![Last commit](https://img.shields.io/github/last-commit/NextWeb4/Python-Basic?style=flat-square)
![Repository size](https://img.shields.io/github/repo-size/NextWeb4/Python-Basic?style=flat-square)
![GitHub stars](https://img.shields.io/github/stars/NextWeb4/Python-Basic?style=flat-square)
![Python](https://img.shields.io/badge/Python-practice-3776AB?style=flat-square&logo=python&logoColor=white)

## Archive scope

The repository preserves an early learning sequence rather than an installable Python package. Each numbered script is a standalone teaching example with its own assumptions, input, output, and side effects; the `.docx` files are reference material, not runtime modules.

No supported Python version, dependency manifest, virtual-environment tool, package manager, common entry point, or compatibility promise covers all 100 cases.

## Audited inventory

The refreshed default-branch tree contains **113 files in 1 directory**:

| Format | Count | Role |
| --- | ---: | --- |
| `.py` | 100 | `Python100Cases-master/001.py` through `100.py` |
| `.docx` | 9 | Syntax, library, exercise, ELIZA, crawler-topic, and case reference documents |
| `.md` | 4 | Root multilingual READMEs and repository instructions |

The tree contains no image assets, dependency lockfile, test directory, notebook, packaging configuration, or CI workflow.

## Exercise map

| Range | Representative topics |
| --- | --- |
| `001.py` to `020.py` | loops, arithmetic, dates, strings, sequences, primes, and factorization |
| `021.py` to `040.py` | recursion, number puzzles, list operations, sorting, and matrices |
| `041.py` to `055.py` | classes, scope, functions, random values, and bit operations |
| `056.py` to `065.py` | drawing and GUI-oriented examples |
| `066.py` to `090.py` | lists, queues, linked structures, strings, dictionaries, and small puzzles |
| `091.py` to `100.py` | time, date parsing, text processing, and file input/output |

The ranges are a navigation aid, not a guarantee of steadily increasing difficulty or current best practice.

## Repository map

| Path | Contents and boundary |
| --- | --- |
| `Python100Cases-master/` | The 100 independent numbered scripts |
| `100题.docx` | Reference material associated with the numbered case collection |
| `python基础(1).docx` to `python基础(4).docx`, `Python基础语法.docx` | Introductory Python study documents |
| `Python库.docx` | Library-oriented reference material |
| `ELIZA .docx` | ELIZA-related learning document |
| `爬虫网易云.docx` | NetEase Cloud Music crawler-topic document |

Do not turn the numbered files into hidden shared modules without explicitly redesigning and documenting the collection.

## Historical requirements

Use an interpreter compatible with the selected script, after reading that script in full. The repository does not establish whether the collection targets one Python 2 or Python 3 release.

Verified compatibility exceptions include removed `time.clock()` usage, a third-party `dateutil` import in `095.py`, GUI or drawing examples that need a desktop session, and file-writing behavior in `097.py` through `099.py`. The remaining cases were not executed, so additional requirements may exist.

## Safe per-case workflow

1. Select one numbered file and read its imports, input handling, output, loops, and filesystem operations.
2. Identify interpreter syntax, third-party imports, GUI requirements, and files that may be read or overwritten.
3. Run only that case in a disposable working directory with synthetic input and a recorded interpreter version.
4. Compare observed output with the exercise intent; record failures or modernization choices for that case only.
5. Remove generated files and avoid presenting one successful case as validation of the other 99.

There is no repository-wide run command. A direct interpreter invocation may be appropriate for an inspected case, but it must not be documented as universally compatible.

## Compatibility and side effects

- Removed APIs such as `time.clock()` can fail on current Python versions.
- `095.py` requires `dateutil`, but no dependency manifest or approved version is present.
- GUI and drawing examples may fail in headless sessions or behave differently across platforms.
- `097.py` through `099.py` can create or overwrite files in the current working directory.
- Historical teaching examples may contain defects, outdated idioms, encoding assumptions, or behavior unsuitable for production use.
- Binary `.docx` files may contain links or embedded content and should be opened with normal document-safety precautions.

## Validation boundaries

No repository-wide test, build, lint, or format command was found, and none of the 100 scripts was executed during this documentation audit. No Python version is therefore claimed as fully compatible.

For a changed case, record input, expected and observed output, interpreter version, dependency versions, generated files, and cleanup. Add focused checks for that case without describing them as an archive-wide test suite.

## Maintenance and contributions

Keep changes scoped to one case or one clearly supported documentation correction. Preserve numeric filenames and the independence of examples; do not bulk-modernize 100 scripts to solve one removed API or silently add a dependency.

Keep English, Simplified Chinese, and Japanese READMEs aligned in section order, counts, paths, links, compatibility facts, and side-effect warnings.

## Provenance and license

No repository license file is present. The scripts and bundled study documents may have different origins. Confirm authorship and permission before copying, modifying, or redistributing either code or documents.

## Maintainer

- HaoXiang Huang
- [didadida1688@gmail.com](mailto:didadida1688@gmail.com)
- [Project homepage](https://nextweb4.github.io/)
