JAN SAMARTH VOTE — COMPLETE STARTER (Hindi)
============================================
Is package mein Firebase-connected frontend ka code, Firestore rules aur poora mobile setup guide hai.
Aapko apne Firebase project ka web config khud bharna hoga. Kisi aur ke account ki jagah hum live publish nahi kar sakte.

ZIP CONTENTS
- index.html: responsive website, public polls, vote/results, sharing, search, SEO metadata, 3 ad placeholders
- firebase/firestore.rules: starter security rules
- SETUP-HI.txt: mobile setup steps
- ADS-HI.txt: ad placements guidance

IMPORTANT
This is a Firebase-ready starter, not a certified election system. Before a wide public launch, review rules and test with multiple phones. A client-side voting app can still be abused; for stronger vote integrity, move vote counting to a trusted Cloud Function and add App Check, moderation, backups and rate limits. Do not describe informal polls as official election results.

PUBLISH
1) Upload index.html to the root of GitHub repository jan-samarth-vote and commit.
2) GitHub repo > Settings > Pages > Deploy from branch > main > /(root) > Save.
3) Follow SETUP-HI.txt to create Firebase project, Authentication, Firestore and Web App.
4) Replace PASTE_ placeholders in index.html with the web app config.
5) Publish the Firestore rules from firebase/firestore.rules in Firebase Console > Firestore Database > Rules.
6) Firebase Authentication > Sign-in method > enable Anonymous.
7) Open published website from two different phones/browser profiles and test creating a poll, voting, and results.

Do not put Firebase service-account private keys in HTML or GitHub. The web config is intended for client use; Firestore rules protect the database.
