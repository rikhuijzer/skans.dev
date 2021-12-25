+++
title = "Template repository"
+++

To quickly get started, go to <https://github.com/rikhuijzer/SkansTemplate> and click on "Use this template".

This will copy the files from there and will immediately start to check the webpages <http://example.com> and <https://bbc.com> for changes.
To monitor pages of your interest, go to the file `.github/workflows/Skan.yml` and replace

```julia
pages = [
    WebPage("http://example.com"),
    WebPage("https://bbc.com")
]
```

with pages of your liking.

For example, to check websites `https://a.com`, `https://b.com` and `https://c.com`, change it to:

```julia
pages = [
    WebPage("http://a.com"),
    WebPage("http://b.com"),
    WebPage("http://c.com")
]
```

Don't forget to add commas.

