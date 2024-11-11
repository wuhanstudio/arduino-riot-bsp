# name of your application
APPLICATION = arduino_mpu6050

# If no BOARD is found in the environment, use this default:
BOARD ?= arduino-uno
PORT_LINUX = /dev/ttyUSB0

# This has to be the absolute path to the RIOT base directory:
RIOTBASE ?= $(CURDIR)/../RIOT

INCLUDES += -I$(CURDIR)/mpu6050
DIRS += $(CURDIR)/mpu6050

INCLUDES += -I$(CURDIR)/madgwick
DIRS += $(CURDIR)/madgwick

USEMODULE += arduino
USEMODULE += stdio_uart_onlcr
USEMODULE += mpu6050
USEMODULE += madgwick

FEATURES_REQUIRED += cpp

# Comment this out to disable code in RIOT that does safety checking
# which is not needed in a production environment but helps in the
# development process:
DEVELHELP ?= 1

# Change this to 0 show compiler invocation lines by default:
QUIET ?= 1

include $(RIOTBASE)/Makefile.include
