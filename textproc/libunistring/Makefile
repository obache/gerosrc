# $NetBSD: Makefile,v 1.13 2020/01/18 23:35:29 rillig Exp $

DISTNAME=	libunistring-0.9.10
CATEGORIES=	textproc
MASTER_SITES=	${MASTER_SITE_GNU:=libunistring/}

MAINTAINER=	gdt@NetBSD.org
HOMEPAGE=	https://www.gnu.org/software/libunistring/
COMMENT=	Unicode string library
LICENSE=	gnu-lgpl-v3 OR gnu-gpl-v2

GNU_CONFIGURE=	yes
USE_LIBTOOL=	yes
INFO_FILES=	yes

.include "../../converters/libiconv/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
