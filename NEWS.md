CHANGES IN 0.6
==============

- **SECURITY**: Chat was vulnerable to XSS attacks. Update as soon as
                possible.

- Feature: [**more plugins**](https://github.com/breunigs/ingress-intel-total-conversion/tree/gh-pages/plugins#readme)
    - weakened portals: highlights portals with few resonators or ones
                        that are decayed, making it easier to see where
                        to attack or defend
    - draw tools: allow you to draw things on the map, making it easier
                  to plan your next big field
- Feature: chat now has a tab that shows all automated messages, not
           only the last one per user
- Feature: render lines between portals and their resonators
- Change: resonators are only re-rendered on demand, could improve per-
          formance
- Change: AP Gain now also includes gains by deploying resonators
- Change: portal images are not shrinked instead of cut in preview
- Bugfix: styling issues in sidebar (by cmrn)
- Bugfix: “field decayed” and similar messages were not shown
- Bugfix: tooltips have broken alignment sometimes (by saithis)
- Bugfix: chat sometimes didn’t warn if message didn’t went through
- Bugfix: base layer was not saved properly
- Bugfix: avoid zooming to invalid lat/lng, crashing the browser



CHANGES IN 0.5 / 0.51
---------------------

- Feature: draw resonators on map on high zoom levels (by Xelio)
- Feature: show AP if portal is taken down (by Pirozek)
- Feature: collapsible sidebar (by cmrn)
- Feature: fields connected to portal (by phoenixsong6)
- Feature: Permalink feature
- Feature: chat now more copy&paste friendly (by scrool)
- Feature: display max. energy for portal (by scrool)
- Feature: auto-reload if page states your account is not enabled for
           Ingress
- Feature: You are now alerted if some of the resources fail to load
- Change: portal level should now stand out better against more
          backgrouds (by jonatkins)
- Change: increased hack range from 35m to 40m
- Change: Sidebar now semi-transparent, just like chat (by cmrn)
- Change: portals are now sized according to their level (by OshiHidra)
- Change: resonators are now more aligned to their octant (thanks
          Worros for helping confirming the slot-to-octant matching)
- Change: release versions are now put in `dist/`. This should avoid
          update issues in the future.
- Bugfix: entities would be drawn again if they were hidden while using
          the map
- Bugfix: Python 3+ now required for building to fix encoding issues
- Bugfix: portal mod rendering of unclaimed portals wrong
- Bugfix: chat/sidebar arrows have gap or overlap (by mledoze)
- Bugfix: entities invisible after hiding some of them
- Bugfix: some portals in automated view were not clickable
- Bugfix: resonators + nicks were sometimes misaligned
- Bugfix: portal mod boxes sometimes misaligned
- Plugin: guess-player-levels now also shows guessed level in tooltip


Additional fixes in 0.51:
- Bugfix: sidebar not visible in Chrome
- Bugfix: layer chooser not usable if sidebar collapsed
- Bugfix: range link not working



CHANGES IN 0.4
--------------

- Feature: display resonator charge percentage in tooltip (by Xelio)
- Feature: display resonator level in reso bar (by JasonMillward)
- Feature: portals may be filtered by level (using the layer switcher)
- Feature: build script in Python (by epf)
- Feature: plugins
- Change: Portal mods are colored according to their rare-ness (by OshiHidra)
- Change: nick highlight in chat now case-insensitive
- Change: +/- zoom buttons visible by default now
- Bugfix: title bar text broken
- Bugfix: rename cardinal to octant (by mledoze)
- Bugfix: Chat display broken in Opera
- Bugfix: Chat tab completion in Chrome
- Bugfix: wrong timestamps displayed in chat input bar
- Bugfix: don’t autobuild when git meta info changes (by ZauberNerd)
- Bugfix: resistance owned portals had wrong border when viewing the full image


CHANGES IN 0.3
--------------

- Feature: more info for shields in tooltip (by JasonMillward)
- Feature: pretty display for redeemed codes (by integ3r)
- Change: Portal details are now scrollable when height is too small
- Change: explain the meaning of the links display in tooltip
- Bugfix: appear less greedy in Chrome when asking permission (by epf)
- Bugfix: Geosearch broken for non-ASCII chars
- Bugfix: fix spelling of Niantic (by Bananeweizen)
- Bugfix: fix spelling in README (by epf)
- Bugfix: report portal displayed wrong longitude
- Bugfix: timestamps in chat were displaying seconds instead of minutes
- Bugfix: level/ap calculations for level 8 players

If your version appears broken, please update before reporting an issue.
Also clean your cache, this can usually be done with ctrl + shift +
clicking the reload button. If your problem persists, please open a new
issue.
