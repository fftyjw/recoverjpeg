AUTOMAKE_OPTIONS = foreign

bin_PROGRAMS = recoverjpeg recovermov
dist_bin_SCRIPTS = sort-pictures remove-duplicates

dist_man_MANS = recoverjpeg.1 recovermov.1 sort-pictures.1 remove-duplicates.1

extra_DIST = ChangeLog

always::

ChangeLog: always
	git2cl > ChangeLog

recoverjpeg_SOURCES = recoverjpeg.c utils.c utils.h
recovermov_SOURCES = recovermov.cpp utils.c utils.h

.md.1:
	pandoc -s -w man $< -o $@
