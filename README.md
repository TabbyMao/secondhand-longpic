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

## Shared lists

Want to sell things together with friends? Tap **Create shared list**. Your current items are copied to an online list and you get a link like `…/secondhand-longpic/#s-xxxx`. Everyone who opens the link can add items, edit prices and mark things as sold; changes show up for the others within a few seconds. Tap **Back to local list** to return to the list stored on your own device.

Shared lists are stored in a free [Supabase](https://supabase.com) project. A GitHub Action (`.github/workflows/keep-supabase-active.yml`) pings the database every 3 days so the free project is not paused for inactivity.

## Backup

**Export backup** saves every item (photos included), long image, name and note to a `.json` file. **Import backup** loads it back, into either a local or a shared list. Export a backup now and then, especially before long breaks.

## Privacy

By default, all photos and item details are stored only in your own browser (IndexedDB) and nothing is uploaded. Each person who opens the site has their own separate local list. Clearing your browser data, or switching to another device or browser, starts with an empty list.

Shared lists are the exception: their photos and details are uploaded to Supabase. Anyone who has a shared list's link can view and edit it, so only send the link to people you trust.

Auto-translation sends the description text (not photos) to the free [MyMemory](https://mymemory.translated.net/) translation service, which has a daily usage limit.
