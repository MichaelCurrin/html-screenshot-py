# HTML Screenshot PY 🌐 🖼 🐍
> Take fullpage screenshots for a batch of URLs with this easy CLI tool

[![GitHub tag](https://img.shields.io/github/tag/MichaelCurrin/html-screenshot-py?include_prereleases=&sort=semver&color=blue)](https://github.com/MichaelCurrin/html-screenshot-py/releases/)
[![License](https://img.shields.io/badge/License-MIT-blue)](#license)

[![Made with Python](https://img.shields.io/badge/Python->=3.6-blue?logo=python&logoColor=white)](https://python.org)
[![dependency - selenium](https://img.shields.io/badge/selenium-3-blue)](https://pypi.org/project/selenium)
[![dependency - requests](https://img.shields.io/badge/requests-2-blue)](https://pypi.org/project/requests)


## About

An easy Python CLI tool. Provide it a batch of one or more URLs as webpages to scrape. Whether for your own sites or by someone else.

### Formats

It uses two approaches, depending on the format:

- **HTML pages** - The tool will go through each to load the page, take a screenshot of the _entire_ page and save it a PNG file. Using _selenium_.
- **Binary data** - For files with a PDF or image extension, the file will be downloaded directly (for speed and reliability) instead of trying to take a screenshot (which could be massive for PDFs with many pages). Using _requests_.

### Use cases

When you should use this tool:

- **Archive** - Save a once-off copy of an article or a page design that inspires you, before it moves or disappears from the internet. Add as many URLS you like and download all of them.
- **Software development** - Create visual snapshots of a page on your website to track improvements and fixes over time. Or watch how a competitor's website changes.


## Dependencies

See [Requirements](/docs/installation.md#requirements).

## Sample usage

For one webpage, here using https://example.com/ which is a real site you can test against:

```sh
$ python -m htmlscreenshot.scrape 'https://example.com'
```

For multiple pages:

```sh
$ python -m htmlscreenshot ~/path/to/urls.txt
```

Then find your screenshots as PNGs in the project's output directory.


## Documentation

<div align="center">

[![view - Documentation](https://img.shields.io/badge/view-Online_Documentation-blue?style=for-the-badge)](https://michaelcurrin.github.io/html-screenshot-py/ "Go to docs site")

</div>


## License

Released under [MIT](/LICENSE) by [@MichaelCurrin](https://github.com/MichaelCurrin).
