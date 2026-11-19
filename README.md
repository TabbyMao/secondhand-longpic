# Yard Sale Long Pic

**Live site: https://tabbymao.github.io/secondhand-longpic/**

A small web tool for selling second-hand items. It combines your item photos into compressed long images, with the price and description added under each item, so they are quick to post and load on social media.

## Features

- Upload each item's photos once, by choosing files or dragging them in; several photos of one item sit side by side
- Price and description are added automatically in black text on white, above or below the photos
- Optional note at the bottom of each long image (e.g. "All pickup only")
- Create as many long images as you like, name them (e.g. "Badminton", "Kitchen"), optionally show the name at the top of the image, and pick which items go in each
- Mark an item as sold and it drops out of every long image automatically
- Items are numbered so buyers can say "I want #3"
- Three size presets (Smallest / Balanced / Sharp) to keep files small
- Chinese / English interface; descriptions written in either language are auto-translated into the other

## Privacy

All photos and item details are stored only in your own browser (IndexedDB). Nothing is uploaded to a server. Each person who opens the site has their own separate list. Clearing your browser data, or switching to another device or browser, starts with an empty list.

Auto-translation sends the description text (not photos) to the free [MyMemory](https://mymemory.translated.net/) translation service, which has a daily usage limit.
