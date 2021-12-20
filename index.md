+++
title = "Monitor web pages"
+++

Monitor web pages and get notified when a page has changed.

~~~
<h2>Features</h2>
~~~

- Scan a list of web pages for changes
- For each page, specify which region of the page has to be checked
- Run the checks on a schedule (specified via a CRON job; powered by GitHub Actions)
- Get notified when a page has changed

~~~
<h2>Use-cases</h2>
~~~

Monitor pages for:

- Updated pricing
- New (financial) reports or other news
- Availability (error detection)
- New job offers
- Updates to legislation

~~~
<h2>Example</h2>
~~~

To check <http://example.com> and <https://bbc.com> for changes, create a new GitHub repository and copy the contents of

<https://github.com/rikhuijzer/Skans.jl/blob/main/.github/workflows/Skan.yml>

into a new GitHub repository.

After doing this, Skans will check the web pages for changes and add an issue comment in your repository every time a page changed.
The downloaded pages are stored in the `skan` branch of your repository to be able to compare them on the next run.
