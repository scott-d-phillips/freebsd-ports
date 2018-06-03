# $FreeBSD$

PORTNAME=	sway
PORTVERSION=	1.0.alpha.2
CATEGORIES=	graphics

MAINTAINER=	scott.d.phillips@intel.com
COMMENT=	i3-compatible Wayland compositor

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE

BUILD_DEPENDS=	wayland-protocols>=1.14:graphics/wayland-protocols
LIB_DEPENDS=	libinput.so:x11/libinput \
		libjson-c.so:devel/json-c \
		libpcre.so:devel/pcre \
		libwayland-client.so:graphics/wayland \
		libwayland-cursor.so:graphics/wayland \
		libwayland-server.so:graphics/wayland \
		libwlroots.so:graphics/wlroots \
		libxkbcommon.so:x11/libxkbcommon

USES=		meson pkgconfig
USE_GITHUB=	yes
USE_GNOME=	cairo gdkpixbuf2 glib20 pango
USE_XORG=	pixman

MESON_ARGS=	-Dsway_version=${PORTVERSION}

GH_ACCOUNT=	swaywm
GH_TAGNAME=	1.0-alpha.2

.include <bsd.port.mk>
