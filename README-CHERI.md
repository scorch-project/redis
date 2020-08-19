# CHERI port of Redis

To compile for purecap:
```
gmake distclean
gmake CC=cheribsd128purecap-clang
```

Transfer the necessary files to the cheri VM:
```
scp -P 18999 -r  src/redis-server src/redis-benchmark redis.conf localhost:~
```

