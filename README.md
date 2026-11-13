# blablabear · Picnic on the Moon 🚀

Static English learning site for GitHub Pages. Preserve `assets/blablabear-original.png`: it is the school's original mascot.

## Included

- Lesson 1: 10:00–15:00, seven exercises (Word garden, Story check, True or false, Picture match, Meaning match, Translation match, Fill the gaps) and the video segment.
- Lesson 2: 15:00–20:00, the same activity structure and the second segment.
- Word pronunciation with US English speech synthesis; immediate feedback; automatic local answer saving.
- A **separate PDF results report** for the currently selected lesson, with the student's name and answers.
- Automatic English captions in an overlay, synchronized approximately to timestamps from the teacher's transcript; YouTube captions are also requested when supported. Transcript timestamps are approximate and may not align to the frame. Sound is played directly from YouTube.

## Deploy to GitHub Pages

Extract the archive. Upload `index.html`, `app.js`, `data.js`, `style.css`, `README.md` and the **assets/** directory directly to the repository root. In repository Settings → Pages choose `Deploy from a branch`, `main`, `/ (root)`.

To change question text, translations, answers, or subtitle lines, edit `data.js`. `captions` are `[second_of_full_video, english_caption]` pairs. The student results are kept in `localStorage` on their own browser. A working internet connection is required for YouTube, voice availability depends on the device, and PDF download loads html2pdf.js; the browser's Print → Save as PDF is offered as fallback. The site does not submit student data to a server.

## Repeat exercises

Click **Try this activity again** under any exercise to clear only that exercise and answer again. Click **Start this lesson again** in the results panel to clear the current lesson only; the other lesson is preserved. The site asks for confirmation first. Download the PDF before resetting if you want a record of an earlier attempt.
