# $NetBSD: Makefile,v 1.12 2020/12/04 20:45:43 nia Exp $

DISTNAME=	vxargs-0.3.3
PKGREVISION=	5
CATEGORIES=	sysutils
#MASTER_SITES=	http://dharma.cis.upenn.edu/planetlab/vxargs/
EXTRACT_SUFX=	.py

MAINTAINER=	pkgsrc-users@NetBSD.org
#HOMEPAGE=	http://dharma.cis.upenn.edu/planetlab/vxargs/
COMMENT=	Runs parallel jobs with visualization and redirection

DEPENDS+=	${PYPKGPREFIX}-curses>=0nb4:../../devel/py-curses

EXTRACT_CMD=	${CP} $${extract_file} ${WRKSRC}/vxargs.py
NO_BUILD=	yes
WRKSRC=		${WRKDIR}

INSTALLATION_DIRS=	bin

REPLACE_PYTHON=	vxargs.py

.include "../../lang/python/application.mk"

do-install:
	${INSTALL_SCRIPT} ${WRKSRC}/vxargs.py ${DESTDIR}${PREFIX}/bin/vxargs

.include "../../mk/bsd.pkg.mk"
