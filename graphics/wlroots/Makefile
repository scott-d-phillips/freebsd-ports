# $FreeBSD$

PORTNAME=	wlroots
PORTVERSION=	1.0.alpha.2
CATEGORIES=	graphics

MAINTAINER=	scott.d.phillips@intel.com
COMMENT=	Pluggable, composable, unopinionated modules for building a Wayland compositor

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE

BUILD_DEPENDS=	wayland-protocols>=1.14:graphics/wayland-protocols \
		xcb-util-image>=0:x11/xcb-util-image

LIB_DEPENDS=	libdrm.so:graphics/libdrm \
		libinput.so:x11/libinput \
		libudev.so:devel/libudev-devd \
		libwayland-client.so:graphics/wayland \
		libwayland-egl.so:graphics/wayland \
		libwayland-server.so:graphics/wayland \
		libxcb-icccm.so:x11/xcb-util-wm \
		libxkbcommon.so:x11/libxkbcommon


USES=		meson pkgconfig
USE_GITHUB=	yes
USE_GL=		egl gbm glesv2
USE_XORG=	pixman x11 xcb

MESON_ARGS=	-Db_lundef=false -Denable-examples=false -Denable-rootston=false

GH_ACCOUNT=	swaywm
GH_TAGNAME=	383ce3d

.include <bsd.port.mk>
