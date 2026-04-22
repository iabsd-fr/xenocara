#	$OpenBSD: Makefile,v 1.2 2023/04/06 10:23:42 jsg Exp $

SUBDIR=	mk

build:
	su ${BUILDUSER} -c 'exec ${MAKE} -C ${.CURDIR} cleandir'
	su ${BUILDUSER} -c 'exec ${MAKE} -C ${.CURDIR} all'
	exec ${MAKE} -C ${.CURDIR} install

.include <bsd.subdir.mk>
.include <bsd.xorg.mk>
