# $OpenBSD: Makefile,v 1.6 2018/06/04 20:25:32 rsadowski Exp $

COMMENT =	create documentation from DocBook
DISTNAME =	kdoctools-${VERSION}

SHARED_LIBS +=  KF5DocTools               2.1 # 5.34

WANTLIB += ${COMPILER_LIBCXX} KF5Archive Qt5Core c exslt m xml2
WANTLIB += xslt

BUILD_DEPENDS =	devel/gettext-tools \
		devel/kf5/ki18n \
		textproc/docbook-xsl \
		www/p5-URI

RUN_DEPENDS =	devel/kf5/ki18n \
		textproc/docbook-xsl

LIB_DEPENDS =	devel/kf5/karchive \
		textproc/libxml \
		textproc/libxslt

.include <bsd.port.mk>
