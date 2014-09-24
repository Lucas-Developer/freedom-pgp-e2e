uproxy-end-to-end
=================

Wrapping up end-to-end code and provide in freedom custom API.


#### Build
- Grab all node modules necessary for the build (npm install)

- Ensure you have dependencies for building end-to-end (unzip, svn,
  Python 2.X, Java >= 1.7)

- Perform normal Grunt build (grunt)

Note - the grunt build will be pulling from various repositories to
build end-to-end. You'll see quite a few things flying by, and may
need to accept certificates for *.googlecode.com. It may also have
warnings on repeated runs as paths/files will already exist - these
shouldn't be an issue, but check tests to be sure.

#### Test

When running grunt, karma PhantomJS tests are automatically run and
should be reported at the end. If you want to run the same tests on
Firefox and Chrome, use "grunt test" instead.

Additionall, a sample chrome app is prepared to show the usage of
end-to-end api. After build, just load "build/samples/chrome-app" to
chrome. You will need to enable developer mode and click "load
unpacked extension", and you should see the text "pgp encryption test
succeeded" at the bottom of the window that pops up once you launch it.


