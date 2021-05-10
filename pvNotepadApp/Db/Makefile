TOP=../..
include $(TOP)/configure/CONFIG
#----------------------------------------
#  ADD MACRO DEFINITIONS AFTER THIS LINE

#----------------------------------------------------
#  Optimization of db files using dbst (DEFAULT: NO)
#DB_OPT = YES

#----------------------------------------------------
# Create and install (or just install)
# databases, templates, substitutions like this
DB_INSTALLS += $(IOCADMIN)/db/iocSoft.db
DB_INSTALLS += $(AUTOSAVE)/db/save_restoreStatus.db

DB += array_1.db
DB += array_10.db
DB += array_20.db
DB += special_ao.db special_bo.db special_longout.db special_waveform.db special_stringin.db
DB += special_mbbo.db
DB += special_array.db
DB += hutch.db
#----------------------------------------------------
# Create and install (or just install)
# Archive files, templates, substitutions like this

ARCHIVE += archive_record.tpl-arch

#----------------------------------------------------
# Create and install (or just install)
# Autosave request files, templates, substitutions like this

REQ += autosave_record.tpl-req

include $(TOP)/configure/RULES
#----------------------------------------
#  ADD RULES AFTER THIS LINE

