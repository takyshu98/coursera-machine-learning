#### Octaveのインストール（Mac）

Octave wiki
[https://wiki.octave.org/Octave_for_macOS](https://wiki.octave.org/Octave_for_macOS)

> If running Mountain Lion (Mac OS 10.8) or later, install XQuartz.

引用よりXQuartz（X Window環境）を先にインストールする

```
takyshu98s-mbp{takyshu98}% brew cask install xquartz
==> Satisfying dependencies
==> Downloading https://dl.bintray.com/xquartz/downloads/XQuartz-2.7.11.dmg
######################################################################## 100.0%
==> Verifying SHA-256 checksum for Cask 'xquartz'.
==> Installing Cask xquartz
==> Running installer for xquartz; your password may be necessary.
==> Package installers may write to any location; options such as --appdir are ignored.
Password:

installer: Package name is XQuartz 2.7.11
installer: Installing at base path /
installer: The install was successful.
🍺  xquartz was successfully installed!
```

Homebrew/homebrew-science
[https://github.com/Homebrew/homebrew-science/issues/6617](https://github.com/Homebrew/homebrew-science/issues/6617)

> The formulae in Homebrew/science have been archived at https://github.com/brewsci/homebrew-science. I've created a new tap for bioinformatics formulae at https://github.com/brewsci/homebrew-bio.
🍺 brew tap brewsci/bio
🍺 brew tap brewsci/science
💀 brew untap homebrew/science

引用よりbrewsci/scienceを指定する.

```
takyshu98s-mbp{takyshu98}% brew tap homebrew/science
Error: homebrew/science was deprecated. This tap is now empty as all its formulae were migrated.
[~/tmp/coursera-machine-learning/week02/enviroment_setup_instructions]
```
```
takyshu98s-mbp{takyshu98}% brew tap brewsci/science
==> Tapping brewsci/science
Cloning into '/usr/local/Homebrew/Library/Taps/brewsci/homebrew-science'...
remote: Enumerating objects: 442, done.
remote: Counting objects: 100% (442/442), done.
remote: Compressing objects: 100% (439/439), done.
remote: Total 442 (delta 1), reused 142 (delta 1), pack-reused 0
Receiving objects: 100% (442/442), 405.50 KiB | 584.00 KiB/s, done.
Resolving deltas: 100% (1/1), done.
Tapped 423 formulae (462 files, 1.3MB).
```
```
takyshu98s-mbp{takyshu98}% brew install octave
==> Installing dependencies for octave: isl, mpfr, libmpc, gcc, veclibfort, arpack, jpeg, libtiff, ghostscript, epstool, fftw, libpng, jasper, netpbm, fig2dev, fltk, freetype, fontconfig, gl2ps, glpk, webp, gd, glib, pixman, cairo, fribidi, graphite2, icu4c, harfbuzz, pango, gnuplot, libtool, graphicsmagick, szip, hdf5, libogg, flac, libvorbis, libsndfile, portaudio, little-cms2, openjpeg, imagemagick, plotutils, pstoedit, qhull, qrupdate, metis, suite-sparse, openssl, open-mpi, sundials and texinfo
==> Installing octave dependency: isl
==> Downloading https://homebrew.bintray.com/bottles/isl-0.20.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring isl-0.20.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/isl/0.20: 71 files, 3.9MB
==> Installing octave dependency: mpfr
==> Downloading https://homebrew.bintray.com/bottles/mpfr-4.0.1.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring mpfr-4.0.1.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/mpfr/4.0.1: 28 files, 4.6MB
==> Installing octave dependency: libmpc
==> Downloading https://homebrew.bintray.com/bottles/libmpc-1.1.0.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring libmpc-1.1.0.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/libmpc/1.1.0: 12 files, 354KB
==> Installing octave dependency: gcc
Warning: Building gcc from source:
  The bottle needs the Xcode CLT to be installed.
==> Downloading https://ftp.gnu.org/gnu/gcc/gcc-8.2.0/gcc-8.2.0.tar.xz
######################################################################## 100.0%
==> Patching
patching file gcc/graphite.h
==> ../configure --build=x86_64-apple-darwin18.0.0 --prefix=/usr/local/Cellar/gcc/8.2.0 --libdir=/usr/local/Cellar/gcc/8.2.0/lib/gcc/8 --disable-nls --enable-ch
==> make
==> make install
🍺  /usr/local/Cellar/gcc/8.2.0: 1,413 files, 287.2MB, built in 44 minutes 10 seconds
==> Installing octave dependency: veclibfort
==> Downloading https://homebrew.bintray.com/bottles/veclibfort-0.4.2_6.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring veclibfort-0.4.2_6.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/veclibfort/0.4.2_6: 8 files, 85.6KB
==> Installing octave dependency: arpack
==> Downloading https://homebrew.bintray.com/bottles/arpack-3.6.3.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring arpack-3.6.3.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/arpack/3.6.3: 22 files, 1.4MB
==> Installing octave dependency: jpeg
==> Downloading https://homebrew.bintray.com/bottles/jpeg-9c.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring jpeg-9c.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/jpeg/9c: 21 files, 733.4KB
==> Installing octave dependency: libtiff
==> Downloading https://homebrew.bintray.com/bottles/libtiff-4.0.10.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring libtiff-4.0.10.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/libtiff/4.0.10: 246 files, 3.5MB
==> Installing octave dependency: ghostscript
==> Downloading https://homebrew.bintray.com/bottles/ghostscript-9.26.mojave.bottle.tar.gz
#######################################                                   55.0%
curl: (56) LibreSSL SSL_read: SSL_ERROR_SYSCALL, errno 54
Error: Failed to download resource "ghostscript"
Download failed: https://homebrew.bintray.com/bottles/ghostscript-9.26.mojave.bottle.tar.gz
Warning: Bottle installation failed: building from source.
==> Downloading https://github.com/ArtifexSoftware/ghostpdl-downloads/releases/download/gs926/ghostpdl-9.26.tar.xz
==> Downloading from https://github-production-release-asset-2e65be.s3.amazonaws.com/50461376/c9110c80-ecdf-11e8-9ab0-9bb65f6af420?X-Amz-Algorithm=AWS4-HMAC-SHA
######################################################################## 100.0%
==> Patching
patching file base/unix-dll.mak
==> ./configure --prefix=/usr/local/Cellar/ghostscript/9.26 --disable-cups --disable-compile-inits --disable-gtk --disable-fontconfig --without-libidn --with-sy
==> make install
==> make install-so
==> Downloading https://downloads.sourceforge.net/project/gs-fonts/gs-fonts/8.11%20%28base%2035%2C%20GPL%29/ghostscript-fonts-std-8.11.tar.gz
==> Downloading from https://jaist.dl.sourceforge.net/project/gs-fonts/gs-fonts/8.11%20%28base%2035%2C%20GPL%29/ghostscript-fonts-std-8.11.tar.gz
######################################################################## 100.0%
🍺  /usr/local/Cellar/ghostscript/9.26: 668 files, 81MB, built in 5 minutes 46 seconds
==> Installing octave dependency: epstool
==> Downloading https://homebrew.bintray.com/bottles/epstool-3.08.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring epstool-3.08.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/epstool/3.08: 8 files, 275.2KB
==> Installing octave dependency: fftw
==> Downloading https://homebrew.bintray.com/bottles/fftw-3.3.8.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring fftw-3.3.8.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/fftw/3.3.8: 52 files, 10.9MB
==> Installing octave dependency: libpng
==> Downloading https://homebrew.bintray.com/bottles/libpng-1.6.35.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring libpng-1.6.35.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/libpng/1.6.35: 26 files, 1.2MB
==> Installing octave dependency: jasper
==> Downloading https://homebrew.bintray.com/bottles/jasper-2.0.14.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring jasper-2.0.14.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/jasper/2.0.14: 39 files, 989.2KB
==> Installing octave dependency: netpbm
==> Downloading https://homebrew.bintray.com/bottles/netpbm-10.73.22.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring netpbm-10.73.22.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/netpbm/10.73.22: 741 files, 6.6MB
==> Installing octave dependency: fig2dev
==> Downloading https://homebrew.bintray.com/bottles/fig2dev-3.2.7a.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring fig2dev-3.2.7a.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/fig2dev/3.2.7a: 36 files, 774.0KB
==> Installing octave dependency: fltk
==> Downloading https://homebrew.bintray.com/bottles/fltk-1.3.4-2.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring fltk-1.3.4-2.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/fltk/1.3.4-2: 328 files, 5.1MB
==> Installing octave dependency: freetype
==> Downloading https://homebrew.bintray.com/bottles/freetype-2.9.1.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring freetype-2.9.1.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/freetype/2.9.1: 60 files, 2.6MB
==> Installing octave dependency: fontconfig
==> Downloading https://homebrew.bintray.com/bottles/fontconfig-2.13.1.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring fontconfig-2.13.1.mojave.bottle.tar.gz
==> Regenerating font cache, this may take a while
==> /usr/local/Cellar/fontconfig/2.13.1/bin/fc-cache -frv
🍺  /usr/local/Cellar/fontconfig/2.13.1: 531 files, 3.3MB
==> Installing octave dependency: gl2ps
==> Downloading https://homebrew.bintray.com/bottles/gl2ps-1.4.0.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring gl2ps-1.4.0.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/gl2ps/1.4.0: 13 files, 239.3KB
==> Installing octave dependency: glpk
==> Downloading https://homebrew.bintray.com/bottles/glpk-4.65.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring glpk-4.65.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/glpk/4.65: 12 files, 2.4MB
==> Installing octave dependency: webp
==> Downloading https://homebrew.bintray.com/bottles/webp-1.0.1.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring webp-1.0.1.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/webp/1.0.1: 39 files, 2.1MB
==> Installing octave dependency: gd
==> Downloading https://homebrew.bintray.com/bottles/gd-2.2.5.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring gd-2.2.5.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/gd/2.2.5: 35 files, 1.1MB
==> Installing octave dependency: glib
==> Downloading https://homebrew.bintray.com/bottles/glib-2.58.1.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring glib-2.58.1.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/glib/2.58.1: 435 files, 18.4MB
==> Installing octave dependency: pixman
==> Downloading https://homebrew.bintray.com/bottles/pixman-0.34.0_1.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring pixman-0.34.0_1.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/pixman/0.34.0_1: 13 files, 1.3MB
==> Installing octave dependency: cairo
==> Downloading https://homebrew.bintray.com/bottles/cairo-1.16.0.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring cairo-1.16.0.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/cairo/1.16.0: 117 files, 5.5MB
==> Installing octave dependency: fribidi
==> Downloading https://homebrew.bintray.com/bottles/fribidi-1.0.5.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring fribidi-1.0.5.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/fribidi/1.0.5: 66 files, 581.3KB
==> Installing octave dependency: graphite2
==> Downloading https://homebrew.bintray.com/bottles/graphite2-1.3.12.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring graphite2-1.3.12.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/graphite2/1.3.12: 18 files, 231.9KB
==> Installing octave dependency: icu4c
==> Downloading https://homebrew.bintray.com/bottles/icu4c-63.1.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring icu4c-63.1.mojave.bottle.tar.gz
==> Caveats
icu4c is keg-only, which means it was not symlinked into /usr/local,
because macOS provides libicucore.dylib (but nothing else).

If you need to have icu4c first in your PATH run:
  echo 'export PATH="/usr/local/opt/icu4c/bin:$PATH"' >> ~/.zshrc
  echo 'export PATH="/usr/local/opt/icu4c/sbin:$PATH"' >> ~/.zshrc

For compilers to find icu4c you may need to set:
  export LDFLAGS="-L/usr/local/opt/icu4c/lib"
  export CPPFLAGS="-I/usr/local/opt/icu4c/include"

For pkg-config to find icu4c you may need to set:
  export PKG_CONFIG_PATH="/usr/local/opt/icu4c/lib/pkgconfig"

==> Summary
🍺  /usr/local/Cellar/icu4c/63.1: 254 files, 68.4MB
==> Installing octave dependency: harfbuzz
==> Downloading https://homebrew.bintray.com/bottles/harfbuzz-2.2.0.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring harfbuzz-2.2.0.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/harfbuzz/2.2.0: 176 files, 7.9MB
==> Installing octave dependency: pango
==> Downloading https://homebrew.bintray.com/bottles/pango-1.42.4.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring pango-1.42.4.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/pango/1.42.4: 106 files, 4.3MB
==> Installing octave dependency: gnuplot
==> Downloading https://homebrew.bintray.com/bottles/gnuplot-5.2.5.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring gnuplot-5.2.5.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/gnuplot/5.2.5: 45 files, 2.6MB
==> Installing octave dependency: libtool
==> Downloading https://homebrew.bintray.com/bottles/libtool-2.4.6_1.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring libtool-2.4.6_1.mojave.bottle.tar.gz
==> Caveats
In order to prevent conflicts with Apple's own libtool we have prepended a "g"
so, you have instead: glibtool and glibtoolize.
==> Summary
🍺  /usr/local/Cellar/libtool/2.4.6_1: 71 files, 3.7MB
==> Installing octave dependency: graphicsmagick
==> Downloading https://homebrew.bintray.com/bottles/graphicsmagick-1.3.31.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring graphicsmagick-1.3.31.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/graphicsmagick/1.3.31: 484 files, 12.7MB
==> Installing octave dependency: szip
==> Downloading https://homebrew.bintray.com/bottles/szip-2.1.1_1.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring szip-2.1.1_1.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/szip/2.1.1_1: 11 files, 109.4KB
==> Installing octave dependency: hdf5
==> Downloading https://homebrew.bintray.com/bottles/hdf5-1.10.4.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring hdf5-1.10.4.mojave.bottle.tar.gz
Warning: hdf5 dependency gcc was built with a different C++ standard
library (libstdc++ from clang). This may cause problems at runtime.
🍺  /usr/local/Cellar/hdf5/1.10.4: 262 files, 14.8MB
==> Installing octave dependency: libogg
==> Downloading https://homebrew.bintray.com/bottles/libogg-1.3.3.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring libogg-1.3.3.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/libogg/1.3.3: 97 files, 459.9KB
==> Installing octave dependency: flac
==> Downloading https://homebrew.bintray.com/bottles/flac-1.3.2_1.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring flac-1.3.2_1.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/flac/1.3.2_1: 53 files, 1.8MB
==> Installing octave dependency: libvorbis
==> Downloading https://homebrew.bintray.com/bottles/libvorbis-1.3.6.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring libvorbis-1.3.6.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/libvorbis/1.3.6: 157 files, 2.3MB
==> Installing octave dependency: libsndfile
==> Downloading https://homebrew.bintray.com/bottles/libsndfile-1.0.28.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring libsndfile-1.0.28.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/libsndfile/1.0.28: 48 files, 1.8MB
==> Installing octave dependency: portaudio
==> Downloading https://homebrew.bintray.com/bottles/portaudio-19.6.0.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring portaudio-19.6.0.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/portaudio/19.6.0: 33 files, 452.4KB
==> Installing octave dependency: little-cms2
==> Downloading https://homebrew.bintray.com/bottles/little-cms2-2.9.mojave.bottle.1.tar.gz
######################################################################## 100.0%
==> Pouring little-cms2-2.9.mojave.bottle.1.tar.gz
🍺  /usr/local/Cellar/little-cms2/2.9: 18 files, 1MB
==> Installing octave dependency: openjpeg
==> Downloading https://homebrew.bintray.com/bottles/openjpeg-2.3.0.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring openjpeg-2.3.0.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/openjpeg/2.3.0: 515 files, 12.9MB
==> Installing octave dependency: imagemagick
==> Downloading https://homebrew.bintray.com/bottles/imagemagick-7.0.8-16.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring imagemagick-7.0.8-16.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/imagemagick/7.0.8-16: 1,519 files, 23.3MB
==> Installing octave dependency: plotutils
==> Downloading https://homebrew.bintray.com/bottles/plotutils-2.6_1.mojave.bottle.1.tar.gz
######################################################################## 100.0%
==> Pouring plotutils-2.6_1.mojave.bottle.1.tar.gz
🍺  /usr/local/Cellar/plotutils/2.6_1: 74 files, 6.5MB
==> Installing octave dependency: pstoedit
==> Downloading https://homebrew.bintray.com/bottles/pstoedit-3.73.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring pstoedit-3.73.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/pstoedit/3.73: 41 files, 2.2MB
==> Installing octave dependency: qhull
==> Downloading https://homebrew.bintray.com/bottles/qhull-2015.2.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring qhull-2015.2.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/qhull/2015.2: 132 files, 5MB
==> Installing octave dependency: qrupdate
==> Downloading https://homebrew.bintray.com/bottles/qrupdate-1.1.2_8.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring qrupdate-1.1.2_8.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/qrupdate/1.1.2_8: 11 files, 450.2KB
==> Installing octave dependency: metis
==> Downloading https://homebrew.bintray.com/bottles/metis-5.1.0.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring metis-5.1.0.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/metis/5.1.0: 18 files, 11.8MB
==> Installing octave dependency: suite-sparse
==> Downloading https://homebrew.bintray.com/bottles/suite-sparse-5.3.0.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring suite-sparse-5.3.0.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/suite-sparse/5.3.0: 157 files, 16.3MB
==> Installing octave dependency: openssl
==> Downloading https://homebrew.bintray.com/bottles/openssl-1.0.2q.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring openssl-1.0.2q.mojave.bottle.tar.gz
==> Caveats
A CA file has been bootstrapped using certificates from the SystemRoots
keychain. To add additional certificates (e.g. the certificates added in
the System keychain), place .pem files in
  /usr/local/etc/openssl/certs

and run
  /usr/local/opt/openssl/bin/c_rehash

openssl is keg-only, which means it was not symlinked into /usr/local,
because Apple has deprecated use of OpenSSL in favor of its own TLS and crypto libraries.

If you need to have openssl first in your PATH run:
  echo 'export PATH="/usr/local/opt/openssl/bin:$PATH"' >> ~/.zshrc

For compilers to find openssl you may need to set:
  export LDFLAGS="-L/usr/local/opt/openssl/lib"
  export CPPFLAGS="-I/usr/local/opt/openssl/include"

For pkg-config to find openssl you may need to set:
  export PKG_CONFIG_PATH="/usr/local/opt/openssl/lib/pkgconfig"

==> Summary
🍺  /usr/local/Cellar/openssl/1.0.2q: 1,794 files, 12.1MB
==> Installing octave dependency: open-mpi
==> Downloading https://homebrew.bintray.com/bottles/open-mpi-3.1.3.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring open-mpi-3.1.3.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/open-mpi/3.1.3: 737 files, 10.5MB
==> Installing octave dependency: sundials
==> Downloading https://homebrew.bintray.com/bottles/sundials-3.2.0.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring sundials-3.2.0.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/sundials/3.2.0: 512 files, 7.5MB
==> Installing octave dependency: texinfo
==> Downloading https://homebrew.bintray.com/bottles/texinfo-6.5.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring texinfo-6.5.mojave.bottle.tar.gz
==> Caveats
texinfo is keg-only, which means it was not symlinked into /usr/local,
because software that uses TeX, such as lilypond and octave, require a newer
version of these files.

If you need to have texinfo first in your PATH run:
  echo 'export PATH="/usr/local/opt/texinfo/bin:$PATH"' >> ~/.zshrc

==> Summary
🍺  /usr/local/Cellar/texinfo/6.5: 403 files, 8.2MB
==> Installing octave
==> Downloading https://homebrew.bintray.com/bottles/octave-4.4.1_3.mojave.bottle.tar.gz
######################################################################## 100.0%
==> Pouring octave-4.4.1_3.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/octave/4.4.1_3: 2,187 files, 48.5MB
==> Caveats
==> icu4c
icu4c is keg-only, which means it was not symlinked into /usr/local,
because macOS provides libicucore.dylib (but nothing else).

If you need to have icu4c first in your PATH run:
  echo 'export PATH="/usr/local/opt/icu4c/bin:$PATH"' >> ~/.zshrc
  echo 'export PATH="/usr/local/opt/icu4c/sbin:$PATH"' >> ~/.zshrc

For compilers to find icu4c you may need to set:
  export LDFLAGS="-L/usr/local/opt/icu4c/lib"
  export CPPFLAGS="-I/usr/local/opt/icu4c/include"

For pkg-config to find icu4c you may need to set:
  export PKG_CONFIG_PATH="/usr/local/opt/icu4c/lib/pkgconfig"

==> libtool
In order to prevent conflicts with Apple's own libtool we have prepended a "g"
so, you have instead: glibtool and glibtoolize.
==> openssl
A CA file has been bootstrapped using certificates from the SystemRoots
keychain. To add additional certificates (e.g. the certificates added in
the System keychain), place .pem files in
  /usr/local/etc/openssl/certs

and run
  /usr/local/opt/openssl/bin/c_rehash

openssl is keg-only, which means it was not symlinked into /usr/local,
because Apple has deprecated use of OpenSSL in favor of its own TLS and crypto libraries.

If you need to have openssl first in your PATH run:
  echo 'export PATH="/usr/local/opt/openssl/bin:$PATH"' >> ~/.zshrc

For compilers to find openssl you may need to set:
  export LDFLAGS="-L/usr/local/opt/openssl/lib"
  export CPPFLAGS="-I/usr/local/opt/openssl/include"

For pkg-config to find openssl you may need to set:
  export PKG_CONFIG_PATH="/usr/local/opt/openssl/lib/pkgconfig"

==> texinfo
texinfo is keg-only, which means it was not symlinked into /usr/local,
because software that uses TeX, such as lilypond and octave, require a newer
version of these files.

If you need to have texinfo first in your PATH run:
  echo 'export PATH="/usr/local/opt/texinfo/bin:$PATH"' >> ~/.zshrc

```
`https://homebrew.bintray.com/bottles/ghostscript-9.26.mojave.bottle.tar.gz` のバイナリダウンロードは失敗したようだが、リカバリーのソースビルドが成功したようなので良しとする
```
takyshu98s-mbp{takyshu98}% octave -v
GNU Octave, version 4.4.1
Copyright (C) 2018 John W. Eaton and others.
This is free software; see the source code for copying conditions.
There is ABSOLUTELY NO WARRANTY; not even for MERCHANTABILITY or
FITNESS FOR A PARTICULAR PURPOSE.

Octave was configured for "x86_64-apple-darwin18.2.0".

Additional information about Octave is available at https://www.octave.org.

Please contribute if you find this software useful.
For more information, visit https://www.octave.org/get-involved.html

Read https://www.octave.org/bugs.html to learn how to submit bug reports.
[~/tmp/coursera-machine-learning/week02/enviroment_setup_instructions]
```
