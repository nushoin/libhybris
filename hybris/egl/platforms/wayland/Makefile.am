pkglib_LTLIBRARIES = eglplatform_wayland.la

eglplatform_wayland_la_SOURCES = eglplatform_wayland.cpp wayland_window.cpp
eglplatform_wayland_la_CXXFLAGS = \
	-I$(top_srcdir)/include \
	-I$(top_srcdir)/egl \
	-I$(top_srcdir)/egl/platforms/common \
	$(WAYLAND_CLIENT_CFLAGS)

eglplatform_wayland_la_LDFLAGS = \
	-avoid-version -module -shared -export-dynamic \
	$(top_builddir)/egl/platforms/common/libhybris-eglplatformcommon.la \
	$(top_builddir)/hardware/libhardware.la \
	$(WAYLAND_CLIENT_LIBS)

