CFLAGS += -Wall -ggdb
ifndef DEBUG
CFLAGS += -O2
endif

T = asmproc cmpmrg_text mkbridge translate cvt_data mkdef_ord

all: $(T)

clean:
	$(RM) $(T) *.o

translate: translate.o
mkbridge: mkbridge.o
cvt_data: cvt_data.o
mkdef_ord: mkdef_ord.o
mkbridge.o translate.o cvt_data.o mkdef_ord.o: \
 protoparse.h my_assert.h my_str.h
