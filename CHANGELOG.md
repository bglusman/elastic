# Elastic Changelog

## 2.3.1

* Fix bug where `Elastic.Bulk.update` would throw an error.

## 2.3.0

* Added `Elastic.Bulk` for bulk operations. Currently only supports `create` and `update`. See documentation for more information.
* `Document.API.index` and `Document.API.update` are no longer interchangeable. `update` will now do a partial update to the document, rather than creating a new version of that document.

## 2.2.2

Added `Elastic.HTTP.bulk`.

## 2.2.1

Handle `econnrefused` and `nxdomain` errors gracefully.

## 2.2

Added `Elastic.Document.API.search_query` for better compatibility with [`scrivener_elastic`](https://github.com/radar/scrivener_elastic).

## 2.1

* `Document.API.count` has now been moved to `Document.API.raw_count`. Use `raw_count` if you want to maintain the behaviour from 2.0.
* Added `Elastic.Query` for `Scrivener` compatibility. See the [`scrivener_elastic`](https://github.com/radar/scrivener_elastic) package for more information.

## 2.0

* `Document.API.search` has now been moved to `Document.API.raw_search`. Use `raw_search` if you want to maintain the behaviour from 1.0.

## 1.0

* Initial release.
