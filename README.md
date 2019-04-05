# The Littoral Line

A newsletter about design, human attention and the web.

So I own my writing, I create a Jekyll web page published to thelittoralline.callumflack.design which is then imported into Mailchimp via URL.

### Localhost

If you need to run a draft or a future post locally, run it with the `--draft` or `--future` flags (although I have set `future: true` in config.yml).

### Deployment for Now v2

Run `now` from the project root.

I use `JEKYLL_ENV=production` in the layout to turn on and off easy settings when using localhost. This is set in the now. `env` object.

If there's a problem, start by updating the rub gems with `bundle update`…

See: https://github.com/zeit/now-examples/blob/master/jekyll/build.sh

Ps. You build the site for production with Jekyll using: `JEKYLL_ENV=production jekyll build --future`.
