the-podcast
===========

Generate
--------

```shell
podenco generate the-podcast.yaml output
```

Notes
-----

The podcast audios were created this way:

```shell
echo "The Poscast: Episode One." | espeak --stdin --stdout | ffmpeg -i - -ar 44100 -ac 2 -ab 192k -f mp3 episode1.mp3
echo "The Poscast: Episode Two." | espeak --stdin --stdout | ffmpeg -i - -ar 44100 -ac 2 -ab 192k -f mp3 episode2.mp3
```
