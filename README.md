
# e2u ~ E2 Userland Library

e2u is a standardized and tested toolchain for E2 script development.

This library has two primary goals:

* Padding over some of E2's limitations for day-to-day development.
* Above all, having fun experimenting and pushing E2 to its limit,
  as a learning exercise.

## Installation:

Clone this repository to your Expression2 data folder, with TortoiseGit
or any command-line interface that you have available in your Windows
installation. The following example uses cygwin + git.

```bash
$ cd <garrysmod directory>/data/Expression2
$ git clone https://github.com/filp/e2u.git
```

The library will be available, from your E2 editor, under "e2u/lib".

*Note:* You can also download this repository's zip file and place
it in your data/Expression2 folder, but you will have to re-download
it every time you want to update it.

## Using the library:

There are two ways to use this library. Since every library component
is stand-alone, you can include just the parts you need:


```C
#include "e2u/lib/assert"
#include "e2u/lib/object"
```

Or you can include the whole library:

```C
#include "e2u/lib/e2u"
```

Including the whole library also includes some meta-programming tools
to introspect the `e2u` library at runtime, which you may find useful.


## Contributing:

*Note:* This section is not currently complete

You may contribute your own features, fixes or new library components
by forking this library and sending a pull request. Please follow
these guidelines before contributing:

* Before adding a new component, be sure it's actually useful in
  a variety of situations.
* Follow the coding style used through-out the rest of the library
* If you add a new component or make any significant changes, make
  sure that, if possible, it's covered by a test in `tests/`.
