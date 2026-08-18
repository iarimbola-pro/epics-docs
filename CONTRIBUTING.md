# Contribution guidelines

Found an issue?
Report it on [GitHub Issues](https://github.com/epics-docs/epics-docs/issues)
or email <tech-talk@aps.anl.gov>.

## Pull requests

- If you are new to GitHub's contribution flow,
  see [Collaborating with pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests).
- Keep changes focused
  and separate unrelated concerns into separate pull requests when possible.
- Read the Docs builds a preview of each pull request automatically.
  Once the check passes,
  follow the **Read the Docs** link in the PR checks
  and confirm your change renders as expected.

## Local development

Install dependencies from `pyproject.toml` and run a local preview:

``` console
$ python -m venv .venv
$ . .venv/bin/activate
$ pip install .
$ sphinx-autobuild . ./_build/html
```

Open <http://127.0.0.1:8000> in your browser.
Changes reload automatically.

## Documentation framework

This documentation follows the [Diátaxis framework](https://diataxis.fr/),
organized into:

- **Tutorials** - for learning new concepts
- **How-to guides** - for achieving specific goals
- **Explanations** - for clarifying understanding
- **References** - for looking up information

Organize pages in this order within each topic.
New pages also need a toctree entry (usually in `index.rst`)
or they will not appear in the navigation.

## Style guide

- Write new documentation in [Markdown](https://www.markdownguide.org/basic-syntax/) (`.md`).
  Progressively convert existing reStructuredText pages to Markdown.
- Use [semantic line breaks](https://sembr.org/) ---
  break after sentences and clauses.
- Vale is available for style checks:
  `vale path/to/your/file.md` (optional).

## Adding dependencies

Add new Sphinx extensions to the `dependencies` list in `pyproject.toml`
and to the `extensions` list in `conf.py`.

## For maintainers

- Merge using merge commits (not fast-forward).
- Refrain from pushing to contributors' branches.
