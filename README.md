# The Littoral Line

A newsletter about design, human attention and the web.

So I own my writing, I create a Jekyll web page published to thelittoralline.callumflack.design which is then imported into Mailchimp via URL.

If you need to run a draft or a future post locally, run it with the `--draft` or `--future` flags (although I have set `future: true` in config.yml).

To set the environment variable for production, build the site with:

`JEKYLL_ENV=production jekyll build --future`

Then run `now && now alias` from the `_site` dir.
