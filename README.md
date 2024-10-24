Conferences
===========

A community-curated list of Software Development conferences around Spain.

Adding a conference
-------------------

Send a pull-request which adds a file to the `_conferences/` directory
with a new file representing the conference. The file should be named
with the conference name, the year, and with an `.md` extension (for
example, `my-cool-conference-2019.md`).

The contents of the file should use the following template:
```
---
name: "CoolConf"
website: http://es.coolconf.com/2019/
twitter: http://twitter.com/coolconf/
location: Illescas, Toledo, Spain

date_start: 2019-10-18
date_end:   2019-10-30

cfp_start: 2019-06-20  # Optional
cfp_end:   2019-07-21  # Optional
cfp_site: http://es.coolconf.com/2019/call-for-papers/ # Optional, will default to website
---
```

*Note: Do not include the location of the conference in the name. The above conference is often referred to as "Devfest Madrid", but we will always render the location with the name so it is redundant.*


Running locally
---------------

## Traditional

```
bundle install --path vendor/bundle
bundle exec jekyll serve
```

On debian you need `sudo apt install ruby-bundle ruby-dev`

Once running the site can be opened at [http://localhost:4000](http://localhost:4000).

## Docker

Compile image

```
docker build -t tech-conferences-spain-app .
```

Run image

```
docker run --rm -it -v ./:/usr/src/app -p 4000:4000 -p 35729:35729 tech-conferences-spain-app bundle exec jekyll serve
```

Once running the site can be opened at [http://localhost:4000](http://localhost:4000).

License
-------

All content is [CC0][1].


 [1]: https://creativecommons.org/publicdomain/zero/1.0/
