# $NetBSD: Makefile,v 1.4 2021/04/29 18:35:02 pin Exp $

DISTNAME=	qrrs-0.1.6
CATEGORIES=	graphics
MASTER_SITES=	${MASTER_SITE_GITHUB:=Lenivaya/}
GITHUB_TAG=	v${PKGVERSION_NOREV}

MAINTAINER=	pin@NetBSD.org
HOMEPAGE=	https://github.com/Lenivaya/qrrs/
COMMENT=	CLI tool for working with qr-codes
LICENSE=	mit

.include "cargo-depends.mk"

USE_LANGUAGES+=	c

INSTALLATION_DIRS=	bin

do-install:
	${INSTALL_PROGRAM} ${WRKSRC}/target/release/qrrs ${DESTDIR}${PREFIX}/bin

.include "../../lang/rust/cargo.mk"
.include "../../mk/bsd.pkg.mk"
