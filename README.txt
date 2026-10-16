JAN SAMARTH VOTE — FINAL PACKAGE

Files:
- index.html: complete website UI + Firebase logic
- firestore.rules: matching Firestore rules

Mobile deployment:
1. GitHub repository: https://github.com/vg9068237-pixel/Jan-Samrath-Vote
2. Open index.html, tap pencil/Edit, replace entire contents with index.html from this package, Commit changes.
3. Firebase Console > Build > Authentication > Sign-in method: enable Anonymous.
4. Firebase Console > Firestore Database > Rules: replace rules with firestore.rules contents, Publish.
5. Wait a few minutes, then open:
   https://vg9068237-pixel.github.io/Jan-Samrath-Vote/

Features:
- Create public polls with state, district, tehsil/block, locality
- Search polls, filter by state/district
- WhatsApp share
- Live vote totals and percentages, trending mode
- Anonymous Firebase authentication

Important limitations:
- This is a public opinion survey, not an official election/voting system.
- Anonymous accounts can be recreated, so one vote per UID is not one vote per real person.
- Location fields are self-reported and do not verify residency.
- Vote documents are publicly readable to allow live result counts. Do not use for sensitive/private polls.
- Rules prevent edits/deletes from the client; an admin/moderation workflow is not included.
