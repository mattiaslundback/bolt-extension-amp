AMP feed publisher
==================

Creates sitewide and/or contenttype specific accelerated mobile pages for your Bolt website.

After installation, a configuration file will be created as
`app/config/extensions/ampfeed.bolt.yml`, where you can define how the RSS feeds
should be created. Depending on your set up in the extension's configuration,
you can access RSS feeds either by sitewide or contenttype specific URLs:

 - **Site wide**: `/amp/feed.{extension}`
 - **Contenttype**: `/{contenttypeslug}/amp/feed.{extension}`

Where:
  - `{contenttypeslug}` is the slug of your contenttype.
  - `{extension}` is either 'xml' or 'rss'.

See the comments in your `ampfeed.bolt.yml` for more details.

**Tip:** To allow Google to easily find your site's feed, you
should add an autodiscovery link to the `<head>`-section of your site. For
example:

```html
<link rel="amphtml" href="/amp/feed.xml" />
```
