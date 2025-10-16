# debian
```
xorriso -as mkisofs \
  -r -J \
  -b isolinux/isolinux.bin \
  -c isolinux/boot.cat \
  -no-emul-boot \
  -boot-load-size 4 \
  -boot-info-table \
  -eltorito-alt-boot \
  -e boot/grub/efi.img \
  -no-emul-boot \
  -isohybrid-mbr /usr/lib/ISOLINUX/isohdpfx.bin \
  -isohybrid-gpt-basdat \
  -V "DEBIAN_ALIYUN_AUTO" \
  -o /root/debian-12.9.0-auto.iso \
  .

```
