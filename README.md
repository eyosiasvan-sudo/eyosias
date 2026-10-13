# eyosias

This static site lives in `index.html`, with its styles and scripts included inline.

## Netlify deployment

`netlify.toml` copies `index.html` into `public/` during deployment and publishes
only that generated directory. No package installation or Makefile is required.
The generated `public/` directory is ignored by Git.

The functions directory is explicitly set to `netlify/functions/`, overriding
the obsolete `my_functions` site setting. A placeholder keeps this directory in
Git; the site does not currently use serverless functions.
