BuildRequires += $(LibDir)/libevent.la

include ../../Library/GNU.mk

Title=		libMemcached
Name=		libmemcached
Version=	1.0.8
Revision=	0
URL=		http://launchpad.net/libmemcached/1.0/$(Version)/+download/
Source=		$(Name)-$(Version).tar.gz

ReadMeFile=	$(SourceDir)/README
LicenseFile=	$(SourceDir)/COPYING

ifdef ONLY_STATIC_LIBS
GnuConfigureExtra += --enable-static --disable-shared
endif
