feedly-opml
===========

Storing my Feedly OPML and a tabular listing, [tabular_feeds](https://github.com/lmmx/feedly-opml/blob/master/feedly.opml), made with:

`grep '<outline type' feedly.opml | awk 'BEGIN{FS="\""};{print $4"\t"$8}' | sort > tabular_feeds.tsv`
