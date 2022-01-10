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


