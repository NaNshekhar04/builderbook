## Add transactional emails to a JavaScript web app (React, Express)
This folder contains the ending code for our tutorial on how to add transactional emails to a JavaScript web app (React, Express). In the tutorial, you integrate an app with AWS SES to send a welcome email to a guest user.


## Run locally
- Clone the builderbook repo to your local machine: `git clone git@github.com:builderbook/builderbook.git`
- Inside the `tutorials/2-start` folder, run `yarn` to add packages
- Start the app with `yarn dev`
- _Important note_: You will need to add your own `Amazon_accessKeyId` and `Amazon_secretAccessKey` values from AWS SES in `server/aws.js`


## Project structure

```
.
├── components                  # React components
│   ├── Header.js               # Header component
│   ├── SharedStyles.js         # List of _reusable_ styles
├── lib                         # Code available on both client and server
│   ├── api                     # Client-side API methods
│   │   ├── public.js           # Public user methods
│   ├── context.js              # Context for Material-UI integration
│   ├── withLayout.js           # HOC for SSR with Material-UI and more
├── pages                       # Pages
│   ├── _document.js            # Main Document for Next.js pages
│   ├── login.js                # Login page
│   ├── index.js                # Dashboard page
│   ├── send-email.js           # Send email page
├── server                      # Server code
│   ├── app.js                  # Custom Express/Next server
│   ├── app.js                  # AWS SES API
├── .babelrc                    # Config for Babel
├── .eslintrc.js                # Config for Eslint
├── .gitignore                  # List of ignored files and directories
├── package.json                # List of packages and scripts
├── yarn.lock                   # Exact versions of packages. Generated by yarn.

```