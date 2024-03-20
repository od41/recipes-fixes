84

There does not seem to be any answer which addresses the very common beginner problem of failing to install the required library in the first place.

On Debianish platforms, if libfoo is missing, you can frequently install it with something like

apt-get install libfoo-dev
The -dev version of the package is required for development work, even trivial development work such as compiling source code to link to the library.

The package name will sometimes require some decorations (libfoo0-dev? foo-dev without the lib prefix? etc), or you can simply use your distro's package search to find out precisely which packages provide a particular file.

(If there is more than one, you will need to find out what their differences are. Picking the coolest or the most popular is a common shortcut, but not an acceptable procedure for any serious development work.)

For other architectures (most notably RPM) similar procedures apply, though the details will be different.
