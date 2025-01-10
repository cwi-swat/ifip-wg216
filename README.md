# Sources of Webpage of IFIP TC2 Working group 2.16 on Language Design

This is deployed via GitHub Pages to appear on:

https://languagedesign.org/

This site is statically generated using Jekyll.

## Testing Locally

1. Install Jekyll ([Jekyll installation guide](https://jekyllrb.com/docs/))

2. Install the project `gem` dependencies:

  ```bash
  bundle install
  ```

3. Open the development server:

  ```bash
  bundle exec jekyll serve
  bundle exec jekyll serve --livereload
  ```

  The `--livereload` optional flag will automatically refresh the page when the source files change.

4. To check that `build` does not fail:

  ```bash
  bundle exec jekyll build
  ```

## Deployment

Simply push.
