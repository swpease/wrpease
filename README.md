# NOTES for 2026
I had no memory of how this worked. `bundle exec jekyll serve` did not work, and it took quite a while to figure out what was up.

I installed [rbenv](https://github.com/rbenv/rbenv) per the suggestion [here](https://stackoverflow.com/questions/51126403/you-dont-have-write-permissions-for-the-library-ruby-gems-2-3-0-directory-ma) of fixing the Ruby issue I was having.

I then had to delete my Gemfile.lock file, per the suggestion [here](https://stackoverflow.com/questions/68411134/how-do-i-resolve-this-bundle-update-error-when-trying-to-use-jekyll).
I also updated the `bundle` version listed in the lock file prior (running `bundle update --bundler`), though that might have automatically happened anyway with this step.

I then ran into an issue with jekyll-menus. I found a solution [here](https://github.com/forestryio/jekyll-menus/issues/29). My current local project did the manual fix route, as the git-sourced specifier in the config file failed. My current worry is how this will work out when I try to deploy it, because presumably my webhost will use the config file to install stuff, so it won't have my modified file.


# NOTES
Per [Jekyll](https://jekyllrb.com/docs/variables/):
>All the variables set via the command line and your _config.yml are available through the site variable. For example, if you have foo: bar in your configuration file, then it will be accessible in Liquid as site.foo. Jekyll does not parse changes to _config.yml in watch mode, you must restart Jekyll to see changes to variables.

Ergo, if you're making changes to the `SITE Menus` in Forestry, you'll need to restart the preview server to see your changes. To read up on the `SITE Menus` feature, see [Jekyll Menus](https://github.com/forestryio/jekyll-menus).

# Forestry Jekyll demo

A Jekyll demo site for [Forestry CMS](https://forestry.io).

## Import to Forestry

This project has been pre-configured to work with Forestry, just import your repository ✨.  
Any changes you make will be commited back to the repo, and deployed if you're using Netlify.

<p><a href="https://app.forestry.io/quick-start?repo=forestryio-templates/belkirk-jekyll-demo&engine=jekyll">
    <img alt="Import this project into Forestry" src="https://assets.forestry.io/import-to-forestryK.svg" />
</a></p>

Forestry empowers editors with a usable interface to edit Markdown, YAML and JSON files:

![](https://res.cloudinary.com/forestry-demo/image/fetch/c_limit,dpr_auto,f_auto,q_80,w_1205/https://forestry.io/uploads/2018/12/draft-post-editor.png)

## Documentation

- [Forestry docs](https://forestry.io/docs/welcome/)
- [Jekyll Developer Guide](https://forestry.io/docs/guides/developing-with-jekyll/)
- [Jekyll docs](https://jekyllrb.com)

## Deployment

The easiest way to deploy this Jekyll v4 demo is to build and deploy through https://netlify.com, just click the button below and follow the instructions.

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/forestryio-templates/belkirk-jekyll-demo)

## Running locally

### Requirements

- Ruby > 2.4
- Bundler > 2.0
- Jekyll > 4.0

Once you've cloned the repository:

```
# Install project dependencies
bundle install

# Run a local server to preview your work 
bundle exec jekyll serve
```


