# Worlds Elsewhere Theater Company Website

This is a site made to promote the [Worlds Elsewhere Theater Company](https://worlds-elsewhere.com). Unless specified, all content within is wholely owned by the company and its Executive Director, Kyle Kallgren, :copyright: 2020.

It was hastily put together by [Adrianne Greenberg-Sud](https://pigsflew.com), and utilizes the Jeckyll theme engine.

The current theme of the website is `vernon-zero`, originally created for Worlds Elsewhere by [Alex Vernon](https://github.com/Alexandra-Vernon/).

## Adding content

To add or change content on the worlds-elsewhere website, you can edit one of the markdown files found within.

Of note, the following files:

1. [index.md](https://github.com/Worlds-Elsewhere/worlds-elsewhere.com/blob/master/index.md): Contains the entire content for the page which maps to `index.html`, and is rendered directly on [the home page](https://worlds-elsewhere.com)
2. [`plays` directory](https://github.com/Worlds-Elsewhere/worlds-elsewhere.com/blob/master/plays/): Contains the playbill content for all our productions past and present, such as [plays/midsummer/index.md](https://github.com/Worlds-Elsewhere/worlds-elsewhere.com/blob/master/plays/midsummer/index.md)
3. [`home` directory](https://github.com/Worlds-Elsewhere/worlds-elsewhere.com/blob/master/home/): Contains all the content to be rendered into the header navigation, such as [home/contact/index.md](https://github.com/Worlds-Elsewhere/worlds-elsewhere.com/blob/master/home/contact/index.md).

## Running the site locally

To run this site locally, you can install [Jekyll for Github-Pages](https://jekyllrb.com) through Ruby and Bundler.

```
gem install jekyll bundler
bundle install
```

After that you can execute jekyll through bundler to build and serve the site locally for testing.

```
bundle exec jekyll serve
```

At this point you can visit your now-running server on [localhost:4000](http://localhost:4000).

To get Ruby and Gem on your machine,
