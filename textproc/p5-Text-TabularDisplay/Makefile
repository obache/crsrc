# $NetBSD: Makefile,v 1.19 2021/05/24 19:54:47 wiz Exp $
#

DISTNAME=	Text-TabularDisplay-1.38
PKGNAME=	p5-${DISTNAME}
PKGREVISION=	7
CATEGORIES=	textproc perl5
MASTER_SITES=	${MASTER_SITE_PERL_CPAN:=Text/}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://metacpan.org/release/Text-TabularDisplay
COMMENT=	Display text in formatted table output
LICENSE=	gnu-gpl-v2

USE_LANGUAGES=	# empty
PERL5_PACKLIST=	auto/Text/TabularDisplay/.packlist

.include "../../lang/perl5/module.mk"
.include "../../mk/bsd.pkg.mk"
