# $NetBSD: Makefile,v 1.12 2021/05/24 19:52:49 wiz Exp $
#

DISTNAME=	Mail-POP3Client-2.19
PKGNAME=	p5-${DISTNAME}
PKGREVISION=	6
CATEGORIES=	mail
MASTER_SITES=	${MASTER_SITE_PERL_CPAN:=Mail/}

MAINTAINER=	ryoon@NetBSD.org
HOMEPAGE=	https://metacpan.org/release/Mail-POP3Client
COMMENT=	Perl 5 module to talk to a POP3 (RFC1939) server
LICENSE=	${PERL5_LICENSE}

PERL5_PACKLIST=	auto/Mail/POP3Client/.packlist
USE_LANGUAGES=	# none

.include "../../lang/perl5/module.mk"
.include "../../mk/bsd.pkg.mk"
