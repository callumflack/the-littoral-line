# The Littoral Line

A newsletter about design, human attention and the web.

So I own my writing, I create a website of posts published to [thelittoralline.callumflack.design](https://thelittoralline.callumflack.design) which is then imported into Mailchimp via URL.

Because the best writing tool for the web is markdown, I'm using Jekyll to build the site. There are other tools (MDX!) but none allow me to keep the simplicity of an old school CSS file. And I have some old projects on Jekyll, so I need to keep my hand in it.

## The newsletter writing process

### Localhost

If you need to run a draft or a future post locally, run it with the `--draft` or `--future` flags (although I have set `future: true` in config.yml).

I use `JEKYLL_ENV=production` in the layout to easily turn on and off settings when using localhost. This is set in the `.env` object within `now.json`.

### Deployment for Now v2

A `now` webhook is set-up for this repo. You can also run `now` from the project root. This process is configured in `now.json` and uses the `build.sh` file in the project root.

Read more about deploying Jekyll with Now [here](https://github.com/zeit/now-examples/blob/master/jekyll/build.sh).

If there's a problem, start by updating the rub gems with `bundle update`…

By deplying with Now-Github webhooks, I can write _directly here in Github_ and Now will publish the commit, from which I can use the resulting post URL for a newsletter edition.

Note that you can always run a production build with Jekyll: `JEKYLL_ENV=production jekyll build --future`.

### Queue it in Mailchimp

Import the post as HTML via URL to create a campaign in Mailchimp, [like so](https://mailchimp.com/help/import-html-from-url-to-create-a-campaign/).

## Todo

- [ ] Add an RSS feed so I can automate the Mailchimp campaigns

- [ ] Just keep writing FFX
