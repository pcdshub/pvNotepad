TOP=../..

include $(TOP)/configure/CONFIG
#----------------------------------------
#  ADD MACRO DEFINITIONS AFTER THIS LINE
#=============================

#=============================
# Build an ioc application
PROD_IOC = pvNotepad

# pvNotepad.dbd will be created and installed
DBD += pvNotepad.dbd

# pvNotepad.dbd will be made up from these files:
pvNotepad_DBD += base.dbd
pvNotepad_DBD += PVAServerRegister.dbd
pvNotepad_DBD += qsrv.dbd
pvNotepad_DBD += iocAdmin.dbd
pvNotepad_DBD += asSupport.dbd

# <name>_registerRecordDeviceDriver.cpp will be created from <name>.dbd
pvNotepad_SRCS += pvNotepad_registerRecordDeviceDriver.cpp
pvNotepad_SRCS_DEFAULT += pvNotepadMain.cpp

# Add locally compiled object code

PROD_LIBS += qsrv
PROD_LIBS += $(EPICS_BASE_PVA_CORE_LIBS)

pvNotepad_LIBS += devIocStats
pvNotepad_LIBS += autosave
pvNotepad_LIBS += $(EPICS_BASE_IOC_LIBS)

#===========================

include $(TOP)/configure/RULES
#----------------------------------------
#  ADD RULES AFTER THIS LINE

