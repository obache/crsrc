# $NetBSD: Makefile,v 1.16 2012/10/23 17:18:45 asau Exp $
#

DISTNAME=	overnetclc-1.0.1
PKGNAME=	${DISTNAME:C/clc//}
PKGREVISION=	2
CATEGORIES=	net
MASTER_SITES=	http://www.zen18864.zen.co.uk/overnet/1.0.1/
DISTFILES=	${DISTNAME}-1.i386_compat.rpm

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://www.overnet.com/
COMMENT=	Peer-to-peer file sharing client (binary pkg)

EMUL_PLATFORMS=		linux-i386
EMUL_MODULES.linux=	compat

WRKSRC=			${WRKDIR}
BUILD_DIRS=		# empty

EMUL_PKG_FMT=		rpm
RPM2PKG_PLIST=		# empty
RPM2PKG_STRIP=		0
RUN_LDCONFIG=		no

INSTALLATION_DIRS=	bin share/doc/overnetclc share/overnetclc

do-install:
	${INSTALL_PROGRAM} ${WRKDIR}/usr/bin/overnetclc ${DESTDIR}${PREFIX}/bin
.for f in ChangeLog LISEZMOI README
	${INSTALL_DATA} ${WRKDIR}/usr/share/doc/overnetclc/${f}		\
	    ${DESTDIR}${PREFIX}/share/doc/overnetclc
.endfor
	${INSTALL_DATA} ${WRKSRC}/usr/share/overnetclc/contact.dat	\
	    ${DESTDIR}${PREFIX}/share/overnetclc

.include "../../mk/bsd.pkg.mk"
