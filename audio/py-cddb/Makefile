# $NetBSD: Makefile,v 1.28 2020/01/26 05:26:13 rillig Exp $

DISTNAME=	CDDB-1.4
PKGNAME=	${PYPKGPREFIX}-cddb-1.4
PKGREVISION=	2
CATEGORIES=	audio python
MASTER_SITES=	${MASTER_SITE_SOURCEFORGE:=cddb-py/}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://cddb-py.sourceforge.net/
COMMENT=	Python module to access the CDDB online database
LICENSE=	gnu-gpl-v2

PYTHON_VERSIONS_ACCEPTED=	27 # not yet ported as of 1.4

.include "../../lang/python/distutils.mk"
.include "../../mk/bsd.pkg.mk"
