PORTNAME=	automake
PORTVERSION=	1.16.5
CATEGORIES=	devel
MASTER_SITES=	GNU

BROKEN_purecap=	requires missing CheriABI Python
USE_PKG64=	1

MAINTAINER=	tijl@FreeBSD.org
COMMENT=	GNU Standards-compliant Makefile generator
WWW=		https://www.gnu.org/software/automake/

LICENSE=	GPLv2+ GFDL
LICENSE_COMB=	multi
LICENSE_FILE_GPLv2+ =	${WRKSRC}/COPYING
LICENSE_FILE_GFDL=	${WRKSRC}/doc/fdl.texi

BUILD_DEPENDS=	autoconf>=2.69:devel/autoconf
RUN_DEPENDS=	autoconf>=2.69:devel/autoconf

BUILD_VERSION=	1.16
PLIST_SUB=	BUILD_VERSION=${BUILD_VERSION}
USES=		cpe perl5 tar:xz
GNU_CONFIGURE=	yes
INFO=		automake automake-history
CPE_VENDOR=	gnu

NO_ARCH=	yes

OPTIONS_DEFINE=	DOCS

.include <bsd.port.mk>
