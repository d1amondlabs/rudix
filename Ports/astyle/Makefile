include ../../Library/Unix.mk

Title=		Artistic Style
Name=		astyle
Version=	2.02.1
Revision=	0
URL=		http://downloads.sourceforge.net/astyle
Source=		$(Name)_$(Version)_macosx.tar.gz

ReadMeFile=	$(SourceDir)/doc/index.html
LicenseFile=	$(SourceDir)/doc/license.html

UncompressedName = $(Name)
BuildDir=	$(SourceDir)/build/mac

MakeInstallExtra += prefix=$(InstallDir)$(Prefix)
MakeInstallExtra += INSTALL=install

define install_post_hook
install -m 644 $(SourceDir)/doc/* $(InstallDir)/$(DocDir)/$(Name)
install -d $(InstallDir)/$(BinDir)
install -m 755 $(BuildDir)/bin/astyle $(InstallDir)/$(BinDir)
endef

define test_inner_hook
endef

define final_inner_hook
$(BinDir)/astyle  --version
endef
