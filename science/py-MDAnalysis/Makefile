# $FreeBSD$

PORTNAME=	MDAnalysis
DISTVERSION=	0.18.0
CATEGORIES=	science python
MASTER_SITES=	CHEESESHOP
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	yuri@FreeBSD.org
COMMENT=	Python library to analyze molecular dynamics trajectories

LICENSE=	GPLv2
LICENSE_FILE=	${WRKSRC}/LICENSE

BUILD_DEPENDS=	${PYNUMPY}
RUN_DEPENDS=	${PYNUMPY} \
		${PYTHON_PKGNAMEPREFIX}biopython>=1.59:biology/py-biopython@${FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}duecredit>0:textproc/py-duecredit@${FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}GridDataFormats>=0.4.0:math/py-GridDataFormats@${FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}gsd>=1.4.0:science/py-gsd@${FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}joblib>0:devel/py-joblib@${FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}matplotlib>=1.5.1:math/py-matplotlib@${FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}mmtf-python>=1.0.0:science/py-mmtf-python@${FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}networkx>=1.0:math/py-networkx@${FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}scipy>0:science/py-scipy@${FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}six>=1.4.0:devel/py-six@${FLAVOR}

USES=		python
USE_PYTHON=	distutils autoplist

.include <bsd.port.mk>
