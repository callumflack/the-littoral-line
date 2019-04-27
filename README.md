# The Littoral Line

A newsletter about design, human attention and the web.

So I own my writing, I create a website of posts published to [thelittoralline.callumflack.design](https://thelittoralline.callumflack.design) which is then imported into Mailchimp via URL.

Because the best writing tool for the web is markdown, I'm using I'm using Jekyll. There are other tools (MDX!) but none allow me to keep the simplicity of an old school CSS file. And I have some old projects on Jekyll, so I need to keep my hand in it.

### Localhost

If you need to run a draft or a future post locally, run it with the `--draft` or `--future` flags (although I have set `future: true` in config.yml).

I use `JEKYLL_ENV=production` in the layout to turn on and off easy settings when using localhost. This is set in the now. `env` object.

### Deployment for Now v2

Run `now` from the project root. This uses the `build/sh` file.

More info: https://github.com/zeit/now-examples/blob/master/jekyll/build.sh

If there's a problem, start by updating the rub gems with `bundle update`…

This means that I can write _directly here in Github_ and Now will publish the commit, from which I can use the resulting post URL for a newsletter edition.

Note that you can always run a production build with Jekyll: `JEKYLL_ENV=production jekyll build --future`.

### Queue it in Mailchimp

Import the post as HTML via URL to create a campaign in Mailchimp, [like so](https://mailchimp.com/help/import-html-from-url-to-create-a-campaign/).
