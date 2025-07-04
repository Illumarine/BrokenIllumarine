# BrokenIllumarine
Debugging current issues with the Illumarine ISO files

## Issues List

### CURRENT: 
1. Boots into GRUB, cannot find kernel. Unsure of how the bug is happening.

### Reprod:
1. > build illumos-gate, Run following command
   ```sh
        mkiso-fs -o name.iso \
        -b boot/grub/stage2_eltorito \
        -no-emul-boot \
        -boot-load-size 4 \
        -boot-info-table \
        -R -J -l \
        root_i386/
   ```
