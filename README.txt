THE COURTROOM — account-based prototype

Preview: open index.html in a modern browser.
- Create a normal account with username/password.
- Sign in and submit a message.
- Sign out, then sign in as username arealpips. On first sign-in, the password entered becomes the demo admin password for this browser.
- The admin inbox can read submissions and reply; users see replies in My conversations.

SECURITY / PRODUCTION NOTICE
This is a browser-only prototype. Accounts, password hashes and messages are stored in localStorage on one browser/device. This is NOT secure authentication, not multi-user online storage, and not suitable for real sensitive disclosures. A visitor with access to browser storage/devtools can tamper with local roles/data. The administrator password is not embedded in the source, and the password previously shared in chat is not used.

For a real public launch, deploy a backend with server-side password hashing (Argon2id/bcrypt), secure sessions, database access controls, rate limiting, email/password reset, private message APIs, admin role granted server-side only, HTTPS, backups, and GDPR-compliant privacy/retention/deletion handling. Configure the initial admin account securely on the server as arealpips. Never use the password previously pasted into chat; set a new unique password during deployment.
