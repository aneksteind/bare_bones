# bare_bones
Minimal kernel from [OS dev wiki](https://wiki.osdev.org/Bare_Bones)

Verify multiboot compatibility with
```
grub-file --is-x86-multiboot myos.bin
```

Enter the kernel with
```
qemu-system-i386 -kernel myos.bin
```

or

```
grub-mkrescue -o myos.iso isodir
qemu-system-i386 -cdrom myos.iso
```

If booting from a CD doesn't work because the CD can't be found, try this first:
```
sudo apt-get install grub-pc-bin
```

