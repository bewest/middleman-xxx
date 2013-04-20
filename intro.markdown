# How does middleman `link_to` work with `http_prefix`?

My page is hosted at eg, `foo.github.io/foo-bar/`.
Therefore, when serving locally, I need either all links to work from `/` or from `/foo-bar/`.  Currently they work in live mode using `/`.

However, after executing `middleman build`, with an `http_prefix` the output links still look like `/` instead of `/foo-bar/`.

If there is a page in a sub-directory as in `subs/index` a nav bar will need to link correctly back correctly; do I need invent my own custom variable to handle this or does `link_to` cover relative links with an `http_prefix` through configuration?