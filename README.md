# ish iPhone server

1. Install [ish](https://apps.apple.com/us/app/ish-shell/id1436902243).
2. Open the app.
3. Create the web folder.
   ```
   mkdir -p /var/www
   ```
4. Install the OS dependencies.
   ```
   apk add nodejs npm git ssh
   ```
5. Create an SSH key.
   ```
   ssh-keygen -t ed25519
   ```
6. Clone the repo.
   ```
   cd /var/www
   git clone git@github.com/selfagency/ish-iphone-server.git .
   ```
7. Install the Node dependencies.
   ```
   npm i
   ```
8. Run the app.
   ```
   npm run start
   ```

This is an experimental proof-of-concept and *not secure*. Do not use in production.

Made entirely on an iPhone using ish, [vim](https://www.vim.org/), [srv.us](https://github.com/pcarrier/srv.us), and [asdf](https://github.com/alsotang/asdf).

