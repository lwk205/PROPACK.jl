include ../Make.inc

DOBJ = zlanbpro.F zreorth.F zgetu0.F zsafescal.F dblasext.F zblasext.F \
       zlansvd.F printstat.F zgemm_ovwr.F dgemm_ovwr.F  \
       zlansvd_irl.F dbsvd.F zritzvec.F z$(MGS).F second.F

all:
	$(FC) -shared $(FFLAG) $(DOBJ) $(LDFLAGS) -o libzpropack.$(SLIB)

debug:
	$(FC) -shared -g $(FFLAG) $(DOBJ) $(LDFLAGS) -o libspropack.$(SLIB)

clean:
	rm *.$(SLIB)