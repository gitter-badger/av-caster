# Automatically generated makefile, created by the Introjucer
# Don't edit this file! Your changes will be overwritten when you re-save the Introjucer project!

# (this disables dependency generation if multiple architectures are set)
DEPFLAGS := $(if $(word 2, $(TARGET_ARCH)), , -MMD)

ifndef CONFIG
  CONFIG=Debug
endif

ifeq ($(CONFIG),Debug)
  BINDIR := build
  LIBDIR := build
  OBJDIR := build/intermediate/Debug
  OUTDIR := build

  ifeq ($(TARGET_ARCH),)
    TARGET_ARCH := -march=native
  endif

  CPPFLAGS := $(DEPFLAGS) -std=c++11 -D "LINUX=1" -D "DEBUG=1" -D "_DEBUG=1" -D "JUCER_LINUX_MAKE_CE4F43AE=1" -D "JUCE_APP_VERSION=0.15.0" -D "JUCE_APP_VERSION_HEX=0xf00" -I /usr/include -I /usr/include/freetype2 -I ../../JuceLibraryCode -I ../../JuceLibraryCode/modules
  CFLAGS += $(CPPFLAGS) $(TARGET_ARCH) -g -ggdb -O0 `pkg-config --cflags gstreamer-1.0`
  CXXFLAGS += $(CFLAGS)
  LDFLAGS += $(TARGET_ARCH) -L$(BINDIR) -L$(LIBDIR) -lX11 -lXext -lXinerama -ldl -lfreetype -lpthread -lrt `pkg-config --libs gstreamer-1.0` `pkg-config --libs gstreamer-video-1.0`

  TARGET := av-caster-dbg
  BLDCMD = $(CXX) -o $(OUTDIR)/$(TARGET) $(OBJECTS) $(LDFLAGS) $(RESOURCES) $(TARGET_ARCH)
  CLEANCMD = rm -rf $(OUTDIR)/$(TARGET) $(OBJDIR)
endif

ifeq ($(CONFIG),Release)
  BINDIR := build
  LIBDIR := build
  OBJDIR := build/intermediate/Release
  OUTDIR := build

  ifeq ($(TARGET_ARCH),)
    TARGET_ARCH := -march=native
  endif

  CPPFLAGS := $(DEPFLAGS) -std=c++11 -D "LINUX=1" -D "NDEBUG=1" -D "JUCER_LINUX_MAKE_CE4F43AE=1" -D "JUCE_APP_VERSION=0.15.0" -D "JUCE_APP_VERSION_HEX=0xf00" -I /usr/include -I /usr/include/freetype2 -I ../../JuceLibraryCode -I ../../JuceLibraryCode/modules
  CFLAGS += $(CPPFLAGS) $(TARGET_ARCH) -O3 `pkg-config --cflags gstreamer-1.0`
  CXXFLAGS += $(CFLAGS)
  LDFLAGS += $(TARGET_ARCH) -L$(BINDIR) -L$(LIBDIR) -fvisibility=hidden -lX11 -lXext -lXinerama -ldl -lfreetype -lpthread -lrt `pkg-config --libs gstreamer-1.0` `pkg-config --libs gstreamer-video-1.0`

  TARGET := av-caster
  BLDCMD = $(CXX) -o $(OUTDIR)/$(TARGET) $(OBJECTS) $(LDFLAGS) $(RESOURCES) $(TARGET_ARCH)
  CLEANCMD = rm -rf $(OUTDIR)/$(TARGET) $(OBJDIR)
endif

ifeq ($(CONFIG),Release32)
  BINDIR := build
  LIBDIR := build
  OBJDIR := build/intermediate/Release32
  OUTDIR := build

  ifeq ($(TARGET_ARCH),)
    TARGET_ARCH := -m32
  endif

  CPPFLAGS := $(DEPFLAGS) -std=c++11 -D "LINUX=1" -D "NDEBUG=1" -D "JUCER_LINUX_MAKE_CE4F43AE=1" -D "JUCE_APP_VERSION=0.15.0" -D "JUCE_APP_VERSION_HEX=0xf00" -I /usr/include -I /usr/include/freetype2 -I ../../JuceLibraryCode -I ../../JuceLibraryCode/modules
  CFLAGS += $(CPPFLAGS) $(TARGET_ARCH) -O3 `pkg-config --cflags gstreamer-1.0`
  CXXFLAGS += $(CFLAGS)
  LDFLAGS += $(TARGET_ARCH) -L$(BINDIR) -L$(LIBDIR) -fvisibility=hidden -lX11 -lXext -lXinerama -ldl -lfreetype -lpthread -lrt `pkg-config --libs gstreamer-1.0` `pkg-config --libs gstreamer-video-1.0`

  TARGET := av-caster
  BLDCMD = $(CXX) -o $(OUTDIR)/$(TARGET) $(OBJECTS) $(LDFLAGS) $(RESOURCES) $(TARGET_ARCH)
  CLEANCMD = rm -rf $(OUTDIR)/$(TARGET) $(OBJDIR)
endif

OBJECTS := \
  $(OBJDIR)/AvCaster_86a5e2ca.o \
  $(OBJDIR)/AvCasterStore_6b7801.o \
  $(OBJDIR)/Background_ba4a3b7.o \
  $(OBJDIR)/Config_5aed31cb.o \
  $(OBJDIR)/Controls_28d2363f.o \
  $(OBJDIR)/Gstreamer_49eed0f5.o \
  $(OBJDIR)/Main_90ebc5c2.o \
  $(OBJDIR)/MainContent_6313eee1.o \
  $(OBJDIR)/PresetSeed_7897bb79.o \
  $(OBJDIR)/Preview_b7601029.o \
  $(OBJDIR)/Statusbar_a0c28bc2.o \
  $(OBJDIR)/Trace_fd3024bc.o \
  $(OBJDIR)/juce_core_aff681cc.o \
  $(OBJDIR)/juce_data_structures_bdd6d488.o \
  $(OBJDIR)/juce_events_79b2840.o \
  $(OBJDIR)/juce_graphics_c8f1e7a4.o \
  $(OBJDIR)/juce_gui_basics_a630dd20.o \

.PHONY: clean

$(OUTDIR)/$(TARGET): $(OBJECTS) $(RESOURCES)
	@echo Linking AvCaster
	-@mkdir -p $(BINDIR)
	-@mkdir -p $(LIBDIR)
	-@mkdir -p $(OUTDIR)
	@$(BLDCMD)

clean:
	@echo Cleaning AvCaster
	@$(CLEANCMD)

strip:
	@echo Stripping AvCaster
	-@strip --strip-unneeded $(OUTDIR)/$(TARGET)

$(OBJDIR)/AvCaster_86a5e2ca.o: ../../Source/AvCaster.cpp
	-@mkdir -p $(OBJDIR)
	@echo "Compiling AvCaster.cpp"
	@$(CXX) $(CXXFLAGS) -o "$@" -c "$<"

$(OBJDIR)/AvCasterStore_6b7801.o: ../../Source/AvCasterStore.cpp
	-@mkdir -p $(OBJDIR)
	@echo "Compiling AvCasterStore.cpp"
	@$(CXX) $(CXXFLAGS) -o "$@" -c "$<"

$(OBJDIR)/Background_ba4a3b7.o: ../../Source/Background.cpp
	-@mkdir -p $(OBJDIR)
	@echo "Compiling Background.cpp"
	@$(CXX) $(CXXFLAGS) -o "$@" -c "$<"

$(OBJDIR)/Config_5aed31cb.o: ../../Source/Config.cpp
	-@mkdir -p $(OBJDIR)
	@echo "Compiling Config.cpp"
	@$(CXX) $(CXXFLAGS) -o "$@" -c "$<"

$(OBJDIR)/Controls_28d2363f.o: ../../Source/Controls.cpp
	-@mkdir -p $(OBJDIR)
	@echo "Compiling Controls.cpp"
	@$(CXX) $(CXXFLAGS) -o "$@" -c "$<"

$(OBJDIR)/Gstreamer_49eed0f5.o: ../../Source/Gstreamer.cpp
	-@mkdir -p $(OBJDIR)
	@echo "Compiling Gstreamer.cpp"
	@$(CXX) $(CXXFLAGS) -o "$@" -c "$<"

$(OBJDIR)/Main_90ebc5c2.o: ../../Source/Main.cpp
	-@mkdir -p $(OBJDIR)
	@echo "Compiling Main.cpp"
	@$(CXX) $(CXXFLAGS) -o "$@" -c "$<"

$(OBJDIR)/MainContent_6313eee1.o: ../../Source/MainContent.cpp
	-@mkdir -p $(OBJDIR)
	@echo "Compiling MainContent.cpp"
	@$(CXX) $(CXXFLAGS) -o "$@" -c "$<"

$(OBJDIR)/PresetSeed_7897bb79.o: ../../Source/PresetSeed.cpp
	-@mkdir -p $(OBJDIR)
	@echo "Compiling PresetSeed.cpp"
	@$(CXX) $(CXXFLAGS) -o "$@" -c "$<"

$(OBJDIR)/Preview_b7601029.o: ../../Source/Preview.cpp
	-@mkdir -p $(OBJDIR)
	@echo "Compiling Preview.cpp"
	@$(CXX) $(CXXFLAGS) -o "$@" -c "$<"

$(OBJDIR)/Statusbar_a0c28bc2.o: ../../Source/Statusbar.cpp
	-@mkdir -p $(OBJDIR)
	@echo "Compiling Statusbar.cpp"
	@$(CXX) $(CXXFLAGS) -o "$@" -c "$<"

$(OBJDIR)/Trace_fd3024bc.o: ../../Source/Trace/Trace.cpp
	-@mkdir -p $(OBJDIR)
	@echo "Compiling Trace.cpp"
	@$(CXX) $(CXXFLAGS) -o "$@" -c "$<"

$(OBJDIR)/juce_core_aff681cc.o: ../../JuceLibraryCode/modules/juce_core/juce_core.cpp
	-@mkdir -p $(OBJDIR)
	@echo "Compiling juce_core.cpp"
	@$(CXX) $(CXXFLAGS) -o "$@" -c "$<"

$(OBJDIR)/juce_data_structures_bdd6d488.o: ../../JuceLibraryCode/modules/juce_data_structures/juce_data_structures.cpp
	-@mkdir -p $(OBJDIR)
	@echo "Compiling juce_data_structures.cpp"
	@$(CXX) $(CXXFLAGS) -o "$@" -c "$<"

$(OBJDIR)/juce_events_79b2840.o: ../../JuceLibraryCode/modules/juce_events/juce_events.cpp
	-@mkdir -p $(OBJDIR)
	@echo "Compiling juce_events.cpp"
	@$(CXX) $(CXXFLAGS) -o "$@" -c "$<"

$(OBJDIR)/juce_graphics_c8f1e7a4.o: ../../JuceLibraryCode/modules/juce_graphics/juce_graphics.cpp
	-@mkdir -p $(OBJDIR)
	@echo "Compiling juce_graphics.cpp"
	@$(CXX) $(CXXFLAGS) -o "$@" -c "$<"

$(OBJDIR)/juce_gui_basics_a630dd20.o: ../../JuceLibraryCode/modules/juce_gui_basics/juce_gui_basics.cpp
	-@mkdir -p $(OBJDIR)
	@echo "Compiling juce_gui_basics.cpp"
	@$(CXX) $(CXXFLAGS) -o "$@" -c "$<"

-include $(OBJECTS:%.o=%.d)
