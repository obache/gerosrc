# $NetBSD: Makefile,v 1.8 2019/04/25 07:33:23 maya Exp $

DISTNAME=	cmark-0.29.0
PKGREVISION=	1
CATEGORIES=	textproc
MASTER_SITES=	${MASTER_SITE_GITHUB:=jgm/}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://github.com/commonmark/cmark
COMMENT=	CommonMark parsing and rendering library and program in C
LICENSE=	2-clause-bsd

USE_CMAKE=		yes
USE_LANGUAGES=		c c++
USE_TOOLS+=		pkg-config
CONFIGURE_DIRS=		build
CMAKE_ARG_PATH=		${WRKSRC}
PKGCONFIG_OVERRIDE+=	src/libcmark.pc.in

PYTHON_FOR_BUILD_ONLY=	yes

PYTHON_VERSIONS_INCOMPATIBLE=	27

TEST_TARGET=	test

post-extract:
	${MKDIR} ${WRKSRC}/build

.include "../../lang/python/tool.mk"
.include "../../mk/bsd.pkg.mk"
