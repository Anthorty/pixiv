# Pixiv Downloader
---

A simple tool to download all illustrations from specific illustrator.

Download illustrations by **uers\_id**, **daily ranking** or **history ranking**.

Modified `pixiv.py` add a Multi-Picture Switch

---

## Features
- [x] Keep login sessions
  - [x] Local storage
  - [x] Secure storage (not memory safe)
- [x] Update downloaded artists
- [x] Refresh downloaded artists
- [x] Mutil-Language
- [x] Command-line interface


## Usage

```(Python)
pixiv

Usage:
    python pixiv.py
    python pixiv.py <id>...
    python pixiv.py -r [-d | --date=<date>] [-m | --mode=<mode>]
    python pixiv.py -u
Arguments:
    <id>                                       user_ids

Options:
    -r                                         Download by ranking
    -d <date> --date <date>                    Target date
    -u                                         Update exist folder
    -m <mode> --mode <mode>                    Change rank list
                                               mode: [daily, weekly, monthly, male, female, rookie,
                                                      daily_r18, weekly_r18, male_r18, female_r18, r18g]
    -h --help                                  Show this screen
    -v --version                               Show version

Examples:
    pixiv.py 7210261 1980643
    pixiv.py -r -d 2018-01-01 -m monthly
```

## Add a Multi-Picture Switch

You can change `skip_multi` in `pixiv.py` to control skip Multi-Picture

Default `skip_multi=True`

such as GIF or manga

Change `api.py` to control illustrations in per page and  pages

## Screenshot


![img](https://raw.github.com/bebound/Pixiv/master/ScreenShot/4.png)


## Credits
- [Pixiv-API](https://github.com/twopon/Pixiv-API)
- [PixivPy](https://github.com/upbit/pixivpy)
- [pixiv api](https://danbooru.donmai.us/wiki_pages/58938)
- [bebound/pixiv](https://github.com/bebound/pixiv)
