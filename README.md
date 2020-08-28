FMP Tools
--

Some tools for reading FileMaker Pro files (fp3, fp5, fp7, and fmp12).

Building requires [autoconf](https://www.gnu.org/software/autoconf/):

```
autoreconf -i -f
./configure
make
make install
```

The tools installed to `$PREFIX/bin` include:

* `fmp2excel` - Convert a FileMaker Pro database to Excel (requires [libxlsxwriter](http://libxlsxwriter.github.io))
* `fmp2json` - Convert a FileMaker Pro database to JSON (requires [yajl](https://lloyd.github.io/yajl/))
* `fmp2sqlite` - Convert a FileMaker Pro database to SQLite (requires [sqlite](https://www.sqlite.org/index.html))

There is also a C library installed that is used by the above tools, but the
API is subject to change.

You might also enjoy [fp5dump](https://github.com/qwesda/fp5dump), although
that project does not read the newer fp7 and fmp12 formats.
