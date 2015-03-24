# SEO-Unit-Tests
Unit testing for on-page SEO

This is a 'work-in-progress' project that is designed to help build on-page SEO best practices in your software development life cycle and continuous integration/testing environment.

Things to unit test for SEO
---------------------------

(For each page)

1. META 'Description' element MUST be present.
2. META 'Keywords' element MUST be present.
3. `<title>` element MUST be present.
4. If `<link rel="canonical">` element exists, the `href=".."` attribute MUST not be empty.
5. META 'Keywords' MUST not be empty.
6. META 'Description' length MUST be => 150 characters and <= 160 characters.
7. HTTP GZIP compression MUST be enabled (http://www.whatsmyip.org/http-compression-test/).
8. MUST have a `<h1>` element that is not empty.
9. MUST not have any outbound links that 404 in terms of status code response.
10. MUST pass W3C Validation. (http://validator.w3.org/)
11. All `<img>` elements MUST have the `alt=".."` attribute set and not empty.
12. All `<img>` elements MUST have the `title=".."` attribute set and not empty.

(Not-per-page)

1. Server MUST have a `/robots.txt` file.
