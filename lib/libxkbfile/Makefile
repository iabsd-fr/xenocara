# $OpenBSD: Makefile,v 1.1 2026/05/14 14:21:28 matthieu Exp $

SUBDIR = mk

build:
	su ${BUILDUSER} -c 'exec ${MAKE} -C ${.CURDIR} cleandir'
	su ${BUILDUSER} -c 'exec ${MAKE} -C ${.CURDIR} all'
	exec ${MAKE} -C ${.CURDIR} install

.include <bsd.subdir.mk>
.include <bsd.xorg.mk>
