# Better Shopify Pagination

The built in default pagination in Shopify is ok, however lacks any ARIA markup, so this snippet adds them in.

Simply save `collection-pagination.lquid` to your snippets directory.

Then add `{% include 'collection-pagination' %}` to your collection templates in place of the usual `{{ paginate }}` tag.

*Notes:*

ARIA tags based on [A11y Style Guide's article](https://a11y-style-guide.com/style-guide/section-navigation.html#kssref-navigation-pagination)

Removed the `rel="prev"` and `rel="next"` attributes after reading [this article](https://moz.com/community/q/implementation-of-rel-next-rel-prev)
