```  
  # make CC=clang LLVM=1 -j 
  mkdir -p /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf
  mkdir -p /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool
  mkdir -p /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include
  mkdir -p /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/bin
  make  -C /sched_ext/sched_ext-sched_ext/tools/lib/bpf OUTPUT=/sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/	\
  	    EXTRA_CFLAGS='-g -O0 -fPIC'					\
  	    DESTDIR=/sched_ext/sched_ext-sched_ext/tools/sched_ext/build prefix= all install_headers
  mkdir -p /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/sched_ext
  make[1]: Entering directory '/sched_ext/sched_ext-sched_ext/tools/lib/bpf'
    GEN     /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/bpf_helper_defs.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/libbpf.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/btf.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/libbpf_common.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/libbpf_legacy.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_tracing.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_endian.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_core_read.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/skel_internal.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/libbpf_version.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/usdt.bpf.h
    HOSTCC  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/fixdep.o
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helper_defs.h
    INSTALL libbpf_headers
    HOSTLD  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/fixdep-in.o
    LINK    /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/fixdep
    GEN     /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/libbpf.pc
    MKDIR   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/
    MKDIR   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/
    MKDIR   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/
    MKDIR   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/libbpf.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/libbpf_errno.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/str_error.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/bpf.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/netlink.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/btf.o
  Warning: Kernel ABI header at 'tools/include/uapi/linux/if_xdp.h' differs from latest version at 'include/uapi/linux/if_xdp.h'
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/bpf_prog_linfo.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/nlattr.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/libbpf_probes.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/hashmap.o
    MKDIR   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/btf_dump.o
    MKDIR   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/
    MKDIR   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/
    MKDIR   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/
    MKDIR   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/
    MKDIR   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/ringbuf.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/strset.o
    MKDIR   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/
    MKDIR   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/linker.o
    MKDIR   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/libbpf.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/gen_loader.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/bpf.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/relo_core.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/nlattr.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/btf.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/libbpf_errno.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/usdt.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/str_error.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/zip.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/netlink.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/bpf_prog_linfo.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/elf.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/libbpf_probes.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/hashmap.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/btf_dump.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/ringbuf.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/strset.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/linker.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/gen_loader.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/relo_core.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/usdt.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/zip.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/elf.o
    LD      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/sharedobjs/libbpf-in.o
    LD      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/staticobjs/libbpf-in.o
    LINK    /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/libbpf.so.1.3.0
  readelf: Warning: Unrecognized form: 0x23
  readelf: Warning: Unrecognized form: 0x23
  readelf: Warning: Unrecognized form: 0x23
  readelf: Warning: Unrecognized form: 0x23
    LINK    /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/libbpf.a
  make[1]: Leaving directory '/sched_ext/sched_ext-sched_ext/tools/lib/bpf'
  make   -C /sched_ext/sched_ext-sched_ext/tools/bpf/bpftool				\
  	    ARCH= CROSS_COMPILE= CC=clang LD=ld.lld		\
  	    EXTRA_CFLAGS='-g -O0'					\
  	    OUTPUT=/sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/				\
  	    LIBBPF_OUTPUT=/sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/libbpf/			\
  	    LIBBPF_DESTDIR=/sched_ext/sched_ext-sched_ext/tools/sched_ext/build/				\
  	    prefix= DESTDIR=/sched_ext/sched_ext-sched_ext/tools/sched_ext/build/ install-bin
  make[1]: Entering directory '/sched_ext/sched_ext-sched_ext/tools/bpf/bpftool'
  
  Auto-detecting system features:
  ...                         clang-bpf-co-re: [ on  ]
  ...                                    llvm: [ OFF ]
  ...                                  libcap: [ on  ]
  ...                                  libbfd: [ on  ]
  
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/hashmap.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/nlattr.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/relo_core.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/libbpf_internal.h
    MKDIR   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/include/bpf
    MKDIR   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/
    MKDIR   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/struct_ops.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/tracelog.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/xlated_dumper.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/disasm.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/btf.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/btf_dumper.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/cfg.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/cgroup.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/common.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/feature.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/gen.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/iter.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/jit_disasm.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/json_writer.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/link.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/main.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/map_perf_ring.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/net.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/map.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/netlink_dumper.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/perf.o
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/include/bpf/hashmap.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/include/bpf/relo_core.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/include/bpf/libbpf_internal.h
  make[2]: Entering directory '/sched_ext/sched_ext-sched_ext/tools/lib/bpf'
    GEN     /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/bpf_helper_defs.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/include/bpf/bpf.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/include/bpf/libbpf.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/include/bpf/btf.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/include/bpf/libbpf_common.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/include/bpf/libbpf_legacy.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/include/bpf/bpf_helpers.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/include/bpf/bpf_tracing.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/include/bpf/bpf_endian.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/include/bpf/bpf_core_read.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/include/bpf/skel_internal.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/include/bpf/libbpf_version.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/include/bpf/usdt.bpf.h
    INSTALL /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/include/bpf/bpf_helper_defs.h
    MKDIR   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/
    INSTALL libbpf_headers
    MKDIR   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/
    MKDIR   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/
    MKDIR   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/libbpf.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/bpf.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/libbpf_errno.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/nlattr.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/btf.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/str_error.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/netlink.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/bpf_prog_linfo.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/libbpf_probes.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/hashmap.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/btf_dump.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/ringbuf.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/strset.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/linker.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/relo_core.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/gen_loader.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/usdt.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/zip.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/elf.o
    LD      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/staticobjs/libbpf-in.o
    LINK    /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/libbpf/libbpf.a
  make[2]: Leaving directory '/sched_ext/sched_ext-sched_ext/tools/lib/bpf'
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/main.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/common.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/json_writer.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/gen.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/btf.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/xlated_dumper.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/btf_dumper.o
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/disasm.o
    LINK    /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bootstrap/bpftool
    GEN     /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/vmlinux.h
    CLANG   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/pid_iter.bpf.o
    CLANG   /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/profiler.bpf.o
    GEN     /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/profiler.skel.h
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/prog.o
    GEN     /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/pid_iter.skel.h
    CC      /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/pids.o
    LINK    /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/bpftool/bpftool
    INSTALL bpftool
  make[1]: Leaving directory '/sched_ext/sched_ext-sched_ext/tools/bpf/bpftool'
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/sbin/bpftool btf dump file /sys/kernel/btf/vmlinux format c > /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/vmlinux.h
  cargo build --manifest-path=scx_rusty/Cargo.toml --release --target-dir /sched_ext/sched_ext-sched_ext/tools/sched_ext/build
  clang -g -D__TARGET_ARCH_x86 -mlittle-endian -I/sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include -I/sched_ext/sched_ext-sched_ext/tools/sched_ext -I/sched_ext/sched_ext-sched_ext/tools/include/uapi -I../../include -idirafter /usr/lib/llvm-18/lib/clang/18/include -idirafter /usr/local/include -idirafter /usr/include/x86_64-linux-gnu -idirafter /usr/include  -Wall -Wno-compare-distinct-pointer-types -O2 -mcpu=v3 -target bpf -c scx_simple.bpf.c -o /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/sched_ext/scx_simple.bpf.o
     Compiling libc v0.2.149
  clang -g -D__TARGET_ARCH_x86 -mlittle-endian -I/sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include -I/sched_ext/sched_ext-sched_ext/tools/sched_ext -I/sched_ext/sched_ext-sched_ext/tools/include/uapi -I../../include -idirafter /usr/lib/llvm-18/lib/clang/18/include -idirafter /usr/local/include -idirafter /usr/include/x86_64-linux-gnu -idirafter /usr/include  -Wall -Wno-compare-distinct-pointer-types -O2 -mcpu=v3 -target bpf -c scx_qmap.bpf.c -o /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/sched_ext/scx_qmap.bpf.o
     Compiling proc-macro2 v1.0.69
     Compiling unicode-ident v1.0.12
     Compiling autocfg v1.1.0
     Compiling cfg-if v1.0.0
     Compiling bitflags v1.3.2
     Compiling syn v1.0.109
     Compiling pin-utils v0.1.0
     Compiling hashbrown v0.14.2
     Compiling thiserror v1.0.50
     Compiling equivalent v1.0.1
     Compiling pkg-config v0.3.27
     Compiling serde v1.0.189
     Compiling toml_datetime v0.6.3
     Compiling winnow v0.5.17
     Compiling once_cell v1.18.0
     Compiling heck v0.4.1
  clang -g -D__TARGET_ARCH_x86 -mlittle-endian -I/sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include -I/sched_ext/sched_ext-sched_ext/tools/sched_ext -I/sched_ext/sched_ext-sched_ext/tools/include/uapi -I../../include -idirafter /usr/lib/llvm-18/lib/clang/18/include -idirafter /usr/local/include -idirafter /usr/include/x86_64-linux-gnu -idirafter /usr/include  -Wall -Wno-compare-distinct-pointer-types -O2 -mcpu=v3 -target bpf -c scx_central.bpf.c -o /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/sched_ext/scx_central.bpf.o
     Compiling rustix v0.38.20
     Compiling rustversion v1.0.14
     Compiling anyhow v1.0.75
     Compiling bitflags v2.4.1
  clang -g -D__TARGET_ARCH_x86 -mlittle-endian -I/sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include -I/sched_ext/sched_ext-sched_ext/tools/sched_ext -I/sched_ext/sched_ext-sched_ext/tools/include/uapi -I../../include -idirafter /usr/lib/llvm-18/lib/clang/18/include -idirafter /usr/local/include -idirafter /usr/include/x86_64-linux-gnu -idirafter /usr/include  -Wall -Wno-compare-distinct-pointer-types -O2 -mcpu=v3 -target bpf -c scx_pair.bpf.c -o /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/sched_ext/scx_pair.bpf.o
     Compiling glob v0.3.1
     Compiling linux-raw-sys v0.4.10
  clang -g -D__TARGET_ARCH_x86 -mlittle-endian -I/sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include -I/sched_ext/sched_ext-sched_ext/tools/sched_ext -I/sched_ext/sched_ext-sched_ext/tools/include/uapi -I../../include -idirafter /usr/lib/llvm-18/lib/clang/18/include -idirafter /usr/local/include -idirafter /usr/include/x86_64-linux-gnu -idirafter /usr/include  -Wall -Wno-compare-distinct-pointer-types -O2 -mcpu=v3 -target bpf -c scx_flatcg.bpf.c -o /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/sched_ext/scx_flatcg.bpf.o
     Compiling regex-syntax v0.8.2
     Compiling memoffset v0.7.1
  clang -g -D__TARGET_ARCH_x86 -mlittle-endian -I/sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include -I/sched_ext/sched_ext-sched_ext/tools/sched_ext -I/sched_ext/sched_ext-sched_ext/tools/include/uapi -I../../include -idirafter /usr/lib/llvm-18/lib/clang/18/include -idirafter /usr/local/include -idirafter /usr/include/x86_64-linux-gnu -idirafter /usr/include  -Wall -Wno-compare-distinct-pointer-types -O2 -mcpu=v3 -target bpf -c scx_userland.bpf.c -o /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/obj/sched_ext/scx_userland.bpf.o
     Compiling serde_json v1.0.107
  In file included from scx_simple.bpf.c:23:21/189: rustversion(build.rs), linux-raw-sys, proc-macro2, bitflags, winnow, thiserror(build), serde(build), libc, rustix(build), hashbrown, serde_json...
  In file included from ./scx_common.bpf.h:14:
  ./user_exit_info.h:25:23: warning: declaration of 'struct scx_exit_info' will not be visible outside of this function [-Wvisibility]
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  ./user_exit_info.h:27:64: error: incomplete definition of type 'struct scx_exit_info'
     27 |         bpf_probe_read_kernel_str(uei->reason, sizeof(uei->reason), ei->reason);
        |                                                                     ~~^
  ./user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  ./user_exit_info.h:28:58: error: incomplete definition of type 'struct scx_exit_info'
     28 |         bpf_probe_read_kernel_str(uei->msg, sizeof(uei->msg), ei->msg);
        |                                                               ~~^
  ./user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  ./user_exit_info.h:30:65: error: incomplete definition of type 'struct scx_exit_info'
     30 |         __sync_val_compare_and_swap(&uei->exit_type, uei->exit_type, ei->type);
        |                                                                      ~~^
  ./user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
     Compiling camino v1.1.6
  In file included from scx_simple.bpf.c:23:22/189: rustversion(build.rs), linux-raw-sys, proc-macro2, bitflags, winnow, thiserror(build), libc, rustix(build), hashbrown, camino(build.rs), serde_...
  ./scx_common.bpf.h:27:17: error: use of undeclared identifier 'SCX_DSQ_FLAG_BUILTIN'
     27 |         _Static_assert(SCX_DSQ_FLAG_BUILTIN,
        |                        ^
     Compiling semver v1.0.20
  In file included from scx_qmap.bpf.c:25:] 24/189: linux-raw-sys, proc-macro2, bitflags, winnow, libc, rustix(build), hashbrown, camino(build.rs), serde_json(build.rs), libc, pkg-config, glob, r...
  In file included from ./scx_common.bpf.h:14:
  ./user_exit_info.h:25:23: warning: declaration of 'struct scx_exit_info' will not be visible outside of this function [-Wvisibility]
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  ./user_exit_info.h:27:64: error: incomplete definition of type 'struct scx_exit_info'
     27 |         bpf_probe_read_kernel_str(uei->reason, sizeof(uei->reason), ei->reason);
        |                                                                     ~~^
  ./user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  ./user_exit_info.h:28:58: error: incomplete definition of type 'struct scx_exit_info'
     28 |         bpf_probe_read_kernel_str(uei->msg, sizeof(uei->msg), ei->msg);
        |                                                               ~~^
  ./user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  ./user_exit_info.h:30:65: error: incomplete definition of type 'struct scx_exit_info'
     30 |         __sync_val_compare_and_swap(&uei->exit_type, uei->exit_type, ei->type);
        |                                                                      ~~^
  ./user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  scx_simple.bpf.c:59:18: error: use of undeclared identifier 'SCX_ENQ_LOCAL'; did you mean 'SGX_ENCL_IOCTL'?
     59 |         if (enq_flags & SCX_ENQ_LOCAL) {
        |                         ^~~~~~~~~~~~~
        |                         SGX_ENCL_IOCTL
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/vmlinux.h:22907 : 2 :  Building note: [==>                       ] 25/189: linux-raw-sys, proc-macro2, bitflags, winnow, libc, hashbrown, camino(build.rs), serde_json(build.rs), libc, pkg-config, glob, rustversion(buil...'SGX_ENCL_IOCTL' declared here
   22907 |         SGX_ENCL_IOCTL = 1,
         |         ^
  In file included from scx_qmap.bpf.c:25:
  ./scx_common.bpf.h:27:17: error: use of undeclared identifier 'SCX_DSQ_FLAG_BUILTIN'
     27 |         _Static_assert(SCX_DSQ_FLAG_BUILTIN,
        |                        ^
  scx_qmap.bpf.c:30:31: error: use of undeclared identifier 'SCX_SLICE_DFL'
     30 | const volatile u64 slice_ns = SCX_SLICE_DFL;
        |                               ^
  scx_qmap.bpf.c:147:29: error: no member named 'scx' in 'struct task_struct'
    147 |         int idx = weight_to_idx(p->scx.weight);
        |                                 ~  ^
  scx_simple.bpf.c:61:23: error: use of undeclared identifier 'SCX_DSQ_LOCAL'
     61 |                 scx_bpf_dispatch(p, SCX_DSQ_LOCAL, SCX_SLICE_DFL, enq_flags);
        |                                     ^
  scx_simple.bpf.c:61:38: error: use of undeclared identifier 'SCX_SLICE_DFL'
     61 |                 scx_bpf_dispatch(p, SCX_DSQ_LOCAL, SCX_SLICE_DFL, enq_flags);
        |                                                    ^
  scx_qmap.bpf.c:178:40: error: use of undeclared identifier 'SCX_ENQ_LAST'
    178 |         if (tctx->force_local || (enq_flags & SCX_ENQ_LAST)) {
        |                                               ^
  scx_qmap.bpf.c:180:23: error: use of undeclared identifier 'SCX_DSQ_LOCAL'o2, bitflags, winnow, rustversion, libc, hashbrown, camino(build.rs), serde_json(build.rs), libc, pkg-config, glob, reg...
    180 |                 scx_bpf_dispatch(p, SCX_DSQ_LOCAL, slice_ns, enq_flags);
        |                                     ^
  scx_simple.bpf.c:68:23: error: use of undeclared identifier 'SCX_DSQ_GLOBAL'
     68 |                 scx_bpf_dispatch(p, SCX_DSQ_GLOBAL, SCX_SLICE_DFL, enq_flags);
        |                                     ^
  scx_simple.bpf.c:68:39: error: use of undeclared identifier 'SCX_SLICE_DFL'
     68 |                 scx_bpf_dispatch(p, SCX_DSQ_GLOBAL, SCX_SLICE_DFL, enq_flags);
        |                                                     ^
  scx_simple.bpf.c:70:18: error: no member named 'scx' in 'struct task_struct'
     70 |                 u64 vtime = p->scx.dsq_vtime;
        |                             ~  ^
  scx_qmap.bpf.c:190:18: error: use of undeclared identifier 'SCX_ENQ_REENQ'
    190 |         if (enq_flags & SCX_ENQ_REENQ) {
        |                         ^
  scx_simple.bpf.c:76:39: error: use of undeclared identifier 'SCX_SLICE_DFL'
     76 |                 if (vtime_before(vtime, vtime_now - SCX_SLICE_DFL))
        |                                                     ^
  scx_qmap.bpf.c:193:23: error: use of undeclared identifier 'SCX_DSQ_GLOBAL'
    193 |                 scx_bpf_dispatch(p, SCX_DSQ_GLOBAL, 0, enq_flags);
        |                                     ^
  scx_qmap.bpf.c:208:23: error: use of undeclared identifier 'SCX_DSQ_GLOBAL'
    208 |                 scx_bpf_dispatch(p, SCX_DSQ_GLOBAL, slice_ns, enq_flags);
        |                                     ^
  scx_simple.bpf.c:77:24: error: use of undeclared identifier 'SCX_SLICE_DFL'
     77 |                         vtime = vtime_now - SCX_SLICE_DFL;
        |                                             ^
  scx_qmap.bpf.c:222:18: error: use of undeclared identifier 'SCX_DEQ_CORE_SCHED_EXEC'
    222 |         if (deq_flags & SCX_DEQ_CORE_SCHED_EXEC)
        |                         ^
  scx_qmap.bpf.c:229:29: error: no member named 'scx' in 'struct task_struct'
    229 |         int idx = weight_to_idx(p->scx.weight);
        |                                 ~  ^
  scx_qmap.bpf.c:256:24: error: use of undeclared identifier 'SCX_DSQ_GLOBAL'
    256 |                         scx_bpf_dispatch(p, SCX_DSQ_GLOBAL, slice_ns, 0);
        |                                             ^
  scx_simple.bpf.c:79:29: error: use of undeclared identifier 'SCX_DSQ_GLOBAL'
     79 |                 scx_bpf_dispatch_vtime(p, SCX_DSQ_GLOBAL, SCX_SLICE_DFL, vtime,
        |                                           ^
  scx_simple.bpf.c:79:45: error: use of undeclared identifier 'SCX_SLICE_DFL'
     79 |                 scx_bpf_dispatch_vtime(p, SCX_DSQ_GLOBAL, SCX_SLICE_DFL, vtime,
        |                                                           ^
  scx_simple.bpf.c:95:33: error: no member named 'scx' in 'struct task_struct'
     95 |         if (vtime_before(vtime_now, p->scx.dsq_vtime))
        |                                     ~  ^
  scx_simple.bpf.c:96:18: error: no member named 'scx' in 'struct task_struct'
     96 |                 vtime_now = p->scx.dsq_vtime;
        |                             ~  ^
  scx_simple.bpf.c:105:5: error: no member named 'scx' in 'struct task_struct'
    105 |         p->scx.dsq_vtime += (SCX_SLICE_DFL - p->scx.slice) * 100 / p->scx.weight;
        |         ~  ^
  scx_qmap.bpf.c:289:25: error: use of undeclared identifier 'SCX_DSQ_GLOBAL'
    289 |                                 scx_bpf_dispatch(p, SCX_DSQ_GLOBAL, slice_ns, 0);
        |                                                     ^
  scx_simple.bpf.c:105:42: error: no member named 'scx' in 'struct task_struct'
    105 |         p->scx.dsq_vtime += (SCX_SLICE_DFL - p->scx.slice) * 100 / p->scx.weight;
        |                                              ~  ^
  scx_simple.bpf.c:105:23: error: use of undeclared identifier 'SCX_SLICE_DFL'
    105 |         p->scx.dsq_vtime += (SCX_SLICE_DFL - p->scx.slice) * 100 / p->scx.weight;
        |                              ^
  fatal error: too many errors emitted, stopping now [-ferror-limit=]
  scx_qmap.bpf.c:305:29: error: no member named 'scx' in 'struct task_struct'
    305 |         int idx = weight_to_idx(p->scx.weight);
        |                                 ~  ^
  scx_qmap.bpf.c:342:55: warning: declaration of 'struct scx_cpu_release_args' will not be visible outside of this function [-Wvisibility]
    342 | void BPF_STRUCT_OPS(qmap_cpu_release, s32 cpu, struct scx_cpu_release_args *args)
        |                                                       ^
  scx_qmap.bpf.c:342:55: warning: declaration of 'struct scx_cpu_release_args' will not be visible outside of this function [-Wvisibility]
  scx_qmap.bpf.c:342:6: error: conflicting types for '____qmap_cpu_release'
    342 | void BPF_STRUCT_OPS(qmap_cpu_release, s32 cpu, struct scx_cpu_release_args *args)
        |      ^
  ./scx_common.bpf.h:77:32: note: expanded from macro 'BPF_STRUCT_OPS'
     77 | SEC("struct_ops/"#name)                                                         \
        |                                                                                 ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_tracing.h:676:48: note: expanded from macro '\
  BPF_PROG'
    676 | static __always_inline typeof(name(0))                                      \
        |                                                                             ^
  <scratch space>:213:1: note: expanded from here
    213 | ____qmap_cpu_release
        | ^
  scx_qmap.bpf.c:342:6: note: previous declaration is here
  ./scx_common.bpf.h:77:32: note: expanded from macro 'BPF_STRUCT_OPS'
     77 | SEC("struct_ops/"#name)                                                         \
        |                                                                                 ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_tracing.h:667:48: note: expanded from macro '\
  BPF_PROG'
    667 | static __always_inline typeof(name(0))                                      \
        |                                                                             ^
  <scratch space>:204:1: note: expanded from here
    204 | ____qmap_cpu_release
        | ^
  scx_qmap.bpf.c:359:13: warning: declaration of 'struct scx_enable_args' will not be visible outside of this function [-Wvisibility]
    359 |                    struct scx_enable_args *args)
        |                           ^
  scx_qmap.bpf.c:359:13: warning: declaration of 'struct scx_enable_args' will not be visible outside of this function [-Wvisibility]
  scx_qmap.bpf.c:358:5: error: conflicting types for '____qmap_prep_enable'
    358 | s32 BPF_STRUCT_OPS(qmap_prep_enable, struct task_struct *p,
        |     ^
  ./scx_common.bpf.h:77:32: note: expanded from macro 'BPF_STRUCT_OPS'
     77 | SEC("struct_ops/"#name)                                                         \
        |                                                                                 ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_tracing.h:676:48: note: expanded from macro '\
  BPF_PROG'
    676 | static __always_inline typeof(name(0))                                      \
        |                                                                             ^
  <scratch space>:230:1: note: expanded from here
    230 | ____qmap_prep_enable
        | ^
  scx_qmap.bpf.c:358:5: note: previous declaration is here
  ./scx_common.bpf.h:77:32: note: expanded from macro 'BPF_STRUCT_OPS'
     77 | SEC("struct_ops/"#name)                                                         \
        |                                                                                 ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_tracing.h:667:48: note: expanded from macro '\
  BPF_PROG'
    667 | static __always_inline typeof(name(0))                                      \
        |                                                                             ^
  <scratch space>:221:1: note: expanded from here
    221 | ____qmap_prep_enable
        | ^
  scx_qmap.bpf.c:362:6: error: no member named 'scx' in 'struct task_struct'
    362 |                 p->scx.disallow = true;
        |                 ~  ^
  scx_qmap.bpf.c:382:39: warning: declaration of 'struct scx_exit_info' will not be visible outside of this function [-Wvisibility]
    382 | void BPF_STRUCT_OPS(qmap_exit, struct scx_exit_info *ei)
        |                                       ^
  scx_qmap.bpf.c:382:39: warning: declaration of 'struct scx_exit_info' will not be visible outside of this function [-Wvisibility]
  fatal error: too many errors emitted, stopping now [-ferror-limit=]
  7 warnings and 20 errors generated.
  1 warning and 20 errors generated.
  make: *** [Makefile:169: scx_qmap.bpf.o] Error 1
  make: *** Waiting for unfinished jobs....
  make: *** [Makefile:169: scx_simple.bpf.o] Error 1
  In file included from scx_central.bpf.c:48:
  In file included from ./scx_common.bpf.h:14:
  ./user_exit_info.h:25:23: warning: declaration of 'struct scx_exit_info' will not be visible outside of this function [-Wvisibility]
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  ./user_exit_info.h:27:64: error: incomplete definition of type 'struct scx_exit_info'
     27 |         bpf_probe_read_kernel_str(uei->reason, sizeof(uei->reason), ei->reason);
        |                                                                     ~~^
  ./user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  ./user_exit_info.h:28:58: error: incomplete definition of type 'struct scx_exit_info'
     28 |         bpf_probe_read_kernel_str(uei->msg, sizeof(uei->msg), ei->msg);
        |                                                               ~~^
  ./user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  ./user_exit_info.h:30:65: error: incomplete definition of type 'struct scx_exit_info'
     30 |         __sync_val_compare_and_swap(&uei->exit_type, uei->exit_type, ei->type);
        |                                                                      ~~^
  ./user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
     Compiling indexmap v2.0.2
     Compiling lazy_static v1.4.0
  In file included from scx_central.bpf.c:48:9/189: linux-raw-sys, proc-macro2, bitflags, winnow, rustversion, indexmap, libc, hashbrown, camino(build.rs), serde_json(build.rs), libc, memoffset(b...
  ./scx_common.bpf.h:27:17: error: use of undeclared identifier 'SCX_DSQ_FLAG_BUILTIN'
     27 |         _Static_assert(SCX_DSQ_FLAG_BUILTIN,
        |                        ^
     Compiling clap_lex v0.5.1
  scx_central.bpf.c:61:31: error: use of undeclared identifier 'SCX_SLICE_DFL'roc-macro2, bitflags, winnow, rustversion, indexmap, libc, camino(build.rs), serde_json(build.rs), libc, memoffset(bu...
     61 | const volatile u64 slice_ns = SCX_SLICE_DFL;
        |                               ^
     Compiling minimal-lexical v0.2.1
     Compiling version_check v0.9.4
     Compiling clang-sys v1.6.1
  scx_central.bpf.c:121:23: error: use of undeclared identifier 'SCX_DSQ_LOCAL'oc-macro2, version_check, winnow, rustversion, indexmap, libc, camino(build.rs), serde_json(build.rs), libc, memoffs...
    121 |                 scx_bpf_dispatch(p, SCX_DSQ_LOCAL, SCX_SLICE_INF,
        |                                     ^
  scx_central.bpf.c:121:38: error: use of undeclared identifier 'SCX_SLICE_INF'
    121 |                 scx_bpf_dispatch(p, SCX_DSQ_LOCAL, SCX_SLICE_INF,
        |                                                    ^
  scx_central.bpf.c:122:18: error: use of undeclared identifier 'SCX_ENQ_PREEMPT'
    122 |                                  enq_flags | SCX_ENQ_PREEMPT);
        |                                              ^
  scx_central.bpf.c:128:40: error: use of undeclared identifier 'SCX_SLICE_INF'oc-macro2, version_check, winnow, rustversion, indexmap, libc, camino(build.rs), libc, memoffset(build), regex-synta...
    128 |                 scx_bpf   Compiling itoa v1.0.9
  _dispatch(p, FA    Building [===>                      ] 35/189: clap_lex, linux-raw-sys, proc-macro2, version_check, winnow, rustversion, itoa, indexmap, libc, camino(build.rs), libc, memoffset(buiLLBACK_DSQ_ID, SCX_SLICE_INF, enq_flags);
        |                                                      ^
  scx_central.bpf.c:135:33: error: use of undeclared identifier 'SCX_KICK_PREEMPT'macro2, version_check, winnow, rustversion, itoa, memoffset, indexmap, libc, camino(build.rs), libc, regex-syntax...
    135 |                 scx_bpf_kick_cpu(central_cpu, SCX_KICK_PREEMPT);
        |                                               ^
  scx_central.bpf.c:143:2: error: variable has incomplete type 'struct bpf_iter_num'
    143 |         bpf_repeat(BPF_MAX_LOOPS) {
        |         ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:390:22: note: expanded from macro 'bpf_repeat'
    390 |         struct bpf_iter_num ___it __attribute__((aligned(8), /* enforce, just in case */        \
        |                             ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:300:8: note: forward declaration of 'struct bpf_iter_num'
    300 | struct bpf_iter_num;
        |        ^
  scx_central.bpf.c:143:13: error: use of undeclared identifier 'BPF_MAX_LOOPS'
    143 |         bpf_repeat(BPF_MAX_LOOPS) {
        |                    ^
  scx_central.bpf.c:161:41: error: use of undeclared identifier 'SCX_SLICE_INF'
    161 |                         scx_bpf_dispatch(p, FALLBACK_DSQ_ID, SCX_SLICE_INF, 0);
        |                                                              ^
  In file included from scx_pair.bpf.c:118:
  In file included from ./scx_common.bpf.h:14:
  ./user_exit_info.h:25:23: warning: declaration of 'struct scx_exit_info' will not be visible outside of this function [-Wvisibility]
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  ./user_exit_info.h:27:64: error: incomplete definition of type 'struct scx_exit_info'
     27 |         bpf_probe_read_kernel_str(uei->reason, sizeof(uei->reason), ei->reason);
        |                                                                     ~~^
  ./user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  ./user_exit_info.h:28:58: error: incomplete definition of type 'struct scx_exit_info'
     28 |         bpf_probe_read_kernel_str(uei->msg, sizeof(uei->msg), ei->msg);
        |                                                               ~~^
  ./user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  ./user_exit_info.h:30:65: error: incomplete definition of type 'struct scx_exit_info'
     30 |         __sync_val_compare_and_swap(&uei->exit_type, uei->exit_type, ei->type);
        |                                                                      ~~^
  ./user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  scx_central.bpf.c:167:23: error: use of undeclared identifier 'SCX_DSQ_LOCAL_ON'
    167 |                 scx_bpf_dispatch(p, SCX_DSQ_LOCAL_ON | cpu, SCX_SLICE_INF, 0);
        |                                     ^
  scx_central.bpf.c:167:47: error: use of undeclared identifier 'SCX_SLICE_INF'
    167 |                 scx_bpf_dispatch(p, SCX_DSQ_LOCAL_ON | cpu, SCX_SLICE_INF, 0);
        |                                                             ^
  scx_central.bpf.c:185:3: error: variable has incomplete type 'struct bpf_iter_num'
    185 |                 bpf_for(cpu, 0, nr_cpu_ids) {
        |                 ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:365:22: note: expanded from macro 'bpf_for'
    365 |         struct bpf_iter_num ___it __attribute__((aligned(8), /* enforce, just in case */        \
        |                             ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:300:8: note: forward declaration of 'struct bpf_iter_num'
    300 | struct bpf_iter_num;
        |        ^
  In file included from scx_pair.bpf.c:118:
  ./scx_common.bpf.h:27:17: error: use of undeclared identifier 'SCX_DSQ_FLAG_BUILTIN'
     27 |         _Static_assert(SCX_DSQ_FLAG_BUILTIN,
        |                        ^
  scx_central.bpf.c:209:34: error: use of undeclared identifier 'SCX_KICK_PREEMPT'
    209 |                         scx_bpf_kick_cpu(central_cpu, SCX_KICK_PREEMPT);
        |                                                       ^
  scx_pair.bpf.c:129:40: error: use of undeclared identifier 'SCX_SLICE_DFL'
    129 | const volatile u32 pair_batch_dur_ns = SCX_SLICE_DFL;
        |                                        ^
     Compiling quote v1.0.33
  scx_pair.bpf.c:385:3: error: variable has incomplete type 'struct bpf_iter_num'-macro2, version_check, winnow, rustversion, itoa, indexmap, libc, quote, camino(build.rs), libc, regex-syntax, se...
    385 |                 bpf_repeat(BPF_MAX_LOOPS) {
        |                 ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:390:22: note: expanded from macro 'bpf_repeat'
    390 |         struct bpf_iter_num ___it __attribute__((aligned(8), /* enforce, just in case */        \
        |                             ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:300:8: note: forward declaration of 'struct bpf_iter_num'
    300 | struct bpf_iter_num;
        |        ^
  scx_pair.bpf.c:385:14: error: use of undeclared identifier 'BPF_MAX_LOOPS'
    385 |                 bpf_repeat(BPF_MAX_LOOPS) {
        |                            ^
  scx_pair.bpf.c:446:2: error: variable has incomplete type 'struct bpf_iter_num'
    446 |         bpf_repeat(BPF_MAX_LOOPS) {
        |         ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:390:22: note: expanded from macro 'bpf_repeat'
    390 |         struct bpf_iter_num ___it __attribute__((aligned(8), /* enforce, just in case */        \
        |                             ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:300:8: note: forward declaration of 'struct bpf_iter_num'
    300 | struct bpf_iter_num;
        |        ^
  In file included from scx_flatcg.bpf.c:46:
  In file included from ./scx_common.bpf.h:14:
  ./user_exit_info.h:25:23: warning: declaration of 'struct scx_exit_info' will not be visible outside of this function [-Wvisibility]
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  scx_central.bpf.c:231:33: error: use of undeclared identifier 'SCX_KICK_PREEMPT'
    231 |                 scx_bpf_kick_cpu(central_cpu, SCX_KICK_PREEMPT);
        |                                               ^
  scx_pair.bpf.c:446:13: error: use of undeclared identifier 'BPF_MAX_LOOPS'
    446 |         bpf_repeat(BPF_MAX_LOOPS) {
        |                    ^
  ./user_exit_info.h:27:64: error: incomplete definition of type 'struct scx_exit_info'
     27 |         bpf_probe_read_kernel_str(uei->reason, sizeof(uei->reason), ei->reason);
        |                                                                     ~~^
  ./user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  ./user_exit_info.h:28:58: error: incomplete definition of type 'struct scx_exit_info'
     28 |         bpf_probe_read_kernel_str(uei->msg, sizeof(uei->msg), ei->msg);
        |                                                               ~~^
  ./user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  ./user_exit_info.h:30:65: error: incomplete definition of type 'struct scx_exit_info'
     30 |         __sync_val_compare_and_swap(&uei->exit_type, uei->exit_type, ei->type);
        |                                                                      ~~^
  ./user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  scx_central.bpf.c:264:2: error: variable has incomplete type 'struct bpf_iter_num'
    264 |         bpf_for(i, 0, nr_cpu_ids) {
        |         ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:365:22: note: expanded from macro 'bpf_for'
    365 |         struct bpf_iter_num ___it __attribute__((aligned(8), /* enforce, just in case */        \
        |                             ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:300:8: note: forward declaration of 'struct bpf_iter_num'
    300 | struct bpf_iter_num;
        |        ^
  fatal error: too many errors emitted, stopping now [-ferror-limit=]
  scx_pair.bpf.c:482:23: error: use of undeclared identifier 'SCX_DSQ_GLOBAL'
    482 |                 scx_bpf_dispatch(p, SCX_DSQ_GLOBAL, SCX_SLICE_DFL, 0);
        |                                     ^
  scx_pair.bpf.c:482:39: error: use of undeclared identifier 'SCX_SLICE_DFL'
    482 |                 scx_bpf_dispatch(p, SCX_DSQ_GLOBAL, SCX_SLICE_DFL, 0);
        |                                                     ^
  In file included from scx_flatcg.bpf.c:46:
  ./scx_common.bpf.h:27:17: error: use of undeclared identifier 'SCX_DSQ_FLAG_BUILTIN'
     27 |         _Static_assert(SCX_DSQ_FLAG_BUILTIN,
        |                        ^
  1 warning and 20 errors generated.
  scx_pair.bpf.c:495:28: error: use of undeclared identifier 'SCX_KICK_PREEMPT'
    495 |                         scx_bpf_kick_cpu(*pair, SCX_KICK_PREEMPT);
        |                                                 ^
  scx_pair.bpf.c:503:2: error: variable has incomplete type 'struct bpf_iter_num'
    503 |         bpf_repeat(BPF_MAX_LOOPS) {
        |         ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:390:22: note: expanded from macro 'bpf_repeat'
    390 |         struct bpf_iter_num ___it __attribute__((aligned(8), /* enforce, just in case */        \
        |                             ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:300:8: note: forward declaration of 'struct bpf_iter_num'
    300 | struct bpf_iter_num;
        |        ^
  scx_flatcg.bpf.c:53:36: error: use of undeclared identifier 'SCX_SLICE_DFL'proc-macro2, version_check, winnow, rustversion, itoa, rustix, indexmap, libc, quote, camino(build.rs), libc, regex-sy...
     53 | const volatile u64 cgrp_slice_ns = SCX_SLICE_DFL;
        |                                    ^
  make: *** [Makefile:169: scx_central.bpf.o] Error 1
  scx_flatcg.bpf.c:206:2: error: variable has incomplete type 'struct bpf_iter_num'
    206 |         bpf_foscx_pair.bpf.cr:503:13: error: use of undeclared identifier 'BPF_MAX_LOOPS'
  (le  vel, 0, cgrp->level + 1) {
        503|  |         ^
          bpf/sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:365:22: note: expanded from macro 'bpf_for'
    365 |         str_repeatu(ct bBPF_pf_iter_num ___it __attribute__((aMligned(8), /* enforce, just in case */        \
        |                             ^
  AX_LOO/sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:300:8: PSnote: forward declaration of 'struct bpf_iter_num'
  )  300 | struct bpf_iter_num;
        |        ^
   {
        |                    ^
  scx_pair.bpf.c:509:55: warning: declaration of 'struct scx_cpu_acquire_args' will not be visible outside of this function [-Wvisibility]
    509 | void BPF_STRUCT_OPS(pair_cpu_acquire, s32 cpu, struct scx_cpu_acquire_args *args)
        |                                                       ^
  scx_pair.bpf.c:509:55: warning: declaration of 'struct scx_cpu_acquire_args' will not be visible outside of this function [-Wvisibility]
  scx_pair.bpf.c:509:6: error: conflicting types for '____pair_cpu_acquire'
    509 | void BPF_STRUCT_OPS(pair_cpu_acquire, s32 cpu, struct scx_cpu_acquire_args *args)
        |      ^
  ./scx_common.bpf.h:77:32: note: expanded from macro 'BPF_STRUCT_OPS'
     77 | SEC("struct_ops/"#name)                                                         \
        |                                                                                 ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_tracing.h:676:48: note: expanded from macro '\
  BPF_PROG'
    676 | static __always_inline typeof(name(0))                                      \
        |                                                                             ^
  <scratch space>:169:1: note: expanded from here
    169 | ____pair_cpu_acquire
        | ^
  scx_pair.bpf.c:509:6: note: previous declaration is here
  ./scx_common.bpf.h:77:32: note: expanded from macro 'BPF_STRUCT_OPS'
     77 | SEC("struct_ops/"#name)                                                         \
        |                                                                                 ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_tracing.h:667:48: note: expanded from macro '\
  BPF_PROG'
    667 | static __always_inline typeof(name(0))                                      \
        |                                                                             ^
  <scratch space>:160:1: note: expanded from here
    160 | ____pair_cpu_acquire
        | ^
  scx_flatcg.bpf.c:325:19: error: use of undeclared identifier 'SCX_ENQ_LOCAL'; did you mean 'SGX_ENCL_IOCTL'?
    325 |         if ((enq_flags & SCX_ENQ_LOCAL) || p->nr_cpus_allowed != nr_cpus) {
        |                          ^~~~~~~~~~~~~
        |                          SGX_ENCL_IOCTL
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/vmlinux.h:22907:2: note: 'SGX_ENCL_IOCTL' declared here
   22907 |         SGX_ENCL_IOCTL = 1,
         |         ^
  scx_pair.bpf.c:531:28: error: use of undeclared identifier 'SCX_KICK_PREEMPT'ion_check, winnow, rustversion, itoa, rustix, semver(build), indexmap, libc, quote, camino(build.rs), libc, regex-sy...
    531 |                         scx_bpf_kick_cpu(*pair, SCX_KICK_PREEMPT);
        |                                                 ^
  scx_pair.bpf.c:536:55: warning: declaration of 'struct scx_cpu_release_args' will not be visible outside of this function [-Wvisibility]
    536 | void BPF_STRUCT_OPS(pair_cpu_release, s32 cpu, struct scx_cpu_release_args *args)
        |                                                       ^
  scx_flatcg.bpf.c:342:20: error: use of undeclared identifier 'SCX_ENQ_LOCAL'; did you mean 'SGX_ENCL_IOCTL'?
    342 |                 if ((enq_flags & SCX_ENQ_LOCAL) ||
        |                                  ^~~~~~~~~~~~~
        |                                  SGX_ENCL_IOCTL
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/vmlinux.h:22907:2: note: 'SGX_ENCL_IOCTL' declared here
   22907 |         SGX_ENCL_IOCTL = 1,
         |         ^
  scx_pair.bpf.c:536:55: warning: declaration of 'struct scx_cpu_release_args' will not be visible outside of this function [-Wvisibility]
  scx_pair.bpf.c:536:6: error: conflicting types for '____pair_cpu_release'
    536 | void BPF_STRUCT_OPS(pair_cpu_release, s32 cpu, struct scx_cpu_release_args *args)
        |      ^
  ./scx_common.bpf.h:77:32: note: expanded from macro 'BPF_STRUCT_OPS'
     77 | SEC("struct_ops/"#name)                                                         \
        |                                                                                 ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_tracing.h:676:48: note: expanded from macro '\
  BPF_PROG'
    676 | static __always_inline typeof(name(0))                                      \
        |                                                                             ^
  <scratch space>:186:1: note: expanded from here
    186 | ____pair_cpu_release
        | ^
  scx_pair.bpf.c:536:6: note: previous declaration is here
  ./scx_common.bpf.h:77:32: note: expanded from macro 'BPF_STRUCT_OPS'
     77 | SEC("struct_ops/"#name)                                                         \
        |                                                                                 ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_tracing.h:667:48: note: expanded from macro '\
  BPF_PROG'
    667 | static __always_inline typeof(name(0))                                      \
        |                                                                             ^
  <scratch space>:177:1: note: expanded from here
    177 | ____pair_cpu_release
        | ^
     Compiling anstyle v1.0.4
     Compiling ryu v1.0.15
  scx_flatcg.bpf.c:345:24: error: use of undeclared identifier 'SCX_DSQ_LOCAL'ro2, version_check, winnow, rustversion, rustix, indexmap, libc, quote, camino(build.rs), libc, anstyle, regex-syntax...
    345 |                         scx_bpf_dispatch(p, SCX_DSQ_LOCAL, SCX_SLICE_DFL, enq_flags);
        |                                             ^
  scx_flatcg.bpf.c:345:39: error: use of undeclared identifier 'SCX_SLICE_DFL'
    345 |                         scx_bpf_dispatch(p, SCX_DSQ_LOCAL, SCX_SLICE_DFL, enq_flags);
        |                                                            ^
  scx_pair.bpf.c:560:28: error: use of undeclared identifier 'SCX_KICK_PREEMPT'
    560 |                         scx_bpf_kick_cpu(*pair, SCX_KICK_PREEMPT | SCX_KICK_WAIT);
        |                                                 ^
  scx_pair.bpf.c:560:47: error: use of undeclared identifier 'SCX_KICK_WAIT'
    560 |                         scx_bpf_kick_cpu(*pair, SCX_KICK_PREEMPT | SCX_KICK_WAIT);
        |                                                                    ^
  fatal error: too many errors emitted, stopping now [-ferror-limit=]
  5 warnings and 20 errors generated.
  make: *** [Makefile:169: scx_pair.bpf.o] Error 1
  scx_flatcg.bpf.c:348:24: error: use of undeclared identifier 'SCX_DSQ_GLOBAL'
    348 |                         scx_bpf_dispatch(p, SCX_DSQ_GLOBAL, SCX_SLICE_DFL, enq_flags);
        |                                             ^
  scx_flatcg.bpf.c:348:40: error: use of undeclared identifier 'SCX_SLICE_DFL'
    348 |                         scx_bpf_dispatch(p, SCX_DSQ_GLOBAL, SCX_SLICE_DFL, enq_flags);
        |                                                             ^
  scx_flatcg.bpf.c:359:37: error: use of undeclared identifier 'SCX_SLICE_DFL'ro2, version_check, winnow, rustversion, rustix, camino(build), indexmap, libc, quote, libc, anstyle, regex-syntax, r...
    359 |                 scx_bpf_dispatch(p, cgrp->kn->id, SCX_SLICE_DFL, enq_flags);
        |                                                   ^
  scx_flatcg.bpf.c:361:19: error: no member named 'scx' in 'struct task_struct'
    361 |                 u64 tvtime = p->scx.dsq_vtime;
        |                              ~  ^
  scx_flatcg.bpf.c:367:46: error: use of undeclared identifier 'SCX_SLICE_DFL'
    367 |                 if (vtime_before(tvtime, cgc->tvtime_now - SCX_SLICE_DFL))
        |                                                            ^
  scx_flatcg.bpf.c:368:31: error: use of undeclared identifier 'SCX_SLICE_DFL'
    368 |                         tvtime = cgc->tvtime_now - SCX_SLICE_DFL;
        |                                                    ^
     Compiling syn v2.0.38
  scx_flatcg.bpf.c:370:43: error: use of undeclared identifier 'SCX_SLICE_DFL'ro2, version_check, winnow, rustversion, syn, rustix, indexmap, libc, quote, libc, anstyle, regex-syntax, ryu, syn, c...
    370 |                 scx_bpf_dispatch_vtime(p, cgrp->kn->id, SCX_SLICE_DFL,
        |                                                         ^
  scx_flatcg.bpf.c:422:2: error: variable has incomplete type 'struct bpf_iter_num'
    422 |         bpf_for(idx, 0, cgrp->level) {
        |         ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:365:22: note: expanded from macro 'bpf_for'
    365 |         struct bpf_iter_num ___it __attribute__((aligned(8), /* enforce, just in case */        \
        |                             ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:300:8: note: forward declaration of 'struct bpf_iter_num'
    300 | struct bpf_iter_num;
        |        ^
  scx_flatcg.bpf.c:501:40: error: no member named 'scx' in 'struct task_struct'
    501 |                 if (vtime_before(cgc->tvtime_now, p->scx.dsq_vtime))
        |                                                   ~  ^
  fatal error: too many errors emitted, stopping now [-ferror-limit=]
  In file included from scx_userland.bpf.c:24:
  In file included from ./scx_common.bpf.h:14:
  ./user_exit_info.h:25:23: warning: declaration of 'struct scx_exit_info' will not be visible outside of this function [-Wvisibility]
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  ./user_exit_info.h:27:64: error: incomplete definition of type 'struct scx_exit_info'
     27 |         bpf_probe_read_kernel_str(uei->reason, sizeof(uei->reason), ei->reason);
        |                                                                     ~~^
  ./user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  ./user_exit_info.h:28:58: error: incomplete definition of type 'struct scx_exit_info'
     28 |         bpf_probe_read_kernel_str(uei->msg, sizeof(uei->msg), ei->msg);
        |                                                               ~~^
  ./user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  ./user_exit_info.h:30:65: error: incomplete definition of type 'struct scx_exit_info'
     30 |         __sync_val_compare_and_swap(&uei->exit_type, uei->exit_type, ei->type);
        |                                                                      ~~^
  ./user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
     25 |                               const struct scx_exit_info *ei)
        |                                            ^
  1 warning and 20 errors generated.
  make: *** [Makefile:169: scx_flatcg.bpf.o] Error 1
  In file included from scx_userland.bpf.c:24:
  ./scx_common.bpf.h:27:17: error: use of undeclared identifier 'SCX_DSQ_FLAG_BUILTIN'
     27 |         _Static_assert(SCX_DSQ_FLAG_BUILTIN,
        |                        ^
     Compiling memchr v2.6.4
  scx_userland.bpf.c:142:23: error: use of undeclared identifier 'SCX_DSQ_GLOBAL', version_check, winnow, rustversion, syn, rustix, indexmap, libc, quote, libc, anstyle, regex-syntax, syn, memchr...
    142 |                 scx_bpf_dispatch(p, SCX_DSQ_GLOBAL, SCX_SLICE_DFL, 0);
        |                                     ^
  scx_userland.bpf.c:142:39: error: use of undeclared identifier 'SCX_SLICE_DFL'
    142 |                 scx_bpf_dispatch(p, SCX_DSQ_GLOBAL, SCX_SLICE_DFL, 0);
        |                                                     ^
  scx_userland.bpf.c:154:19: error: no member named 'scx' in 'struct task_struct'
    154 |         task.weight = p->scx.weight;
        |                       ~  ^
     Compiling clap_builder v4.4.6
     Compiling unicase v2.7.0
  scx_userland.bpf.c:162:23: error: use of undeclared identifier 'SCX_DSQ_GLOBAL', winnow, rustversion, syn, rustix, clap_builder, indexmap, libc, quote, libc, unicase(build.rs), regex-syntax, sy...
    162 |                 scx_bpf_dispatch(p, SCX_DSQ_GLOBAL, SCX_SLICE_DFL, enq_flags);
        |                                     ^
  scx_userland.bpf.c:162:39: error: use of undeclared identifier 'SCX_SLICE_DFL'
    162 |                 scx_bpf_dispatch(p, SCX_DSQ_GLOBAL, SCX_SLICE_DFL, enq_flags);
        |                                                     ^
  scx_userland.bpf.c:172:16: error: use of undeclared identifier 'SCX_DSQ_GLOBAL'
    172 |                 u64 dsq_id = SCX_DSQ_GLOBAL;
        |                              ^
  scx_userland.bpf.c:182:13: error: use of undeclared identifier 'SCX_DSQ_LOCAL'2, winnow, rustversion, syn, rustix, clap_builder, indexmap, libc, quote, libc, unicase(build.rs), regex-syntax, cl...
    182 |                         dsq_id = SCX_DSQ_LOCAL;
        |                                  ^
     Compiling memoffset v0.6.5
     Compiling libloading v0.7.4
  scx_userland.bpf.c:184:31: error: use of undeclared identifier 'SCX_SLICE_DFL'build.rs), winnow, rustversion, syn, rustix, clap_builder, libloading, indexmap, libc, anyhow(build), libc, unicase...
    184 |                 scx_bpf_dispatch(p, dsq_id, SCX_SLICE_DFL, enq_flags);
        |                                             ^
  scx_userland.bpf.c:197:2: error: variable has incomplete type 'struct bpf_iter_num'
    197 |         bpf_repeat(4096) {
        |         ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:390:22: note: expanded from macro 'bpf_repeat'
    390 |         struct bpf_iter_num ___it __attribute__((aligned(8), /* enforce, just in case */        \
        |                             ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:300:8: note: forward declaration of 'struct bpf_iter_num'
    300 | struct bpf_iter_num;
        |        ^
  scx_userland.bpf.c:213:23: error: use of undeclared identifier 'SCX_DSQ_GLOBAL'
    213 |                 scx_bpf_dispatch(p, SCX_DSQ_GLOBAL, SCX_SLICE_DFL, 0);
        |                                     ^
  scx_userland.bpf.c:213:39: error: use of undeclared identifier 'SCX_SLICE_DFL'
    213 |                 scx_bpf_dispatch(p, SCX_DSQ_GLOBAL, SCX_SLICE_DFL, 0);
        |                                                     ^
  scx_userland.bpf.c:219:13: warning: declaration of 'struct scx_enable_args' will not be visible outside of this function [-Wvisibility]
    219 |                    struct scx_enable_args *args)
        |                           ^
  scx_userland.bpf.c:219:13: warning: declaration of 'struct scx_enable_args' will not be visible outside of this function [-Wvisibility]
  scx_userland.bpf.c:218:5: error: conflicting types for '____userland_prep_enable'
    218 | s32 BPF_STRUCT_OPS(userland_prep_enable, struct task_struct *p,
        |     ^
  ./scx_common.bpf.h:77:32: note: expanded from macro 'BPF_STRUCT_OPS'
     77 | SEC("struct_ops/"#name)                                                         \
        |                                                                                 ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_tracing.h:676:48: note: expanded from macro '\
  BPF_PROG'
    676 | static __always_inline typeof(name(0))                                      \
        |                                                                             ^
  <scratch space>:147:1: note: expanded from here
    147 | ____userland_prep_enable
        | ^
  scx_userland.bpf.c:218:5: note: previous declaration is here
  ./scx_common.bpf.h:77:32: note: expanded from macro 'BPF_STRUCT_OPS'
     77 | SEC("struct_ops/"#name)                                                         \
        |                                                                                 ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_tracing.h:667:48: note: expanded from macro '\
  BPF_PROG'
    667 | static __always_inline typeof(name(0))                                      \
        |                                                                             ^
  <scratch space>:138:1: note: expanded from here
    138 | ____userland_prep_enable
        | ^
  scx_userland.bpf.c:247:43: warning: declaration of 'struct scx_exit_info' will not be visible outside of this function [-Wvisibility]
    247 | void BPF_STRUCT_OPS(userland_exit, struct scx_exit_info *ei)
        |                                           ^
  scx_userland.bpf.c:247:43: warning: declaration of 'struct scx_exit_info' will not be visible outside of this function [-Wvisibility]
  scx_userland.bpf.c:247:6: error: conflicting types for '____userland_exit'
    247 | void BPF_STRUCT_OPS(userland_exit, struct scx_exit_info *ei)
        |      ^
  ./scx_common.bpf.h:77:32: note: expanded from macro 'BPF_STRUCT_OPS'
     77 | SEC("struct_ops/"#name)                                                         \
        |                                                                                 ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_tracing.h:676:48: note: expanded from macro '\
  BPF_PROG'
    676 | static __always_inline typeof(name(0))                                      \
        |                                                                             ^
  <scratch space>:195:1: note: expanded from here
    195 | ____userland_exit
        | ^
  scx_userland.bpf.c:247:6: note: previous declaration is here
  ./scx_common.bpf.h:77:32: note: expanded from macro 'BPF_STRUCT_OPS'
     77 | SEC("struct_ops/"#name)                                                         \
        |                                                                                 ^
  /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_tracing.h:667:48: note: expanded from macro '\
  BPF_PROG'
    667 | static __always_inline typeof(name(0))                                      \
        |                                                                             ^
  <scratch space>:186:1: note: expanded from here
    186 | ____userland_exit
        | ^
  scx_userland.bpf.c:249:19: warning: incompatible pointer types passing 'struct scx_exit_info *' to parameter of type 'const struct scx_exit_info *' [-Wincompatible-pointer-types]
    249 |         uei_record(&uei, ei);
        |                          ^~
  ./user_exit_info.h:25:38: note: passing argument to parameter 'ei' here
     25 |                               const struct scx_exit_info *ei)
        |                                                           ^
  scx_userland.bpf.c:253:22: error: variable has incomplete type 'struct sched_ext_ops'
    253 | struct sched_ext_ops userland_ops = {
        |                      ^
  scx_userland.bpf.c:253:8: note: forward declaration of 'struct sched_ext_ops'
    253 | struct sched_ext_ops userland_ops = {
        |        ^
  6 warnings and 18 errors generated.
  make: *** [Makefile:169: scx_userland.bpf.o] Error 1
     Compiling either v1.9.0
     Compiling utf8parse v0.2.1
     Compiling fastrand v2.0.1
     Compiling home v0.5.5
     Compiling nom v7.1.3
     Compiling bindgen v0.61.0
     Compiling toml_edit v0.19.15
     Compiling cc v1.0.83
     Compiling nix v0.26.4
     Compiling num_cpus v1.16.0
     Compiling memmap2 v0.5.10
     Compiling anstyle-parse v0.2.2
     Compiling regex-automata v0.4.3
     Compiling num-traits v0.2.17
     Compiling powerfmt v0.2.0
     Compiling shlex v1.2.0
     Compiling colorchoice v1.0.0
     Compiling lazycell v1.3.0
     Compiling which v4.4.2
     Compiling tempfile v3.8.0
     Compiling peeking_take_while v0.1.2
     Compiling radium v0.7.0
     Compiling anstyle-query v1.0.0
     Compiling rustc-hash v1.1.0
     Compiling time-core v0.1.2
     Compiling scroll v0.11.0
     Compiling vsprintf v2.0.0
     Compiling log v0.4.20
     Compiling anstream v0.6.4
     Compiling time-macros v0.2.15
     Compiling proc-macro-crate v1.3.1
     Compiling terminal_size v0.3.0
     Compiling deranged v0.3.9
     Compiling cexpr v0.6.0
     Compiling tap v1.0.1
     Compiling strsim v0.10.0
     Compiling num_threads v0.1.6
     Compiling unicode-width v0.1.11
     Compiling nix v0.25.1
     Compiling threadpool v1.8.1
     Compiling regex v1.10.2
     Compiling wyz v0.5.1
     Compiling openat v0.1.21
     Compiling time v0.3.30
     Compiling nix v0.27.1
     Compiling funty v2.0.0
     Compiling termcolor v1.1.3
     Compiling ordered-float v3.9.2
     Compiling hex v0.4.3
     Compiling serde_derive v1.0.189
     Compiling thiserror-impl v1.0.50
     Compiling clap_derive v4.4.2
     Compiling scroll_derive v0.11.1
     Compiling simplelog v0.12.1
     Compiling libbpf-sys v1.2.1+v1.2.0
     Compiling ctrlc v3.4.1
     Compiling num_enum_derive v0.5.11
     Compiling strum_macros v0.24.3
     Compiling num_enum v0.5.11
     Compiling clap v4.4.6
     Compiling libbpf-rs v0.21.2
     Compiling cargo-platform v0.1.4
     Compiling bitvec v1.0.1
     Compiling fb_procfs v0.7.1
     Compiling cargo_metadata v0.15.4
     Compiling libbpf-cargo v0.21.2
     Compiling scx_rusty v0.5.0 (/sched_ext/sched_ext-sched_ext/tools/sched_ext/scx_rusty)
  error: failed to run custom build command for `scx_rusty v0.5.0 (/sched_ext/sched_ext-sched_ext/tools/sched_ext/scx_rusty)`
  
  Caused by:
    process didn't exit successfully: `/sched_ext/sched_ext-sched_ext/tools/sched_ext/build/release/build/scx_rusty-4bafe8d15851198d/build-script-build` (exit status: 101)
    --- stdout
    cargo:rerun-if-changed=src/bpf/rusty.h
    cargo:rerun-if-changed=/usr/lib/llvm-18/lib/clang/18/include/stdbool.h
  
    --- stderr
    Warning: can't set `imports_granularity = Item`, unstable features are only available in nightly channel.
    Warning: can't set `group_imports = StdExternalCrate`, unstable features are only available in nightly channel.
    Warning: can't set `version = Two`, unstable features are only available in nightly channel.
    clang
    thread 'main' panicked at build.rs:56:10:
    called `Result::unwrap()` on an `Err` value: Build(Failed to compile ./src/bpf/.output/rusty.bpf.o from ./src/bpf/rusty.bpf.c
  
    Caused by:
        0: Command `clang -g -D__TARGET_ARCH_x86 -mlittle-endian -I/sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include -I/sched_ext/sched_ext-sched_ext/tools/sched_ext -I/sched_ext/sched_ext-sched_ext/tools/include/uapi -I../../include -idirafter /usr/lib/llvm-18/lib/clang/18/include -idirafter /usr/local/include -idirafter /usr/include/x86_64-linux-gnu -idirafter /usr/include -Wall -Wno-compare-distinct-pointer-types -O2 -mcpu=v3 -I/tmp/.tmpaXAHib/bpf/src -fno-stack-protector -g -O2 -target bpf -c ./src/bpf/rusty.bpf.c -o ./src/bpf/.output/rusty.bpf.o` failed (exit status: 1)
        1: In file included from ./src/bpf/rusty.bpf.c:38:
           In file included from ./src/bpf/../../../scx_common.bpf.h:14:
           ./src/bpf/../../../user_exit_info.h:25:23: warning: declaration of 'struct scx_exit_info' will not be visible outside of this function [-Wvisibility]
              25 |                               const struct scx_exit_info *ei)
                 |                                            ^
           ./src/bpf/../../../user_exit_info.h:27:64: error: incomplete definition of type 'struct scx_exit_info'
              27 |         bpf_probe_read_kernel_str(uei->reason, sizeof(uei->reason), ei->reason);
                 |                                                                     ~~^
           ./src/bpf/../../../user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
              25 |                               const struct scx_exit_info *ei)
                 |                                            ^
           ./src/bpf/../../../user_exit_info.h:28:58: error: incomplete definition of type 'struct scx_exit_info'
              28 |         bpf_probe_read_kernel_str(uei->msg, sizeof(uei->msg), ei->msg);
                 |                                                               ~~^
           ./src/bpf/../../../user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
              25 |                               const struct scx_exit_info *ei)
                 |                                            ^
           ./src/bpf/../../../user_exit_info.h:30:65: error: incomplete definition of type 'struct scx_exit_info'
              30 |         __sync_val_compare_and_swap(&uei->exit_type, uei->exit_type, ei->type);
                 |                                                                      ~~^
           ./src/bpf/../../../user_exit_info.h:25:23: note: forward declaration of 'struct scx_exit_info'
              25 |                               const struct scx_exit_info *ei)
                 |                                            ^
           In file included from ./src/bpf/rusty.bpf.c:38:
           ./src/bpf/../../../scx_common.bpf.h:27:17: error: use of undeclared identifier 'SCX_DSQ_FLAG_BUILTIN'
              27 |         _Static_assert(SCX_DSQ_FLAG_BUILTIN,
                 |                        ^
           ./src/bpf/rusty.bpf.c:69:33: error: use of undeclared identifier 'SCX_SLICE_DFL'
              69 | const volatile __u64 slice_ns = SCX_SLICE_DFL;
                 |                                 ^
           ./src/bpf/rusty.bpf.c:74:17: error: use of undeclared identifier 'SCX_EXIT_NONE'; did you mean 'ATA_ECAT_NONE'?
              74 | int exit_type = SCX_EXIT_NONE;
                 |                 ^~~~~~~~~~~~~
                 |                 ATA_ECAT_NONE
           /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/vmlinux.h:135680:2: note: 'ATA_ECAT_NONE' declared here
            135680 |         ATA_ECAT_NONE = 0,
                   |         ^
           ./src/bpf/rusty.bpf.c:75:15: error: use of undeclared identifier 'SCX_EXIT_MSG_LEN'
              75 | char exit_msg[SCX_EXIT_MSG_LEN];
                 |               ^
           ./src/bpf/rusty.bpf.c:190:2: error: variable has incomplete type 'struct bpf_iter_num'
             190 |         bpf_for(cpu, 0, nr_cpus) {
                 |         ^
           /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:365:22: note: expanded from macro 'bpf_for'
             365 |         struct bpf_iter_num ___it __attribute__((aligned(8), /* enforce, just in case */        \
                 |                             ^
           /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:300:8: note: forward declaration of 'struct bpf_iter_num'
             300 | struct bpf_iter_num;
                 |        ^
           ./src/bpf/rusty.bpf.c:238:20: error: no member named 'scx' in 'struct task_struct'
             238 |                 vtime_delta = p->scx.dsq_vtime - old_domc->vtime_now;
                 |                               ~  ^
           ./src/bpf/rusty.bpf.c:265:6: error: no member named 'scx' in 'struct task_struct'
             265 |                 p->scx.dsq_vtime = new_domc->vtime_now + vtime_delta;
                 |                 ~  ^
           ./src/bpf/rusty.bpf.c:301:46: error: use of undeclared identifier 'SCX_WAKE_SYNC'; did you mean 'SOCK_WAKE_SPACE'?
             301 |         if (p->nr_cpus_allowed > 1 && (wake_flags & SCX_WAKE_SYNC)) {
                 |                                                     ^~~~~~~~~~~~~
                 |                                                     SOCK_WAKE_SPACE
           /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/vmlinux.h:73683:2: note: 'SOCK_WAKE_SPACE' declared here
            73683 |         SOCK_WAKE_SPACE = 2,
                  |         ^
           ./src/bpf/rusty.bpf.c:392:10: error: use of undeclared identifier 'SCX_PICK_IDLE_CORE'
             392 |                                             SCX_PICK_IDLE_CORE);
                 |                                             ^
           ./src/bpf/rusty.bpf.c:436:12: error: use of undeclared identifier 'SCX_PICK_IDLE_CORE'
             436 |                                                             SCX_PICK_IDLE_CORE);
                 |                                                             ^
           ./src/bpf/rusty.bpf.c:446:12: error: use of undeclared identifier 'SCX_PICK_IDLE_CORE'
             446 |                                                             SCX_PICK_IDLE_CORE);
                 |                                                             ^
           ./src/bpf/rusty.bpf.c:530:23: error: use of undeclared identifier 'SCX_DSQ_LOCAL'
             530 |                 scx_bpf_dispatch(p, SCX_DSQ_LOCAL, slice_ns, enq_flags);
                 |                                     ^
           ./src/bpf/rusty.bpf.c:553:18: error: no member named 'scx' in 'struct task_struct'
             553 |                 u64 vtime = p->scx.dsq_vtime;
                 |                             ~  ^
           ./src/bpf/rusty.bpf.c:606:2: error: variable has incomplete type 'struct bpf_iter_num'
             606 |         bpf_for(cpu, 0, nr_cpus) {
                 |         ^
           /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:365:22: note: expanded from macro 'bpf_for'
             365 |         struct bpf_iter_num ___it __attribute__((aligned(8), /* enforce, just in case */        \
                 |                             ^
           /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:300:8: note: forward declaration of 'struct bpf_iter_num'
             300 | struct bpf_iter_num;
                 |        ^
           ./src/bpf/rusty.bpf.c:644:2: error: variable has incomplete type 'struct bpf_iter_num'
             644 |         bpf_repeat(nr_doms - 1) {
                 |         ^
           /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:390:22: note: expanded from macro 'bpf_repeat'
             390 |         struct bpf_iter_num ___it __attribute__((aligned(8), /* enforce, just in case */        \
                 |                             ^
           /sched_ext/sched_ext-sched_ext/tools/sched_ext/build/include/bpf/bpf_helpers.h:300:8: note: forward declaration of 'struct bpf_iter_num'
             300 | struct bpf_iter_num;
                 |        ^
           ./src/bpf/rusty.bpf.c:698:39: error: no member named 'scx' in 'struct task_struct'
             698 |         if (vtime_before(domc->vtime_now, p->scx.dsq_vtime))
                 |                                           ~  ^
           fatal error: too many errors emitted, stopping now [-ferror-limit=]
           1 warning and 20 errors generated.
           )
    note: run with `RUST_BACKTRACE=1` environment variable to display a backtrace
  warning: build failed, waiting for other jobs to finish...
  make: *** [Makefile:218: scx_rusty] Error 101
```
