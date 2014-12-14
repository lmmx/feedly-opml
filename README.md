feedly-opml
===========

Storing my Feedly OPML and a searchable tabular listing, [tabular_feeds.tsv](https://github.com/lmmx/feedly-opml/blob/master/tabular_feeds.tsv), made with:

`tabulatedfeeds=$(echo -e "Feed\tFeed URL"; grep '<outline type' feedly.opml | awk 'BEGIN{FS="\""};{print $4"\t"$8}' | sort)`

`echo "$tabulatedfeeds" > tabular_feeds.tsv`
