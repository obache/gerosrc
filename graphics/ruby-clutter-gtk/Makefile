# $NetBSD: Makefile,v 1.28 2020/08/17 20:19:09 leot Exp $
#

DISTNAME=		clutter-gtk-${VERSION}
COMMENT=		Ruby binding of Clutter-GTK
PKGREVISION=		1
CATEGORIES=		graphics

MAINTAINER=		pkgsrc-users@NetBSD.org

CONFLICTS+=		${RUBY_PKGPREFIX}-gnome2-clutter-gtk>=3.0.7nb1
SUPERSEDES+=		${RUBY_PKGPREFIX}-gnome2-clutter-gtk>=3.0.7nb1

DEPENDS+=	${RUBY_PKGPREFIX}-clutter>=${VERSION}:../../graphics/ruby-clutter
DEPENDS+=	${RUBY_PKGPREFIX}-clutter-gdk>=${VERSION}:../../graphics/ruby-clutter-gdk
DEPENDS+=	${RUBY_PKGPREFIX}-gtk3>=${VERSION}:../../x11/ruby-gtk3
DEPENDS+=	clutter-gtk>=1.0:../../graphics/clutter-gtk

.include "../../graphics/clutter-gtk/buildlink3.mk"
.include "../../meta-pkgs/ruby-gnome/Makefile.common"
.include "../../lang/ruby/gem.mk"
.include "../../mk/bsd.pkg.mk"
