dspljson
========

This is an experimental repository for a JSON dialect of the [Dataset Publishing Language (DSPL)](https://developers.google.com/public-data/). JSON has numerous advantages over XML for client-side parsing, while DSPL is an extensible and robust dataset description format.

At the moment, this repository contains one script: `xml2json`, which reads DSPL XML on `STDIN` and emits JSON on `STDOUT`.

An example translation from the DSPL file `sample.xml` can be found in `sample.json`.

Please note
-----------

This is currently a quick half-hour-hack. `xml2json` does not come close to implementing all of the DSPL specification ([see here for the schema](https://developers.google.com/public-data/docs/schema/dspl9) if you want to help improve `dspljson`).

While this is partially deliberate (I think adding I18N support to the schema adds unnecessary complexity and can be avoided) it's mostly not. If you believe there are important pieces of functionality missing, please fork this repository and issue a pull request.