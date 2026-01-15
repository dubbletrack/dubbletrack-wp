=== Dubbletrack WP ===
Contributors: Dubbletrack. LLC
Tags: dubbletrack
Requires PHP: 7.3
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

Dubbletrack helpers for wordpress sites

[dubbletrack data=] is for injecting raw data

[dubbletrack embed=] is for injecting components from dubbletrack

#### Now Playing Info
`[dubbletrack data="now-playing" key="show-title"]` → currently playing show title

`[dubbletrack data="now-playing" key="show-time"]` → currently playing show’s times

`[dubbletrack data="now-playing" key="artist-name"]` → currently playing artist

`[dubbletrack data="now-playing" key="track-title"]` → currently playing track

`[dubbletrack data="now-playing" key="album-name"]` → currently playing album

#### Now Playing
`[dubbletrack embed="now-playing"]` → now playing component that displays track, show, and show times

#### Station Player
`[dubbletrack embed="station-player"]`

The following additional attributes can also be supplied:

- `background_color` (hex value, i.e. #333)
    - if not supplied, will look for a field on the current page named `dubbletrack_player_background_color`
    - if the above is not available, it will use the player background color set in dubbletrack section of the theme options
- `text_color` (hex value, i.e. #FFF)
    - if not supplied, will look for a field on the current page named `dubbletrack_player_text_color`
    - if the above is not available, it will use the player text color set in dubbletrack section of the theme options
- `highlight_color` (hex value, i.e. #207BF9)
    - if not supplied, will look for a field on the current page named `dubbletrack_player_highlight_color`
    - if the above is not available, it will use the player highlight color set in dubbletrack section of the theme options
- `autoplay` (boolean, i.e. autoplay=”true”)
    - if not supplied, it will not attempt to autoplay

####  Show Player
`[dubbletrack embed="show-player"]`
The following additional attributes can also be supplied:
- `show_id`  The identifier/slug of the dubbletrack show.
    - If not supplied directly, it will look for a field on the current page named `dubbletrack_show_id`
- `background_color` (hex value, i.e. #333)
    - if not supplied, will look for a field on the current page named `dubbletrack_player_background_color`
    - if the above is not available, it will use the player background color set in dubbletrack section of the theme options
- `text_color` (hex value, i.e. #FFF)
    - if not supplied, will look for a field on the current page named `dubbletrack_player_text_color`
    - if the above is not available, it will use the player text color set in dubbletrack section of the theme options
- `highlight_color` (hex value, i.e. #207BF9)
    - if not supplied, will look for a field on the current page named `dubbletrack_player_highlight_color`
    - if the above is not available, it will use the player highlight color set in dubbletrack section of the theme options
- `autoplay` (boolean, i.e. autoplay=”true”)
    - if not supplied, it will not attempt to autoplay on pageload

#### Changing the HTML tag the shortcode uses:

An additional `tag` argument can be supplied to specify the tag instead of the default `figure` tag for embeddables, and `span` tag for data. 



