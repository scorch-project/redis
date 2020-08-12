# CHERI port of Redis

To compile for purecap:
```
gmake distclean
gmake CC=cheribsd128purecap-clang -C deps/hiredis clean
gmake CC=cheribsd128purecap-clang -C deps/linenoise
gmake CC=cheribsd128purecap-clang -C deps/lua/freebsd
gmake CC=cheribsd128purecap-clang
```

