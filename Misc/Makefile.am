if HAVE_GHC_MMAP
bin_PROGRAMS = abyss-samtobreak
endif

abyss_samtobreak_SOURCES = samtobreak.hs

CLEANFILES=*.hi

GHC_FLAGS=-O2 -Wno-tabs

abyss-samtobreak$(EXEEXT): $(abyss_samtobreak_SOURCES)
	$(GHC) --make $(GHC_FLAGS) -hidir $(dir $@) -odir $(dir $@) -o $@ $^
