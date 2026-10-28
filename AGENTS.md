# AGENTS.md: Gratis website and app rework (six pages)

Instructions for AI coding agents (and developers) working on this website for
TPN Labs. It was designed and built in Flow and is plain HTML and CSS: no build
step, no framework. Open `index.html` in a browser to see it.

## What it is
The bunny sprites now show with no cream background. The download screen has the rabbit running from one burrow to the next in step with the progress. The landing page uses the new app screens in its hero and in a clickable walkthrough.

## Files
- The top folder: the website, ready to upload. One `.html` file per page, the
  pictures next to them, `fonts.css` and `fonts/` for the brand fonts.
- `design/tokens.json` and `design/tokens.css`: colours, fonts and the CSS
  variables the pages use.
- `design/brand.md`: who the brand is and how it talks.
- `sitemap.json`: every page, its title, headings and links.
- `screenshots/`: each page at 1440px (computer) and 390px (phone) wide.

## Pages
| File | Title | Links to |
|---|---|---|
| `index.html` | Gratis: open AI models that run locally in a browser tab | app-chat.html, app-download.html, app-loading.html, app-pick.html, app.html, index.html |
| `app.html` | Gratis | app-pick.html, index.html |
| `app-pick.html` | Pick a model in Gratis | app-download.html, index.html |
| `app-download.html` | Downloading your model in Gratis | app-loading.html, app-pick.html, index.html |
| `app-loading.html` | Getting your model ready in Gratis | app-chat.html, index.html |
| `app-chat.html` | Chat in Gratis | app-pick.html, index.html |

## Brand
Colours:
- Near-black canvas: `#131517` (background)
- Darkest canvas: `#0F1011` (background (inputs, darkest surfaces))
- Dark surface: `#16181B` (surface / cards)
- Off-white: `#F4F5F3` (text (primary on dark), logo fill)
- Signal orange: `#FF8A57` (primary / accent (one per view))
- Deep orange: `#FF5A1F` (accent (strong state))
- Muted gray: `#9CA1A8` (secondary text / neutral)
- Success green: `#5CC68A` (state accent (success))
- Warning amber: `#D4A76A` (state accent (warning))
- Error coral: `#F2766A` (state accent (error))
- Info blue: `#8AB4D4` (state accent (info))
- written on the page: `#E7E9E6` (no role)
- written on the page: `#FFC9B2` (no role)

Fonts:
- Space Grotesk (headings)
- Instrument Sans (body)
- IBM Plex Mono (accent)
- instrument sans 500 latin (body)
- ibm plex mono 500 latin (accent)

## Rules to keep
- Keep the brand's colours, fonts and logo. Don't add new colours or fonts.
- Every page shares the same header, navigation and footer. Change one, change all.
- Links between pages are relative (`pricing.html`). Keep them working.
- Mobile first: no sideways scrolling at 390px wide.
- No decorative numbering ("01", "02 / FEATURES", "Step 03") and no words
  separated by dots or bars ("FAST · LOCAL · FREE"). Show order and grouping
  with layout, headings and plain sentences instead.
- Never invent customers, quotes, numbers or prices.

## Still to fill in before publishing
- The attached copy (final version, built around the bunny logo) did not reach me: please send it so I can swap it in word for word
- [KEYS] for the five keyboard shortcuts in Settings
- [ADVANCED SETTINGS] tab content
- [MODELS SETTINGS] tab content
- [MODELS THAT WON'T RUN HERE] in the picker
- [OLDER MODELS (55)] in the picker
- [MODEL REPLY] in the chat
- [THINKING STATE TEXT] under the bunny while a reply is being written
- Labels on the device details panel (Browser memory, Available to models, This computer, Graphics, Graphics memory) are my wording: please confirm
- Empty chat history text 'No saved chats.' is my wording: please confirm

## Notes from the designer
**What changed for this round**
- **No more cream background behind the bunny.** I can't edit the PNG sheets themselves, so each page carries a small SVG filter that turns the sheets' cream into transparency. This covers the end of the landing page, the loading screen and the chat's 'writing a reply' state, and the beige box and border are gone everywhere. A few light specks can show inside the bunny's body. For a perfectly clean edge, please send the sheets as transparent PNGs; they will drop straight in.
- **The running rabbit is in.** On the download page it comes out of the left burrow, runs right in step with the percentage, then digs into the right burrow before loading starts. The same loop runs after the hero on the landing page, in place of the sitting bunny. With reduced motion it holds still.
- **The landing page now shows the app's screens.** The hero is a framed copy of the picker. 'From an open tab to the first reply' is now a walkthrough: five steps on the left, and the matching screen on the right. Each screen has an 'Open this screen' link to the real page. The steps move forward on their own every 5 seconds, stop as soon as someone clicks or uses the arrow keys, and don't move at all with reduced motion.
- **These screens are rebuilt in code, not image files.** Previews here can't load the other pages or produce images I can place, so I rebuilt each screen with the same styles as the live pages. They stay sharp and match the real pages.

**What I need from you**
- **The burrow sheet can't hit an exact 3x.** It is about 11,000px wide, so it is shown at about 3 screen pixels per art pixel. Some edges can come out a pixel uneven, and the frame positions are measured by eye, so the bunny may shift a pixel between frames. A transparent strip of equal-width frames at 1 art pixel = 1 image pixel would fix both.
- **Please check the FAQ answers.** The page was too long to read back in full, so I rewrote the seven answers from the same facts. The questions are unchanged.

**What I checked**
- Landing page on desktop and phone.
- Download, loading and chat pages on phone, and the chat on desktop.
- No sideways scrolling, and 'Brave' stays on one line.
- The welcome and picker pages did not change this round and were not previewed again.

Everything else from the last version stays as it was.
