# Notulia — problem reports

This repository receives the problem reports that [Notulia](https://github.com/DiamondForgeFr/notulia-releases) users choose to send from inside the app. It holds no code.

## How a report gets here

When something fails, Notulia's notification center offers **Report this problem**. The app builds the report on the user's machine, **shows it in full**, lets the user edit or delete any part of it, then opens this page in the browser with the report pre-filled. Nothing is sent until the user submits the issue with their own GitHub account. The app holds no token and never posts on anyone's behalf.

Before opening the page, the app looks for an issue carrying the same fingerprint (`notulia-fp:…`). If the problem was already reported, it offers that issue instead, so the user can add to it.

## What a report contains

- the message the app showed (its text and the identity of the situation, with identifiers removed);
- the version, the operating system, and which feature families the build ships;
- the last lines of the app's diagnostic log, with home-folder paths, e-mail addresses and identifiers removed;
- whatever the user chose to write.

## What a report never contains

No recording, no transcript, no note, no meeting title, no attendee, no API key. The app does not put them in the report, and the user sees every line before sending.

Everything posted here is **public**. If you spot personal information in a report, please say so in a comment and it will be removed.

## What happens next

Reports are triaged: checked, reproduced when possible, linked to the internal ticket that fixes them, and closed with a link to the version that ships the fix. Duplicates are closed in favour of the first report.
