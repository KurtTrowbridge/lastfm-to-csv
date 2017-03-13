lastfm-export
=============

Currently exports play count and song title correctly. Artist does not export to CSV correctly; artist currently repeats based on [last.fm API's default *limit* of 50](http://www.last.fm/api/show/user.getTopTracks), but lowering that number (ideally to 1; see js/lastfm-export.js:24 for commented-out example) causes errors.

Compare to XML output: http://ws.audioscrobbler.com/2.0/?method=user.gettoptracks&user=trombone13&api_key=974a5ebc077564f72bd639d122479d4b&period=7day