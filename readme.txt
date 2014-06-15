What does it support:
1. partition style: both MBR and GPT
2. partition type: both primary and logical
3. partition format: all
4. windows version: all windows version since winxp, like, winxp, vista, win7, win8(win8.1)
5. platform architect: x86(32bit), x64(64bit)
6. support maximum disk number: 10
7. support maximum partition number in a disk: 26

note:
1. system partition: all GPT system partition, and partition whose size is not larger than 300MB.
in the test application, these partition names are prefixed with star.
2. boot area: the free space before the first partition in a disk
3. page file should be put into swap partitions

How to config:
1. tick all partitions you want to protect, tick boot area and system partition for most security
must select one of them as the swap partition(page file path will changed to here).
don't select the partition where windows is installed first, so that we can remove page file after reboot.
2. reboot
3. tick the windows partition now. the page files in this partition is removed automaticly.
4. install driver, and reboot.
