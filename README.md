# bare_bones
minimal kernel from [OS dev wiki](https://wiki.osdev.org/Bare_Bones)

verify multiboot compatibility with
```
grub-file --is-x86-multiboot myos.bin
```

enter the kernel with
```
qemu-system-i386 -kernel myos.bin
```

