<div align="center">

🖋️ NOTE88

A note-taking app that looks like it was written with a quill. Because some things deserve better than Arial.

</div>

---

👋 Welcome

Every notes app I've used looks the same. White background, gray text field, blue "New Note" button, sans-serif everywhere. They're efficient. They're also soulless. You write your ideas into a spreadsheet, and the spreadsheet stares back.

NOTE88 goes the other way.

It's a text editor that looks like a page torn from a medieval manuscript. The background is parchment — actually three different kinds of parchment, if you want to choose. The fonts are blackletter, gothic, Old English, the kind of lettering monks used in scriptoriums long before "productivity" was a word. Your note appears on the page in a script that makes even a grocery list feel like a decree.

And it works exactly the way you'd expect a modern editor to work. Every keystroke is saved the moment you stop typing. Multiple notes, switched from a small drawer on the right. Export to .txt, import from .txt, everything local, nothing uploaded. There's no account, no sync, no cloud, no password, no "upgrade to unlock unlimited notes."

The one thing that isn't medieval? The wax seal in the bottom-right corner. That's mine. A red blob with MC88 pressed into it, sitting on the page like a scribe signed his work. It drops in when the page loads and stays put, a small declaration that this page belongs to its writer.

It's not a tool for teams. It's not a place to plan your startup. It's a place to write things down — journal entries, fragments of a story, a phone number, a thought that came to you at 2 a.m. and you don't want to lose.

---

<!--
## 📸 Look Inside

<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/note88/raw/main/images/preview-1.png" alt="The editor in the parchment theme" width="100%" />
  <br />
  <sub><b>① Parchment — the default theme</b></sub>
</div>

<br />
<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/note88/raw/main/images/preview-2.png" alt="The drawer with font, size and paper settings" width="100%" />
  <br />
  <sub><b>② The drawer — fonts, size, paper, notes list</b></sub>
</div>

<br />
<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/note88/raw/main/images/preview-3.png" alt="The vintage theme" width="100%" />
  <br />
  <sub><b>③ Vintage — the darker, leathery paper</b></sub>
</div>
-->

---

✨ What you'll find

A page that looks like parchment.
Not a white rectangle pretending to be paper. The background is built from four or five overlapping radial gradients — light patches, dark patches, a warm cream in the middle, a subtle frayed edge around the borders — plus an SVG noise overlay that gives the whole thing the tooth of real paper. There's even a repeating pattern of faint horizontal lines, like a sheet of ruled paper that's been sitting in a drawer for fifty years. It's the same texture you'd find on a letter that was written in 1820 and forgotten in an attic.

Three paper variants.
The default is Parchment — light, warm, creamy, with visible ruled lines. Vintage is darker and browner, the kind of paper that's been exposed to light and air for decades. Scroll is a gradient from a pale top to a deep ochre bottom, as if the sheet had been rolled and the ends had aged differently from the middle. One button in the drawer switches between them, and the choice is remembered.

Eight typefaces, mostly blackletter.
The default is UnifrakturMaguntia — the classic German gothic face, the same family you'd find on the title page of a book printed in 1650. There are seven others: UnifrakturCook, Pirata One, Grenze Gotisch, MedievalSharp, Cinzel Decorative, IM Fell English, and a plain serif for when you just want to read what you wrote. Every font is loaded from Google Fonts, and every one of them renders your note as if it were a page from a manuscript.

Two fields — title and body.
The title sits at the top, larger, in the same script as the body. It gets its own dotted underline, like the header of a letter. The body is a plain text area — no rich text, no bold, no italics, no bullet points, no formatting tools. You type. The words appear. That's it. The editor doesn't get in your way, and it doesn't pretend to be something it isn't.

Autosave that actually autosaves.
Every keystroke fires a timer. Four hundred milliseconds after you stop typing, the current note is written to localStorage — a snapshot of the title, the body, the active note ID, the current font, the current size, and the current paper. Close the tab, reopen the file tomorrow, and your note is exactly where you left it. No save button, no "unsaved changes" indicator, no anxiety.

Multiple notes, listed in the drawer.
The same drawer that holds the font and paper settings also holds your notes. Each note appears as a small card: the title in blackletter, a one-line preview of the body in italic, and a small timestamp in the corner. Click one, and it loads into the editor. The list is sorted by the last time each note was touched, so your most recent work is always at the top.

Export and import as plain .txt.
The Export button takes the current note and downloads it as a plain text file. The title goes on the first line, a blank line after it, then the body. The filename is derived from the title, with invalid characters stripped out. Import does the reverse — you pick a .txt file, NOTE88 reads it, tries to detect a title on the first line, and creates a new note from the contents. Everything stays as plain text. Nothing is embedded, nothing is encoded, nothing is locked into a format.

A wax seal that says it's yours.
In the bottom-right corner there's a red wax seal. It's drawn in SVG — a circle with a displacement filter to make the edges bumpy, an inner pressed disc, two layers of "MC88" text stacked for the engraved effect, a wet highlight in the upper-left. It rotates slightly off-axis and drops in with a spring animation the moment the page loads. It's not a feature. It's a signature — a small, tangible thing that says this page came from somewhere, made by a hand, not scraped from a template.

Keyboard shortcuts, for when you don't want to reach for the mouse.
Ctrl + S forces a save (though the app saves on its own anyway). Ctrl + N creates a new note. Escape closes the drawer. That's the whole list — because everything else you do by typing, and typing is what the app is for.

Everything stays in your browser.
No backend. No server. No request to any API except Google Fonts, and that only loads the typefaces. Your notes never leave your device. Not for sync, not for backup, not for telemetry, not for anything. If you clear your browser data, the notes are gone — which is why the app also lets you export to .txt for safekeeping.

Bilingual by design, but English to the eye.
The interface text — placeholders, buttons, labels — is in English, because the Old English aesthetic is tied to that tradition. But the title and body fields use dir="auto", which means if you type in Arabic or Hebrew, the text will render right-to-left automatically, and the cursor will behave correctly. You can write in Arabic in a blackletter editor, and it will look strange and beautiful at the same time.

---

🧭 How it works

1. Open the file.
One HTML file, no build step, no install, no account. The page loads with the wax seal dropping into the corner, the brand name in the top-left, and a welcome note already typed into the editor.

2. Start writing.
Click on the title or the body. Type. Every keystroke is captured and saved four hundred milliseconds after you stop typing. There is no save button, because there's nothing to press — the note saves itself as you go.

3. Change the typeface, if you want.
Click the hamburger in the top-right. The drawer slides out. In the Typeface dropdown, choose one of the eight fonts. The editor updates immediately, and so does the small preview inside the dropdown itself. The choice is saved.

4. Change the writing size.
The Size slider goes from 18 to 60 pixels. Drag it left for smaller, right for larger. The sizeVal next to it shows the current value in pixels. The title scales with the body — it's always exactly 1.5 times larger.

5. Change the paper.
Three buttons under Paper: Parchment, Vintage, Scroll. Click one, and the whole page retextures. The choice is saved and stays with you.

6. Manage multiple notes.
The Notes section in the drawer shows every note you've written. Click one to load it. The + New button creates a fresh empty note. The small trash icon deletes the current note, with a confirmation prompt first. If you delete the last note, the app creates a new empty one, so you're never left staring at a blank canvas with nothing to type on.

7. Export when you're done.
Click Export .txt to download the current note as a plain text file. The filename is the title, cleaned up for the filesystem. If you don't have a title, it defaults to note.txt.

8. Import when you want something back.
Click Import, and pick a .txt file from your computer. The app reads the first line — if it's short and is followed by a blank line, it becomes the title. Everything after that becomes the body. A new note is created and opened immediately.

9. Close the tab.
Your notes are saved. Your font choice is saved. Your paper choice is saved. Your size is saved. Everything will be exactly where you left it when you come back.

---

🛠️ A few small helps

"Where are my notes saved?"
In your browser's localStorage, on your own device. Nothing is uploaded, nothing is synced, nothing leaves your machine. If you clear your browser data, or open the file on a different device, the notes won't follow you. This is deliberate — a note that stays where you wrote it.

"Can I use this on my phone?"
Yes. The layout adjusts — the editor takes full width, the drawer is a bit narrower, the wax seal shrinks a little. Everything works by touch. The keyboard shortcuts won't apply, but every function is reachable from the drawer.

"The blackletter font is beautiful but hard to read for long texts."
That's a fair point, and it's why there's a Plain · Sans-serif option at the bottom of the typeface dropdown. You can write in UnifrakturMaguntia for the aesthetic, then switch to a plain serif when you want to reread what you wrote. The text itself doesn't change — only how it's rendered on screen.

"Can I add more fonts?"
Yes, but you'll need to edit the file. Near the top of the script there's a FONTS array. Each entry has an id, a name, and a css string with the font-family. Add a new entry, and also add the font to the <link> at the top of the file (the one loading Google Fonts). The dropdown will pick it up automatically.

"Can I add more paper themes?"
Yes. Open the file, find the CSS block that defines --paper-bg for each theme, and add a new one under a new [data-theme="..."] selector. Then add a matching button in the drawer next to the existing three. The rest is automatic — the JavaScript reads the theme name from the button's data-theme attribute.

"Why don't my exports include the fonts or formatting?"
Because a .txt file is plain text. No fonts, no colors, no styling. The blackletter face only exists on the screen. When you export, you get what you wrote — just the words, in the order you wrote them. If you want to preserve formatting, you'd need to export as HTML or Markdown, which isn't built in.

"Can I sync between two devices?"
No. NOTE88 has no sync, no account, no server. The only way to move a note from one device to another is to export it as .txt on one, transfer the file (email, USB, AirDrop, anything), and import it on the other. It takes thirty seconds, and your notes stay under your control.

"Does it work offline?"
Almost. The app itself runs entirely in the browser, no network requests except for Google Fonts. Load the page once with network, and the fonts get cached. After that, the app works fully offline — you can write, save, and export without any connection. The only thing you'll miss without network on first load is the fonts themselves, and the page will fall back to a system serif.

"The wax seal is covering part of my note on small screens."
It is, a little. On phones, the seal shrinks from 104 to 74 pixels and moves closer to the corner, but it still sits on top of the text area. If it bothers you, open the file and change the .seal-wrap CSS — either make it smaller, or change position: fixed to position: absolute and place it inside the drawer instead.

"Is this safe to use for private notes?"
It's as safe as any file on your computer. Your notes are stored in your browser's local storage, on your device, and never transmitted. But local storage isn't encrypted — anyone with access to your browser can read it. If you want encryption, you'd need to encrypt the exported .txt yourself with a tool like GPG or 7-Zip before storing it.

"Why Old English and not just 'antique' or 'vintage'?"
Because blackletter is one specific tradition with a specific history. It's the script of early printed books in Europe, of Bibles, of legal documents, of the first mass-produced writing. Using it in a notes app isn't decorative — it's a claim that what you write deserves the same care that the monks put into their manuscripts.

"Can I write in Arabic with this?"
Yes. The text fields have dir="auto", which means if you type an Arabic character, the field switches to right-to-left direction automatically and your Arabic will render correctly. It will look strange in a blackletter context — but strange in the way that a bilingual manuscript looks strange, which is to say, not strange at all.

"Is there a dark mode?"
Not as a separate theme. But the Vintage paper is dark enough that it reads like an evening companion to the light Parchment. If you want something truly dark, you can edit the CSS and change the background gradients to something with black and dark grey — it's all in one block at the top of the file.

"Does the wax seal do anything?"
No. It's purely decorative. It's a signature — a small, physical-feeling mark that says this page was made by a hand, not generated. If you don't like it, open the file and delete the <div class="seal-wrap"> block. Everything else will keep working.

"Can I add a fourth paper theme?"
Yes. There are three theme blocks in the CSS, each under a [data-theme="..."] selector. Copy one, rename it, adjust the colors, and add a matching button in the drawer with the same data-theme attribute. There's no counter or limit — you can have as many themes as you want.

"Can I use this as a diary?"
Yes, but you'll want to create a new note each day, since there's no automatic dating or daily-note feature. The drawer keeps them all in a list, sorted by the last time you touched them. If you want to browse by date, the timestamp is displayed on each note in the list.

"What happens if I accidentally delete a note?"
There's no undo. Deleting a note removes it from localStorage immediately, and there's no trash or history. If you want to keep a copy, export it as .txt before deleting — or better, don't delete at all, just leave old notes in the list.

"Why is this called NOTE88?"
Because it's a notes app, and 88 is the number I put on all my projects. It's a marker, not a version. There's no NOTE89 coming — this is it.

---

<div align="center">

📞 A question, an idea, a bug?

https://img.shields.io/badge/Email-mohamed005cheikh@gmail.com-d14836?style=flat-square&logo=gmail&logoColor=white
https://img.shields.io/badge/WhatsApp-+222_30_73_64_75-25D366?style=flat-square&logo=whatsapp&logoColor=white
https://img.shields.io/badge/GitHub-mohamed005cheikh--rgb-181717?style=flat-square&logo=github

<br />

Write it down. Keep it.

<sub>© 2026 Mohamed Cheikh — MC88</sub>

<br />
<br />

</div>