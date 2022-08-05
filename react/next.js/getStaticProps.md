# getStaticProps

`getStaticProps` pre-render Next.js pages at build time.

If you need fetch some data from external data source at build time ahead of user's request, `getStaticProps` should be used.

In other words, `getStaticProps` tells Next.js that which page has some data dependencies.

NOTE: `getStaticProps` can only be exported from a `page`.
