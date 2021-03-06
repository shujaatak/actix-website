# Actix Website

The work in progress website for the actix project based on tokio's website.

## Getting Started

Building the website depends on [Hugo](http://gohugo.io). So, first make sure
that you have it installed. If on OS X and using Homebrew, run the following:

```sh
brew update && brew install hugo
```

Then, get the website running locally:

```sh
git clone https://github.com/actix/actix-website.git
cd actix-website
hugo server
```

Then visit [http://localhost:1313](http://localhost:1313).

## Updating diagrams

Diagrams are located under [/static/css/img/diagrams/](https://github.com/actix/actix-website/tree/master/static/img/diagrams) and built with [Mermaid CLI](https://github.com/mermaidjs/mermaid.cli).

For instance to edit `connection_overview` diagram:
```sh
cd static/css/img/diagrams
vi connection_overview.mmd
# Compile diagrams:
mmdc -i connection_overview.mmd -o connection_overview.svg
```

# License

Pretty murky.  Right now a massive clone of the tokio website.  Will get this
figured out as we go along.
