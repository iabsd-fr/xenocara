# $OpenBSD: Makefile,v 1.1 2025/08/12 16:39:28 matthieu Exp $

SUBDIR = mk

build:
	su ${BUILDUSER} -c 'exec ${MAKE} -C ${.CURDIR} cleandir'
	su ${BUILDUSER} -c 'exec ${MAKE} -C ${.CURDIR} all'
	exec ${MAKE} -C ${.CURDIR} install

.include <bsd.subdir.mk>
.include <bsd.xorg.mk>
