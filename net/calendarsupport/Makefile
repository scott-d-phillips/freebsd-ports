# $FreeBSD$

PORTNAME=	calendarsupport
DISTVERSION=	${KDE_APPLICATIONS_VERSION}
CATEGORIES=	net kde kde-applications

MAINTAINER=	kde@FreeBSD.org
COMMENT=	Calendar support libriares for KDEPim

LICENSE=	LGPL21

LIB_DEPENDS=	libboost_system.so:devel/boost-libs

USES=		cmake:outsource compiler:c++11-lib gettext kde:5 tar:xz
USE_KDE=	auth codecs completion config configwidgets coreaddons ecm \
		guiaddons i18n iconthemes itemmodels jobwidgets kio service \
		widgetsaddons
# pim components
USE_KDE+=	akonadi akonadicalendar calendarcore calendarutils holidays \
		identitymanagement kdepim-apps-libs mime pimcommon pimtextedit
USE_QT5=	core gui network printsupport testlib uitools widgets xml \
		buildtools_build qmake_build
USE_LDCONFIG=	yes

.include <bsd.port.mk>
