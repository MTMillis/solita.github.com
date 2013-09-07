# /dev/solita/greetings

Here are some developer-oriented thoughts from [Solita Oy](http://www.solita.fi/). Our stories have not yet been told. More will come. Stay tuned at <http://dev.solita.fi>.

## Writing

We use a combination of Jekyll and Github Pages to run the site.

If you want to write a post, here's how:

1. Fork this project to yourself (upper right corner)
  - You need a Github account to do this
2. Clone your own fork to your computer (git clone)
3. Add your author info to `_config.yml`
4. Write a new post under the `_posts` folder using Markdown, look at other posts for example of what to write there
5. If you have Ruby and Jekyll, preview your post locally (instructions below)
6. Create a pull request at https://github.com/solita/solita.github.com/pull/new/master
  - Choose your fork on the right
  - Write some info about the post
7. Wait for comments and publish!


## Previewing posts

You need Ruby and Jekyll if you want to preview your posts locally on the blog. If you're fine with just previewing the Markdown, you can use a Markdown preview script, like [this one for Sublime Text](https://github.com/revolunet/sublimetext-markdown-preview).

### Installing Ruby

For Windows, download & install the latest Ruby 1.9.x and Development Kit from http://rubyinstaller.org/downloads/.  
**Note:** Make sure to tick the checkbox "Add Ruby to PATH" (or something)

For OSX(/Linux), use the instructions below. If you have installed Xcode, you might have ruby (1.9.2 or something like that) already. No guarantinees about this working with that so use RVM


1. \curl -L https://get.rvm.io | bash
2. rvm install 1.9.3
3. fork this repo
4. go to dir
5. rvm use 1.9.3
6. verify that 1.9.3 used by ruby -v
7. gem install bundler
8. bundle install
9. done
10. Type in: `jekyll serve --watch`
11. Open browser to: http://localhost:4000/ (or some other address?)

### Installing Jekyll (and Foreman)

1. Open a command prompt or terminal
2. Make sure ruby is active by typing in `ruby -v` (rvm.io ftw)
3. To run Jekyll, go to your working copy of solita.github.com
4. Run bundle install for depencies
5. Make sure the installation succeeds
6. Type in: `jekyll serve --watch`
7. Open browser to: http://localhost:4000/ (or some other address?)


## Development

For development, you need Ruby and Jekyll. If you want to tweak the CSS, you need Compass. Also, if you want to make stuff easier, install foreman.

1. Install Ruby (above)
2. To install Jekyll, Compass and foreman, type into a command prompt or terminal:  
`gem install jekyll compass foreman`
3. Make sure the install succeeds
4. Go to your cloned copy of solita.github.com
5. Type in: `foreman start`
6. Jekyll and Compass should start!

## Technology stack

/dev/solita is built using all the hippiest hip technologies available:

    git, Github Pages, Ruby, Jekyll, Markdown, Sass, Compass, foreman, jQuery, Gravatar, disqus, Google Analytics, AddThis
