# $NetBSD: Makefile,v 1.7 2017/09/11 07:54:27 wiz Exp $

DISTNAME=	chironfs-1.1.1
PKGNAME=	fuse-chironfs-1.1.1
PKGREVISION=	1
CATEGORIES=	filesystems
MASTER_SITES=	http://chironfs.googlecode.com/files/

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://github.com/tweksteen/chironfs
COMMENT=	Replicating file system
LICENSE=	gnu-gpl-v3

GNU_CONFIGURE=	yes

LDFLAGS.DragonFly+=	-lpthread

.include "../../mk/fuse.buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
