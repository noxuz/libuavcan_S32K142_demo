################################################################################
# Automatically-generated file. Do not edit!
################################################################################

#Progress monitor hint: 4
first : all
-include ../makefile.init

# This file contains definitions of environment variables used in the makefiles and .args files if exist.
-include makefile.local

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include subdir.mk
-include Project_Settings/Linker_Files/subdir.mk
-include Project_Settings/Startup_Code/subdir.mk
-include src/subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(CC_DEPS)),)
-include $(CC_DEPS)
endif
ifneq ($(strip $(C++_DEPS)),)
-include $(C++_DEPS)
endif
ifneq ($(strip $(C_UPPER_DEPS)),)
-include $(C_UPPER_DEPS)
endif
ifneq ($(strip $(CXX_DEPS)),)
-include $(CXX_DEPS)
endif
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
ifneq ($(strip $(CPP_DEPS)),)
-include $(CPP_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 
EXECUTABLES += \
libuavcan_S32K142_demo.elf \

EXECUTABLES_QUOTED += \
"libuavcan_S32K142_demo.elf" \

EXECUTABLES_OS_FORMAT += \
libuavcan_S32K142_demo.elf \

SECONDARY_FLASH += \
libuavcan_S32K142_demo.srec \

SECONDARY_FLASH_QUOTED += \
"libuavcan_S32K142_demo.srec" \

SECONDARY_FLASH_OS_FORMAT += \
libuavcan_S32K142_demo.srec \

SECONDARY_SIZE += \
libuavcan_S32K142_demo.siz \

SECONDARY_SIZE_QUOTED += \
"libuavcan_S32K142_demo.siz" \

SECONDARY_SIZE_OS_FORMAT += \
libuavcan_S32K142_demo.siz \


# All Target
all: warning-messages explicit-dependencies libuavcan_S32K142_demo.elf secondary-outputs

# Tool invocations
libuavcan_S32K142_demo.elf: $(OBJS) C:/Users/noxuz/workspaceS32DS.ARM.2018.R1/libuavcan_S32K142_demo/libuavcan_S32K142_demo/Project_Settings/Linker_Files/S32K142_32_flash.ld $(USER_OBJS)
	@echo 'Building target: $@'
	@echo 'Executing target #5 $@'
	@echo 'Invoking: Standard S32DS C++ Linker'
	arm-none-eabi-g++ -o "libuavcan_S32K142_demo.elf" "@libuavcan_S32K142_demo.args"  $(USER_OBJS_QUOTED) $(LIBS_QUOTED)
	@echo 'Finished building target: $@'
	@echo ' '

libuavcan_S32K142_demo.srec: $(EXECUTABLES)
	@echo 'Executing target #6 $@'
	@echo 'Invoking: Standard S32DS Create Flash Image'
	arm-none-eabi-objcopy -O srec $(EXECUTABLES)  "libuavcan_S32K142_demo.srec"
	@echo 'Finished building: $@'
	@echo ' '

libuavcan_S32K142_demo.siz: $(EXECUTABLES)
	@echo 'Executing target #7 $@'
	@echo 'Invoking: Standard S32DS Print Size'
	arm-none-eabi-size --format=berkeley $(EXECUTABLES)
	@echo 'Finished building: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) $(SECONDARY_FLASH_QUOTED) ./*/*.d  $(CC_DEPS_QUOTED) $(CXX_DEPS_QUOTED) $(C_UPPER_DEPS_QUOTED) $(SECONDARY_SIZE_QUOTED) $(C++_DEPS_QUOTED) ./*/*/*.d  ./*/*.o ./*/*/*.o  $(EXECUTABLES_QUOTED)
	-@echo ' '

secondary-outputs: $(SECONDARY_FLASH) $(SECONDARY_SIZE)

.PHONY: all clean dependents explicit-dependencies warning-messages
.SECONDARY:

-include ../makefile.targets

explicit-dependencies: 

warning-messages: 

