PROGRAM = x

INSTALL     = install
INSTALL_BIN = $(INSTALL) -D -m 755
INSTALL_DAT = $(INSTALL) -D -m 644

PREFIX = /usr/local

BIN_DIR = $(PREFIX)/bin
DAT_DIR = $(PREFIX)/share
COM_DIR = bash-completion/completions

all:
.PHONY: all

install:
	$(INSTALL_BIN)            $(PROGRAM) $(DESTDIR)$(BIN_DIR)/$(PROGRAM)
	$(INSTALL_DAT) $(COM_DIR)/$(PROGRAM) $(DESTDIR)$(DAT_DIR)/$(COM_DIR)/$(PROGRAM)
.PHONY: install

uninstall:
	$(RM) $(DESTDIR)$(BIN_DIR)/$(PROGRAM)
	$(RM) $(DESTDIR)$(DAT_DIR)/$(COM_DIR)/$(PROGRAM)
.PHONY: uninstall
