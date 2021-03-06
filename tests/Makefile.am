AM_CPPFLAGS = \
	-I$(top_srcdir)/include \
	-I$(top_srcdir)/common \
	@LIBCERROR_CPPFLAGS@ \
	@LIBCTHREADS_CPPFLAGS@ \
	@LIBCDATA_CPPFLAGS@ \
	@LIBCLOCALE_CPPFLAGS@ \
	@LIBCNOTIFY_CPPFLAGS@ \
	@LIBCSPLIT_CPPFLAGS@ \
	@LIBUNA_CPPFLAGS@ \
	@LIBCFILE_CPPFLAGS@ \
	@LIBCPATH_CPPFLAGS@ \
	@LIBBFIO_CPPFLAGS@ \
	@LIBFDATETIME_CPPFLAGS@ \
	@LIBFGUID_CPPFLAGS@ \
	@LIBFOLE_CPPFLAGS@ \
	@LIBFVALUE_CPPFLAGS@ \
	@LIBFWPS_CPPFLAGS@ \
	@LIBCSYSTEM_CPPFLAGS@ \
	@PTHREAD_CPPFLAGS@ \
	@LIBOLECF_DLL_IMPORT@

if HAVE_PYTHON_TESTS
TESTS_PYOLECF = \
	test_python_functions.sh \
	test_pyolecf_set_ascii_codepage.sh
endif

TESTS = \
	test_api_functions.sh \
	test_api_types.sh \
	test_olecfinfo.sh \
	test_olecfexport.sh \
	$(TESTS_PYOLECF)

check_SCRIPTS = \
	pyolecf_test_get_version.py \
	pyolecf_test_open_close.py \
	pyolecf_test_set_ascii_codepage.py \
	test_api_functions.sh \
	test_api_types.sh \
	test_olecfexport.sh \
	test_olecfinfo.sh \
	test_pyolecf_set_ascii_codepage.sh \
	test_python_functions.sh \
	test_runner.sh

EXTRA_DIST = \
	$(check_SCRIPTS)

check_PROGRAMS = \
	olecf_test_allocation_table \
	olecf_test_directory_entry \
	olecf_test_error \
	olecf_test_file \
	olecf_test_io_handle \
	olecf_test_item \
	olecf_test_notify \
	olecf_test_property_section \
	olecf_test_property_set \
	olecf_test_property_value \
	olecf_test_support

olecf_test_allocation_table_SOURCES = \
	olecf_test_allocation_table.c \
	olecf_test_libcerror.h \
	olecf_test_libolecf.h \
	olecf_test_macros.h \
	olecf_test_memory.c olecf_test_memory.h \
	olecf_test_unused.h

olecf_test_allocation_table_LDADD = \
	../libolecf/libolecf.la \
	@LIBCERROR_LIBADD@

olecf_test_directory_entry_SOURCES = \
	olecf_test_directory_entry.c \
	olecf_test_libcdata.h \
	olecf_test_libcerror.h \
	olecf_test_libolecf.h \
	olecf_test_macros.h \
	olecf_test_memory.c olecf_test_memory.h \
	olecf_test_unused.h

olecf_test_directory_entry_LDADD = \
	../libolecf/libolecf.la \
	@LIBCERROR_LIBADD@

olecf_test_error_SOURCES = \
	olecf_test_error.c \
	olecf_test_libolecf.h \
	olecf_test_macros.h \
	olecf_test_unused.h

olecf_test_error_LDADD = \
	../libolecf/libolecf.la

olecf_test_file_SOURCES = \
	olecf_test_file.c \
	olecf_test_libcerror.h \
	olecf_test_libclocale.h \
	olecf_test_libcsystem.h \
	olecf_test_libolecf.h \
	olecf_test_libuna.h \
	olecf_test_macros.h \
	olecf_test_memory.c olecf_test_memory.h

olecf_test_file_LDADD = \
	@LIBCSYSTEM_LIBADD@ \
	@LIBUNA_LIBADD@ \
	@LIBCNOTIFY_LIBADD@ \
	@LIBCLOCALE_LIBADD@ \
	@LIBCDATA_LIBADD@ \
	../libolecf/libolecf.la \
	@LIBCTHREADS_LIBADD@ \
	@LIBCERROR_LIBADD@ \
	@PTHREAD_LIBADD@

olecf_test_io_handle_SOURCES = \
	olecf_test_io_handle.c \
	olecf_test_libcerror.h \
	olecf_test_libolecf.h \
	olecf_test_macros.h \
	olecf_test_memory.c olecf_test_memory.h \
	olecf_test_unused.h

olecf_test_io_handle_LDADD = \
	../libolecf/libolecf.la \
	@LIBCERROR_LIBADD@

olecf_test_item_SOURCES = \
	olecf_test_item.c \
	olecf_test_libcerror.h \
	olecf_test_libolecf.h \
	olecf_test_macros.h \
	olecf_test_memory.c olecf_test_memory.h \
	olecf_test_unused.h

olecf_test_item_LDADD = \
	../libolecf/libolecf.la \
	@LIBCERROR_LIBADD@

olecf_test_notify_SOURCES = \
	olecf_test_libolecf.h \
	olecf_test_macros.h \
	olecf_test_notify.c \
	olecf_test_unused.h

olecf_test_notify_LDADD = \
	../libolecf/libolecf.la

olecf_test_property_section_SOURCES = \
	olecf_test_libcerror.h \
	olecf_test_libolecf.h \
	olecf_test_macros.h \
	olecf_test_memory.c olecf_test_memory.h \
	olecf_test_property_section.c \
	olecf_test_unused.h

olecf_test_property_section_LDADD = \
	../libolecf/libolecf.la \
	@LIBCERROR_LIBADD@

olecf_test_property_set_SOURCES = \
	olecf_test_libcerror.h \
	olecf_test_libolecf.h \
	olecf_test_macros.h \
	olecf_test_memory.c olecf_test_memory.h \
	olecf_test_property_set.c \
	olecf_test_unused.h

olecf_test_property_set_LDADD = \
	../libolecf/libolecf.la \
	@LIBCERROR_LIBADD@

olecf_test_property_value_SOURCES = \
	olecf_test_libcerror.h \
	olecf_test_libolecf.h \
	olecf_test_macros.h \
	olecf_test_memory.c olecf_test_memory.h \
	olecf_test_property_value.c \
	olecf_test_unused.h

olecf_test_property_value_LDADD = \
	../libolecf/libolecf.la \
	@LIBCERROR_LIBADD@

olecf_test_support_SOURCES = \
	olecf_test_libbfio.h \
	olecf_test_libcerror.h \
	olecf_test_libclocale.h \
	olecf_test_libcsystem.h \
	olecf_test_libolecf.h \
	olecf_test_libuna.h \
	olecf_test_macros.h \
	olecf_test_support.c

olecf_test_support_LDADD = \
	@LIBCSYSTEM_LIBADD@ \
	@LIBBFIO_LIBADD@ \
	@LIBCPATH_LIBADD@ \
	@LIBCFILE_LIBADD@ \
	@LIBUNA_LIBADD@ \
	@LIBCNOTIFY_LIBADD@ \
	@LIBCLOCALE_LIBADD@ \
	@LIBCDATA_LIBADD@ \
	../libolecf/libolecf.la \
	@LIBCERROR_LIBADD@

MAINTAINERCLEANFILES = \
	Makefile.in

distclean: clean
	/bin/rm -f Makefile

