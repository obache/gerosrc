# $NetBSD: Makefile,v 1.18 2021/05/19 09:50:12 adam Exp $

DISTNAME=	asyncpg-0.23.0
PKGNAME=	${PYPKGPREFIX}-${DISTNAME}
CATEGORIES=	databases python
MASTER_SITES=	${MASTER_SITE_PYPI:=a/asyncpg/}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://github.com/MagicStack/asyncpg
COMMENT=	Asyncio PosgtreSQL driver
LICENSE=	apache-2.0

TEST_DEPENDS+=	${PYPKGPREFIX}-codestyle>=2.5.0:../../devel/py-codestyle
TEST_DEPENDS+=	${PYPKGPREFIX}-flake8>=3.7.9:../../devel/py-flake8
TEST_DEPENDS+=	${PYPKGPREFIX}-uvloop>=0.14.0:../../devel/py-uvloop

.include "../../lang/python/pyversion.mk"
.if ${_PYTHON_VERSION} < 38
DEPENDS+=	${PYPKGPREFIX}-typing-extensions>=3.7.4.3:../../devel/py-typing-extensions
.endif

PYTHON_VERSIONS_INCOMPATIBLE=	27 36

# Testing requires postgresql-contrib

.include "../../lang/python/egg.mk"
.include "../../mk/bsd.pkg.mk"
