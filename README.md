# epics-docs

This repository is the source for the top-level documentation site
at [docs.epics-controls.org](https://docs.epics-controls.org).

## Scope

This repository contains user and developer documentation for EPICS,
including guides, explanations, and reference material across EPICS topics.

The published site also carries documentation
built from other repositories, such as EPICS Base,
which appears under `docs.epics-controls.org/projects/`.
This repository doesn't maintain those pages.

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

## Contributing

See [CONTRIBUTING.md](./CONTRIBUTING.md).

## Support

For questions or help, use
[Tech-talk email](mailto:tech-talk@aps.anl.gov), visit the
[mailing lists](https://epics-controls.org/resources-and-support/mailing-lists/),
or join [EPICS Chat](https://epics-controls.org/epics-chat/).
