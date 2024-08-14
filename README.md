python-docs-linkcheck
=====================

This repository is dedicated to identifying and fixing issues with links in the [Python Documentation](https://docs.python.org/), as reported by the [Sphinx](https://www.sphinx-doc.org/) linkcheck builder. The project originated from [CPython issue #103484](https://github.com/python/cpython/issues/103484), with the goal of testing patches across various Python versions efficiently, without having to wait for the linkcheck command to complete or relying on personal hardware for multiple documentation builds.

The [linkcheck.yml](.github/workflows/linkcheck.yml) GitHub Actions workflow is designed to automate checks, including link verification, across the supported Python releases—typically the 'main' branch and the two most recent (pre-)releases.

The output from linkcheck is categorized by status (e.g., broken links, permanent redirects, temporary redirects), and committed back to this repository, to enhance readability and streamline the process of identifying and resolving issues.
