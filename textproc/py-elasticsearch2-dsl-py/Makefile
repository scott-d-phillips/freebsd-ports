# Created by: Dan Langille <dvl@FreeBSD.org>
# $FreeBSD$

PORTNAME=	py-elasticsearch2-dsl-py
PORTVERSION=	2.1.0
PORTREVISION=	2
CATEGORIES=	textproc python
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	dvl@FreeBSD.org
COMMENT=	High level Python client for Elasticsearch

LICENSE=	APACHE20

DEPRECATED=	Needs Python ElasticSearch 2.x
EXPIRATION_DATE=	2018-06-14

RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}elasticsearch>=1.3.0:textproc/py-elasticsearch@${FLAVOR}

USE_GITHUB=	yes
GH_ACCOUNT=	elastic
GH_PROJECT=	elasticsearch-dsl-py

USES=		python:2.7
USE_PYTHON=	autoplist distutils

.include <bsd.port.mk>
