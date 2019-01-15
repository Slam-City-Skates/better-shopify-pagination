# Better Shopify Pagination

The built in default pagination in Shopify is ok, however lacks the rel"prev" attributes and also lacks any ARIA markup, so this snippet adds them in.

Simply save `collection-pagination.lquid` to your snippets directory.

Then add `{% include 'collection-pagination' %}` to your collection templates in place of the usual `{{ paginate }}` tag.
