# ShowMe
A browser based media server with no options what so ever.

I don't want all these options, it will just confuse my spouse.

This project contains one executable called Fetcher. Run it with:
```
$ ./fetcher your-video-root-directory
```

Based on the required directory structure and the WebM files it contains it
will:
# create a bunch of JSON files containing show information.
# creates a subdirectory for every episode.
# creates, in every directory, an `index.html`.

These `index.html` files are 'apps'. There's a:
# Shows app
# Show app
# Season app
# Episode app

Next spin up your favourite webserver with the correct document root and you're
ready to watch, in your browser.

# Required directory structure.
```
shows
|-- Name
|    |-- 1
|    |   |-- Name 1x01-Title.webm
|    |   +-- Name 1x02-Title.webm
|    |-- 2
|    |   |-- Name 1x01-Title.webm
|    |   +-- Name 1x02-Title.webm
|
|-- Other Name
     |-- 1

```
