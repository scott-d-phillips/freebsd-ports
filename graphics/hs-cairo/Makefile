# $FreeBSD$

PORTNAME=	cairo
PORTVERSION=	0.13.5.0
CATEGORIES=	graphics haskell

MAINTAINER=	haskell@FreeBSD.org
COMMENT=	Binding to the Cairo library

LICENSE=	BSD3CLAUSE

USES=		pkgconfig
USE_CABAL=	gtk2hs-buildtools mtl utf8-string

BUILD_DEPENDS+=	${LOCALBASE}/libdata/pkgconfig/cairo-pdf.pc:graphics/cairo

.include "${.CURDIR}/../../lang/ghc/bsd.cabal.mk"
.include <bsd.port.mk>
