# Repository instructions

## 1. Project structure
- `Python100Cases-master/001.py` through `100.py` are independent introductory exercises.
- Root `.docx` files are reference material and are not Python package modules or runtime dependencies.
- The repository is a historical learning archive, not an installable package.
- Keep the audited inventory of 100 `.py`, 9 `.docx`, and 4 `.md` files synchronized with the complete tree.

## 2. Run commands
- No repository-wide run command or supported Python version was found.
- Review and run only one numbered script at a time with a compatible interpreter; use a disposable working directory for file-writing cases `097.py` through `099.py`.

## 3. Test commands
- No test command was found in the current repository; add one before claiming automated regression coverage.
- For a changed exercise, add or record focused input/output checks without claiming all 100 cases were validated.

## 4. Build commands
- No build command was found; the scripts and reference documents are not packaged artifacts.
- Do not introduce packaging or a site generator for a single exercise change.

## 5. Code style
- Keep the exact centered Shields language selector in all root README files; its visible native labels are `English`, `简体中文`, and `日本語`.
- Keep all three README versions aligned in section order, counts, paths, links, badge URLs, compatibility facts, and side-effect warnings.
- Preserve each case as a standalone teaching example and keep its numeric filename stable.
- Modernize removed APIs only in a deliberately scoped case, with behavior documented before and after.
- README files use UTF-8 Markdown. No lint/format command was found in the current repository.

## 6. Module boundaries
- Each numbered script owns its inputs, side effects, and demonstration output.
- Do not create hidden shared state or imports between numbered cases unless the collection is explicitly restructured.
- GUI, third-party dependency, and file-I/O cases must remain clearly identified.

## 7. Prohibited changes
- Do not claim one Python version supports all cases without running them.
- Do not bulk-rewrite 100 educational scripts to fix one compatibility issue.
- Do not commit files produced by `097.py` through `099.py` unless they are intentionally added fixtures.
- Do not silently add `dateutil` or another dependency without a manifest, license review, and scoped need.

## 8. Completion criteria
- A changed case has its expected input, output, side effects, and interpreter version recorded and verified.
- Every README retains the detailed inventory, exercise map, per-case workflow, compatibility exceptions, validation limits, provenance, and maintenance guidance.
- Documentation maps real numbered files, multilingual links work, and reference documents remain unchanged.
- Any new dependency or generated file is justified and explicitly documented.

## 9. Review criteria
- Verify the language selector renders through GitHub without browser-translatable text and all three README versions keep the same facts, commands, links, and images.
- Review each changed script from input through state changes to output and filesystem effects.
- Check removed APIs, integer/float behavior, GUI requirements, third-party imports, and current-working-directory assumptions.
- Reject package-wide compatibility or test claims based on a small sample.

## 10. Common risks
- Historical examples may use removed APIs such as `time.clock()` or contain known teaching-code defects.
- Case 095 needs an undeclared third-party package, and GUI examples may fail in headless environments.
- File-I/O examples can overwrite local files in the current directory.
- No license file clarifies redistribution rights for code or bundled documents.
