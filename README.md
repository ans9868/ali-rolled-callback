# ali-rolled-callback

OAuth callback page for the Rolled research tool's AliExpress Open Platform app.

Callback URL to register: `https://ans9868.github.io/ali-rolled-callback/`

The page is static: it reads the one-time `code` AliExpress adds to the address, shows it with a Copy
button, and removes it from the address bar. It makes no network requests (a Content-Security-Policy
blocks them) and sends no referrer. The code is exchanged for an access token by a local script that
holds the App Key and Secret — nothing secret lives in this repo.
