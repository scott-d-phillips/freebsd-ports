# $FreeBSD$

PORTNAME=	bareos

PKGNAMESUFFIX=	-traymonitor
PORTREVISION=	1

COMMENT=	Backup archiving recovery open sourced (traymonitor)

LIB_DEPENDS+=	libqwt.so:x11-toolkits/qwt5 \
		libbareos.so:sysutils/bareos-client

CONFLICTS=	bacula*-bat-* bareos16-traymonitor-*

USES=		pkgconfig gettext-runtime desktop-file-utils
USE_QT4=	qmake_build uic_build moc_build rcc_build gui corelib
WITH_BAT=	yes

PLIST=		${.CURDIR}/pkg-plist
MAKE_ENV+=	MAKEOBJDIRPREFIX=/

MASTERDIR=	${.CURDIR}/../../sysutils/bareos-server

CONFIGURE_ARGS+=	--enable-traymonitor=yes \
			--with-qwt=${LOCALBASE}/lib \
			--disable-build-dird \
			--disable-build-stored \
			--enable-client-only \
			--with-jansson=${LOCALBASE} \
			--enable-nls=yes

.include "${MASTERDIR}/Makefile"
