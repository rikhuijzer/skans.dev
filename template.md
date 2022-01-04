+++
title = "Template repository"
+++

~~~
<h2>Template</h2>
~~~

To quickly get started, go to <https://github.com/rikhuijzer/SkansTemplate> and click on "Use this template".

This will copy the files from there and will daily check the webpages <http://example.com> and <https://bbc.com> for changes.
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
    WebPage("https://a.com"),
    WebPage("https://b.com"),
    WebPage("https://c.com")
]
```

Don't forget to add commas.

To change the interval to check for changes, change the line containing `- cron: '00 16 * * *'`.
See [Wikipedia - Cron](https://en.wikipedia.org/wiki/Cron) for more information about how to specify intervals.

