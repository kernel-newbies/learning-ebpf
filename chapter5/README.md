# Chapter 5 - CO-RE, BTF and libbpf

Run `make` to build the examples in this file. In the book you'll explore the
BTF data associated with the example code, as well as comparing the libbpf
approach to earlier BCC examples.


My problem was: 
the vmlinux.h file was not correct for my Linux. In order to solve that I
create a new vmlinux.h file with this command:

```bash
bpftool btf dump file /sys/kernel/btf/vmlinux format c > vmlinux.h
```

