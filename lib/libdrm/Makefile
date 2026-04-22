#	$OpenBSD: Makefile,v 1.13 2021/02/11 10:34:51 jsg Exp $

SUBDIR=	mk

build:
	su ${BUILDUSER} -c 'exec ${MAKE} -C ${.CURDIR} cleandir'
	su ${BUILDUSER} -c 'exec ${MAKE} -C ${.CURDIR} all'
	exec ${MAKE} -C ${.CURDIR} install

.include <bsd.subdir.mk>
.include <bsd.xorg.mk>
