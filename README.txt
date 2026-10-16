JAN SAMARTH VOTE — complete replacement files

Package contents:
- index.html: replacement single-file site for the existing GitHub Pages repo.
- firestore.rules: rules matching this code.
- README.txt: setup steps and limitations.

ONE-TIME SETUP ON MOBILE
1. Download and unzip this package.
2. In your GitHub repository, open index.html, tap Edit, Select all, and replace it with the contents of the package's index.html. Commit changes.
3. In Firebase Console > Build > Firestore Database > Rules, replace the old rules with firestore.rules from this package and tap Publish.
4. In Firebase Console > Authentication > Sign-in method, make sure Anonymous is enabled.
5. Wait a minute or two and open your GitHub Pages site. Create a test poll, then open the site in a second browser/device to test voting and live results.

IMPORTANT LIMITATIONS
- This is an informal public opinion poll, not an official election system.
- Anonymous Authentication does not prove a real-world person; a user can clear browser data or use another device to get another anonymous UID.
- Vote option records are publicly readable in this free MVP so browsers can calculate live results. Do not use for secret/private ballots or sensitive polls.
- Rules prevent changing/deleting a vote document after creation, and prevent clients from changing poll documents. Test with non-sensitive sample data first.
- The expiry is enforced by the website UI, not a trusted server clock. This is an MVP, not tamper-proof election software.
- Never put Firebase service-account credentials in the HTML. Firebase web config is intended to be public; security depends on Firestore Rules.
