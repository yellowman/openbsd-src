.include <bsd.own.mk>

PROG=	newfs_hammer2
SRCS=	newfs_hammer2.c mkfs_hammer2.c ondisk.c subs.c xxhash.c icrc32.c
MAN=	newfs_hammer2.8

.PATH:	../hammer2 ../../sys/lib/libkern ../../sys/hammer2/xxhash

WARNS=	5

CFLAGS+=	-I../../sys
CFLAGS+=	-I../hammer2

DPADD+=		${LIBUTIL}
LDADD+=		-lutil

.include <bsd.prog.mk>
