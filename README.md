## Jenkins Style

This is forked from Isotope11 Style so original for details

1. Install the [Jenkins Simple Theme Plugin][simple_theme].
2. Set your custom css to `http://isotope11.github.com/jenkins-isotope-style/jenkins-isotope-style.css`
3. Fork our project, make your own changes (pull requests welcome!), add your
organization's logo and colors.
4. Run the ruby script provided to publish your stylesheet to github-pages for
hosting, so you can just point your Jenkins custom CSS to your own fork.
5. Tweak to your heart's content.

### Development
To run sass and compile the stylesheet as you make changes, run this:

    sass --watch jenkins-isotope-style.scss:jenkins-isotope-style.css

To push the styles to github pages, which is where jenkins looks for them, make
sure you've committed and pushed everything to master.  Then run:

    ruby copy_styles.rb

That'll do all the git magic.  Now when you ctrl+refresh jenkins, your changes
are there.

[isotope]: http://www.isotope11.com
[jenkins]: http://www.jenkins-ci.org
[sass]: http://sass-lang.com/
[simple_theme]: https://wiki.jenkins-ci.org/display/JENKINS/Simple+Theme+Plugin
