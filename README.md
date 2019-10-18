# Better Shopify Pagination

The built in default pagination in Shopify is ok, however lacks any ARIA markup, so this snippet adds them in.

Simply save `collection-pagination.lquid` to your snippets directory.

Then add `{% include 'collection-pagination' %}` to your collection templates in place of the usual `{{ paginate }}` tag.

*Notes:*

ARIA tags based on [A11y Style Guide's article](https://a11y-style-guide.com/style-guide/section-navigation.html#kssref-navigation-pagination)

Removed the `rel="prev"` and `rel="next"` attributes after reading [this MOZ forum post](https://moz.com/community/q/implementation-of-rel-next-rel-prev) as Shopify already includes the prev/next link tags in the head.

[Removes the "?page=1" parameter](https://medium.com/@stephenkeable/shopify-seo-removing-page-1-from-urls-865d3ff67421) from page one links to prevent duplicate content stuff,
