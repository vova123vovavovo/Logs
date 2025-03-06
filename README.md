GXL:BL1:9ac50e:a1974b;FEAT:ADFC318C;POC:3;RCY:0;EMMC:0;READ:0;0.0;CHK:0;
TE: 94540

BL2 Built : 13:48:56, Sep 23 2016. 
gxl g7459bd4 - jianxin.pan@droid06

set vcck to 1120 mv
set vddee to 1000 mv
Board ID = 3
CPU clk: 1200MHz
DQS-corr enabled
DDR scramble enabled
DDR3 chl: Rank0+1 @ 912MHz - FAIL
DDR3 chl: Rank0 @ 912MHz - PASS
Rank0: 1024MB(auto)-2T-13
DataBus test pass!
AddrBus test pass!
-s
Load fip header from eMMC, src: 0x0000c200, des: 0x01400000, size: 0x00004000
New fip structure!
Load bl30 from eMMC, src: 0x00010200, des: 0x01100000, size: 0x0000d600
Load bl31 from eMMC, src: 0x00020200, des: 0x10100000, size: 0x00015400
Load bl33 from eMMC, src: 0x00038200, des: 0x01000000, size: 0x000a9e00
NOTICE:  BL3-1: v1.0(debug):34b885f
NOTICE:  BL3-1: Built : 15:32:22, Oct 29 2016
aml log : bl31 normal boot !
[Image: gxl_v1.1.3154-065f772 2016-09-29 14:08:54 yan.wang@droid05]

OPS=0x82

6a 4c e1 b6 e8 22 80 9c c1 d b6 da [0.436475 Inits done]

secure task start!
high task start!
low task start!
INFO:    BL3-1: Initializing runtime services
WARNING: No OPTEE provided by BL2 boot loader
ERROR:   Error initializing runtime service opteed_fast
INFO:    BL3-1: Preparing for EL3 exit to normal world
INFO:    BL3-1: Next image address = 0x1000000
INFO:    BL3-1: Next image spsr = 0x3c9


U-Boot 2015.01 (Dec 07 2016 - 10:14:37)

DRAM:  1 GiB
Relocation Offset is: 36ec9000
register usb cfg[0][1] = 0000000037f5f9a0
vpu: error: vpu: check dts: FDT_ERR_BADMAGIC, load default parameters
vpu: clk_level = 7
vpu: set clk: 666667000Hz, readback: 666660000Hz(0x300)
vpp: vpp_init
boot_device_flag : 1
Nand PHY Ver:1.01.001.0006 (c) 2013 Amlogic Inc.
init bus_cycle=6, bus_timing=7, system=5.0ns
reset failed
get_chip_type and ret:fffffffe
get_chip_type and ret:fffffffe
chip detect failed and ret:fffffffe
nandphy_init failed and ret=0xfffffff1
MMC:   aml_priv->desc_buf = 0x0000000033ec96b0
aml_priv->desc_buf = 0x0000000033ecb9d0
SDIO Port B: 0, SDIO Port C: 1
emmc/sd response timeout, cmd8, status=0x1ff2800
emmc/sd response timeout, cmd55, status=0x1ff2800
[mmc_startup] mmc refix success
[mmc_init] mmc init success
mmc read lba=0x14000, blocks=0x400
Amlogic multi-dtb tool
      Multi dtb detected
      Multi dtb tool version: v2 .
      Support 2 dtbs.
        aml_dt soc: gxl platform: p212 variant: 1g
        dtb 0 soc: gxl   plat: p212   vari: 1g
        dtb 1 soc: gxl   plat: p212   vari: 2g
      Find match dtb: 0
start dts,buffer=0000000033ece270,dt_addr=0000000033ecea70
parts: 11
00:      logo	0000000002000000 1
01:  recovery	0000000002000000 1
02:       rsv	0000000000800000 1
03:       tee	0000000000800000 1
04:     crypt	0000000002000000 1
05:      misc	0000000002000000 1
06: instaboot	0000000020000000 1
07:      boot	0000000002000000 1
08:    system	0000000040000000 1
09:     cache	0000000020000000 2
10:      data	ffffffffffffffff 4
get_dtb_struct: Get emmc dtb OK!
overide_emmc_partition_table: overide cache 
[mmc_get_partition_table] skip partition cache.
Partition table get from SPL is : 
name                        offset              size              flag
===================================================================================
   0: bootloader                         0            400000                  0
   1: reserved                     2400000           4000000                  0
   2: cache                        6c00000          20000000                  2
   3: env                         27400000            800000                  0
   4: logo                        28400000           2000000                  1
   5: recovery                    2ac00000           2000000                  1
   6: rsv                         2d400000            800000                  1
   7: tee                         2e400000            800000                  1
   8: crypt                       2f400000           2000000                  1
   9: misc                        31c00000           2000000                  1
  10: instaboot                   34400000          20000000                  1
  11: boot                        54c00000           2000000                  1
  12: system                      57400000          40000000                  1
  13: data                        97c00000         13a400000                  4
mmc read lba=0x12000, blocks=0x2
mmc read lba=0x12002, blocks=0x2
mmc_read_partition_tbl: mmc read partition OK!
eMMC/TSD partition table have been checked OK!
mmc env offset: 0x27400000 
In:    serial
Out:   serial
Err:   serial
reboot_mode=cold_boot
hpd_state=0
cvbs performance type = 6, table = 0
[store]To run cmd[emmc dtb_read 0x1000000 0x40000]
read emmc dtb
      Amlogic multi-dtb tool
      Multi dtb detected
      Multi dtb tool version: v2 .
      Support 2 dtbs.
        aml_dt soc: gxl platform: p212 variant: 1g
        dtb 0 soc: gxl   plat: p212   vari: 1g
        dtb 1 soc: gxl   plat: p212   vari: 2g
      Find match dtb: 0
Net:   dwmac.c9410000
wipe_data=successful
wipe_cache=successful
upgrade_step=2
[OSD]load fb addr from dts
[OSD]failed to get fb addr for logo
[OSD]use default fb_addr parameters
[OSD]fb_addr for logo: 0x3d800000
[OSD]load fb addr from dts
[OSD]failed to get fb addr for logo
[OSD]use default fb_addr parameters
[OSD]fb_addr for logo: 0x3d800000
[CANVAS]canvas init
[CANVAS]addr=0x3d800000 width=3840, height=2160
amlkey_init() enter!
[EFUSE_MSG]keynum is 4
[BL31]: tee size: 0
[KM]Error:f[key_manage_query_size]L507:key[usid] not programed yet
[KM]Error:f[key_manage_query_size]L507:key[deviceid] not programed yet
get_cpu_id flag_12bit=1
saradc - saradc sub-system

Usage:
saradc saradc open <channel>		- open a SARADC channel
saradc close	- close the SARADC
saradc getval	- get the value in current channel
saradc get_in_range <min> <max>	- return 0 if current value in the range of current channel

key1 = a857ff00
key2 = a81bff00
time_out = 2625a0
ir init
irkey - irkey key_value1 key_value2 time_value

Usage:
irkey 
Hit Enter or space or Ctrl+C key to stop autoboot -- :  1  0 
card out
emmc/sd response timeout, cmd8, status=0x1ff2800
emmc/sd response timeout, cmd55, status=0x1ff2800
emmc/sd response timeout, cmd1, status=0x1ff2800
(Re)start USB...
USB0:   USB3.0 XHCI init start
Register 2000140 NbrPorts 2
Starting the controller
USB XHCI 1.00
    scanning bus 0 for devices... 2 USB Device(s) found
reading s905_autoscript
1654 bytes read in 23 ms (69.3 KiB/s)
## Executing script at 01020000
start amlogic old u-boot
## Error: "bootfromsd" not defined
emmc/sd response timeout, cmd8, status=0x1ff2800
emmc/sd response timeout, cmd55, status=0x1ff2800
emmc/sd response timeout, cmd1, status=0x1ff2800
** Bad device mmc 0 **
reading boot_android
** Unable to read file boot_android **
emmc/sd response timeout, cmd8, status=0x1ff2800
emmc/sd response timeout, cmd55, status=0x1ff2800
emmc/sd response timeout, cmd1, status=0x1ff2800
** Bad device mmc 0 **
reading u-boot.ext
** Unable to read file u-boot.ext **
emmc/sd response timeout, cmd8, status=0x1ff2800
emmc/sd response timeout, cmd55, status=0x1ff2800
emmc/sd response timeout, cmd1, status=0x1ff2800
** Bad device mmc 0 **
start test usb
reading uEnv.txt
1349 bytes read in 22 ms (59.6 KiB/s)
mac=98:aa:fc:60:05:b4
reading /zImage
28080640 bytes read in 14532 ms (1.8 MiB/s)
reading /uInitrd
10076354 bytes read in 5228 ms (1.8 MiB/s)
reading /dtb/amlogic/meson-gxl-s905x-hwacom-amazetv.dtb
25384 bytes read in 61 ms (406.3 KiB/s)
## Error: "aadmac" not defined
libfdt fdt_path_offset() returned FDT_ERR_NOTFOUND
[rsvmem] bl31 reserved memory set addr error.
## Loading init Ramdisk from Legacy Image at 13000000 ...
   Image Name:   uInitrd
   Image Type:   AArch64 Linux RAMDisk Image (gzip compressed)
   Data Size:    10076290 Bytes = 9.6 MiB
   Load Address: 00000000
   Entry Point:  00000000
   Verifying Checksum ... OK
      Amlogic multi-dtb tool
      Single dtb detected
load dtb from 0x1000000 ......
## Flattened Device Tree blob at 01000000
   Booting using the fdt blob at 0x1000000
libfdt fdt_path_offset() returned FDT_ERR_NOTFOUND
[rsvmem] bl31 reserved memory set addr error.
   Loading Ramdisk to 3351a000, end 33eb6082 ... OK
   Loading Device Tree to 000000001fff6000, end 000000001ffff327 ... OK
signature: 
fdt_instaboot: no instaboot image

Starting kernel ...

uboot time: 26866988 us
[    0.000000] Booting Linux on physical CPU 0x0000000000 [0x410fd034]
[    0.000000] Linux version 5.7.2-arm-64 (root@arm-64) (gcc version 9.3.0 (Ubuntu 9.3.0-10ubuntu2), GNU ld (GNU Binutils for Ubuntu) 2.34) #20.05.6 SMP PREEMPT Fri Jun 12 12:44:47 UTC 2020
[    0.000000] Machine model: Hwacom AmazeTV (S905X)
[    0.000000] efi: UEFI not found.
[    0.000000] Reserved memory: created CMA memory pool at 0x0000000023400000, size 256 MiB
[    0.000000] OF: reserved mem: initialized node linux,cma, compatible id shared-dma-pool
[    0.000000] NUMA: No NUMA configuration found
[    0.000000] NUMA: Faking a node at [mem 0x0000000001000000-0x0000000037ffffff]
[    0.000000] NUMA: NODE_DATA [mem 0x37e36100-0x37e37fff]
[    0.000000] Zone ranges:
[    0.000000]   DMA      [mem 0x0000000001000000-0x0000000037ffffff]
[    0.000000]   DMA32    empty
[    0.000000]   Normal   empty
[    0.000000] Movable zone start for each node
[    0.000000] Early memory node ranges
[    0.000000]   node   0: [mem 0x0000000001000000-0x0000000004ffffff]
[    0.000000]   node   0: [mem 0x0000000007300000-0x000000000fffffff]
[    0.000000]   node   0: [mem 0x0000000010200000-0x0000000037ffffff]
[    0.000000] Initmem setup node 0 [mem 0x0000000001000000-0x0000000037ffffff]
[    0.000000] psci: probing for conduit method from DT.
[    0.000000] psci: PSCIv0.2 detected in firmware.
[    0.000000] psci: Using standard PSCI v0.2 function IDs
[    0.000000] psci: Trusted OS migration not required
[    0.000000] percpu: Embedded 22 pages/cpu s51288 r8192 d30632 u90112
[    0.000000] Detected VIPT I-cache on CPU0
[    0.000000] CPU features: detected: ARM erratum 845719
[    0.000000] Built 1 zonelists, mobility grouping on.  Total pages: 212288
[    0.000000] Policy zone: DMA
[    0.000000] Kernel command line: root=LABEL=ROOTFS rootflags=data=writeback rw console=ttyAML0,115200n8 console=tty0 no_console_suspend consoleblank=0 fsck.fix=yes fsck.repair=yes net.ifnames=0 mac=98:aa:fc:60:05:b4
[    0.000000] Dentry cache hash table entries: 131072 (order: 8, 1048576 bytes, linear)
[    0.000000] Inode-cache hash table entries: 65536 (order: 7, 524288 bytes, linear)
[    0.000000] mem auto-init: stack:off, heap alloc:off, heap free:off
[    0.000000] Memory: 542712K/863232K available (16188K kernel code, 1310K rwdata, 6428K rodata, 3456K init, 944K bss, 58376K reserved, 262144K cma-reserved)
[    0.000000] random: get_random_u64 called from cache_random_seq_create+0x80/0x150 with crng_init=0
[    0.000000] SLUB: HWalign=64, Order=0-3, MinObjects=0, CPUs=4, Nodes=1
[    0.000000] rcu: Preemptible hierarchical RCU implementation.
[    0.000000] rcu: 	RCU restricting CPUs from NR_CPUS=8 to nr_cpu_ids=4.
[    0.000000] 	Tasks RCU enabled.
[    0.000000] rcu: RCU calculated value of scheduler-enlistment delay is 25 jiffies.
[    0.000000] rcu: Adjusting geometry for rcu_fanout_leaf=16, nr_cpu_ids=4
[    0.000000] NR_IRQS: 64, nr_irqs: 64, preallocated irqs: 0
[    0.000000] GIC: Using split EOI/Deactivate mode
[    0.000000] irq_meson_gpio: 110 to 8 gpio interrupt mux initialized
[    0.000000] arch_timer: cp15 timer(s) running at 24.00MHz (phys).
[    0.000000] clocksource: arch_sys_counter: mask: 0xffffffffffffff max_cycles: 0x588fe9dc0, max_idle_ns: 440795202592 ns
[    0.000003] sched_clock: 56 bits at 24MHz, resolution 41ns, wraps every 4398046511097ns
[    0.000356] Console: colour dummy device 80x25
[    0.000776] printk: console [tty0] enabled
[    0.000869] Calibrating delay loop (skipped), value calculated using timer frequency.. 48.00 BogoMIPS (lpj=96000)
[    0.000892] pid_max: default: 32768 minimum: 301
[    0.001006] LSM: Security Framework initializing
[    0.001064] SELinux:  Initializing.
[    0.001178] Mount-cache hash table entries: 2048 (order: 2, 16384 bytes, linear)
[    0.001199] Mountpoint-cache hash table entries: 2048 (order: 2, 16384 bytes, linear)
[    0.002551] rcu: Hierarchical SRCU implementation.
[    0.003432] EFI services will not be available.
[    0.003692] smp: Bringing up secondary CPUs ...
[    0.004242] Detected VIPT I-cache on CPU1
[    0.004291] CPU1: Booted secondary processor 0x0000000001 [0x410fd034]
[    0.004816] Detected VIPT I-cache on CPU2
[    0.004859] CPU2: Booted secondary processor 0x0000000002 [0x410fd034]
[    0.005377] Detected VIPT I-cache on CPU3
[    0.005419] CPU3: Booted secondary processor 0x0000000003 [0x410fd034]
[    0.005486] smp: Brought up 1 node, 4 CPUs
[    0.005556] SMP: Total of 4 processors activated.
[    0.005568] CPU features: detected: 32-bit EL0 Support
[    0.005580] CPU features: detected: CRC32 instructions
[    0.015193] CPU: All CPU(s) started at EL2
[    0.015250] alternatives: patching kernel code
[    0.016165] devtmpfs: initialized
[    0.021043] Registered cp15_barrier emulation handler
[    0.021072] Registered setend emulation handler
[    0.021087] KASLR disabled due to lack of seed
[    0.021403] clocksource: jiffies: mask: 0xffffffff max_cycles: 0xffffffff, max_idle_ns: 7645041785100000 ns
[    0.021460] futex hash table entries: 1024 (order: 4, 65536 bytes, linear)
[    0.028403] xor: measuring software checksum speed
[    0.068111]    8regs     :  2373.000 MB/sec
[    0.108142]    32regs    :  2723.000 MB/sec
[    0.148180]    arm64_neon:  2311.000 MB/sec
[    0.148191] xor: using function: 32regs (2723.000 MB/sec)
[    0.148255] pinctrl core: initialized pinctrl subsystem
[    0.148915] thermal_sys: Registered thermal governor 'step_wise'
[    0.149149] DMI not present or invalid.
[    0.149703] NET: Registered protocol family 16
[    0.151218] DMA: preallocated 256 KiB pool for atomic allocations
[    0.151259] audit: initializing netlink subsys (disabled)
[    0.151450] audit: type=2000 audit(0.148:1): state=initialized audit_enabled=0 res=1
[    0.152569] cpuidle: using governor ladder
[    0.152601] cpuidle: using governor menu
[    0.152940] hw-breakpoint: found 6 breakpoint and 4 watchpoint registers.
[    0.153030] ASID allocator initialised with 65536 entries
[    0.153778] Serial: AMBA PL011 UART driver
[    0.168680] HugeTLB registered 1.00 GiB page size, pre-allocated 0 pages
[    0.168707] HugeTLB registered 32.0 MiB page size, pre-allocated 0 pages
[    0.168720] HugeTLB registered 2.00 MiB page size, pre-allocated 0 pages
[    0.168734] HugeTLB registered 64.0 KiB page size, pre-allocated 0 pages
[    0.172532] cryptd: max_cpu_qlen set to 1000
[    0.248398] raid6: neonx8   gen()  2147 MB/s
[    0.316452] raid6: neonx8   xor()  1606 MB/s
[    0.384524] raid6: neonx4   gen()  2201 MB/s
[    0.452582] raid6: neonx4   xor()  1589 MB/s
[    0.520644] raid6: neonx2   gen()  2104 MB/s
[    0.588699] raid6: neonx2   xor()  1480 MB/s
[    0.656766] raid6: neonx1   gen()  1836 MB/s
[    0.724826] raid6: neonx1   xor()  1248 MB/s
[    0.792888] raid6: int64x8  gen()  1491 MB/s
[    0.860970] raid6: int64x8  xor()   784 MB/s
[    0.929002] raid6: int64x4  gen()  1668 MB/s
[    0.997053] raid6: int64x4  xor()   839 MB/s
[    1.065115] raid6: int64x2  gen()  1420 MB/s
[    1.133182] raid6: int64x2  xor()   730 MB/s
[    1.201234] raid6: int64x1  gen()  1055 MB/s
[    1.269298] raid6: int64x1  xor()   559 MB/s
[    1.269308] raid6: using algorithm neonx4 gen() 2201 MB/s
[    1.269319] raid6: .... xor() 1589 MB/s, rmw enabled
[    1.269329] raid6: using neon recovery algorithm
[    1.269804] ACPI: Interpreter disabled.
[    1.270693] iommu: Default domain type: Translated 
[    1.270950] vgaarb: loaded
[    1.271539] SCSI subsystem initialized
[    1.271947] usbcore: registered new interface driver usbfs
[    1.271992] usbcore: registered new interface driver hub
[    1.272061] usbcore: registered new device driver usb
[    1.272440] pps_core: LinuxPPS API ver. 1 registered
[    1.272453] pps_core: Software ver. 5.3.6 - Copyright 2005-2007 Rodolfo Giometti <giometti@linux.it>
[    1.272478] PTP clock support registered
[    1.272505] EDAC MC: Ver: 3.0.0
[    1.273390] FPGA manager framework
[    1.273499] Advanced Linux Sound Architecture Driver Initialized.
[    1.274034] NetLabel: Initializing
[    1.274049] NetLabel:  domain hash size = 128
[    1.274059] NetLabel:  protocols = UNLABELED CIPSOv4 CALIPSO
[    1.274111] NetLabel:  unlabeled traffic allowed by default
[    1.274605] clocksource: Switched to clocksource arch_sys_counter
[    1.274943] VFS: Disk quotas dquot_6.6.0
[    1.275012] VFS: Dquot-cache hash table entries: 512 (order 0, 4096 bytes)
[    1.275147] FS-Cache: Loaded
[    1.275471] pnp: PnP ACPI: disabled
[    1.280842] NET: Registered protocol family 2
[    1.281310] tcp_listen_portaddr_hash hash table entries: 512 (order: 1, 8192 bytes, linear)
[    1.281350] TCP established hash table entries: 8192 (order: 4, 65536 bytes, linear)
[    1.281420] TCP bind hash table entries: 8192 (order: 5, 131072 bytes, linear)
[    1.281530] TCP: Hash tables configured (established 8192 bind 8192)
[    1.281650] UDP hash table entries: 512 (order: 2, 16384 bytes, linear)
[    1.281686] UDP-Lite hash table entries: 512 (order: 2, 16384 bytes, linear)
[    1.281877] NET: Registered protocol family 1
[    1.282330] RPC: Registered named UNIX socket transport module.
[    1.282350] RPC: Registered udp transport module.
[    1.282361] RPC: Registered tcp transport module.
[    1.282371] RPC: Registered tcp NFSv4.1 backchannel transport module.
[    1.282387] NET: Registered protocol family 44
[    1.282408] PCI: CLS 0 bytes, default 64
[    1.282661] Trying to unpack rootfs image as initramfs...
[    1.726261] Freeing initrd memory: 9840K
[    1.727155] hw perfevents: enabled with armv8_cortex_a53 PMU driver, 7 counters available
[    1.935563] Initialise system trusted keyrings
[    1.935770] workingset: timestamp_bits=44 max_order=18 bucket_order=0
[    1.941353] zbud: loaded
[    1.942785] squashfs: version 4.0 (2009/01/31) Phillip Lougher
[    1.943093] FS-Cache: Netfs 'nfs' registered for caching
[    1.943685] NFS: Registering the id_resolver key type
[    1.943723] Key type id_resolver registered
[    1.943734] Key type id_legacy registered
[    1.943751] nfs4filelayout_init: NFSv4 File Layout Driver Registering...
[    1.943763] Installing knfsd (copyright (C) 1996 okir@monad.swb.de).
[    1.944943] FS-Cache: Netfs 'cifs' registered for caching
[    1.945272] Key type cifs.spnego registered
[    1.945298] Key type cifs.idmap registered
[    1.945321] ntfs: driver 2.1.32 [Flags: R/W].
[    1.945906] JFS: nTxBlock = 6364, nTxLock = 50918
[    1.949242] SGI XFS with ACLs, security attributes, realtime, quota, no debug enabled
[    1.951025] ocfs2: Registered cluster interface o2cb
[    1.951280] OCFS2 User DLM kernel interface loaded
[    1.952992] gfs2: GFS2 installed
[    1.954000] aufs 5.x-rcN-20200518
[    1.975076] NET: Registered protocol family 38
[    1.975106] Key type asymmetric registered
[    1.975118] Asymmetric key parser 'x509' registered
[    1.975128] Asymmetric key parser 'pkcs8' registered
[    1.975191] Block layer SCSI generic (bsg) driver version 0.4 loaded (major 245)
[    1.975368] io scheduler mq-deadline registered
[    1.975383] io scheduler kyber registered
[    1.975576] io scheduler bfq registered
[    1.988320] soc soc0: Amlogic Meson GXL (S905X) Revision 21:a (82:2) Detected
[    1.992130] Serial: 8250/16550 driver, 5 ports, IRQ sharing enabled
[    1.993798] Serial: AMBA driver
[    1.994096] c81004c0.serial: ttyAML0 at MMIO 0xc81004c0 (irq = 10, base_baud = 1500000) is a meson_uart
[    2.996218] printk: console [ttyAML0] enabled
[    3.012629] brd: module loaded
[    3.020956] loop: module loaded
[    3.025328] libphy: Fixed MDIO Bus: probed
[    3.025982] meson8b-dwmac c9410000.ethernet: IRQ eth_wake_irq not found
[    3.030395] meson8b-dwmac c9410000.ethernet: IRQ eth_lpi not found
[    3.036594] meson8b-dwmac c9410000.ethernet: PTP uses main clock
[    3.042455] meson8b-dwmac c9410000.ethernet: no reset control found
[    3.049122] meson8b-dwmac c9410000.ethernet: User ID: 0x11, Synopsys ID: 0x37
[    3.055758] meson8b-dwmac c9410000.ethernet: 	DWMAC1000
[    3.060914] meson8b-dwmac c9410000.ethernet: DMA HW capability register supported
[    3.068326] meson8b-dwmac c9410000.ethernet: RX Checksum Offload Engine supported
[    3.075743] meson8b-dwmac c9410000.ethernet: COE Type 2
[    3.080916] meson8b-dwmac c9410000.ethernet: TX Checksum insertion supported
[    3.087902] meson8b-dwmac c9410000.ethernet: Wake-Up On Lan supported
[    3.094337] meson8b-dwmac c9410000.ethernet: Normal descriptors
[    3.100153] meson8b-dwmac c9410000.ethernet: Ring mode enabled
[    3.105929] meson8b-dwmac c9410000.ethernet: Enable RX Mitigation via HW Watchdog Timer
[    3.114274] libphy: stmmac: probed
[    3.118512] VFIO - User Level meta-driver version: 0.3
[    3.123343] ehci_hcd: USB 2.0 'Enhanced' Host Controller (EHCI) Driver
[    3.128794] ehci-pci: EHCI PCI platform driver
[    3.133224] ehci-platform: EHCI generic platform driver
[    3.138484] ohci_hcd: USB 1.1 'Open' Host Controller (OHCI) Driver
[    3.144513] ohci-pci: OHCI PCI platform driver
[    3.148922] ohci-platform: OHCI generic platform driver
[    3.154488] usbcore: registered new interface driver usb-storage
[    3.160207] mousedev: PS/2 mouse device common for all mice
[    3.166352] i2c /dev entries driver
[    3.170785] Error: Driver 'khadas-mcu-fan-ctrl' is already registered, aborting...
[    3.177742] sdhci: Secure Digital Host Controller Interface driver
[    3.182619] sdhci: Copyright(c) Pierre Ossman
[    3.187060] Synopsys Designware Multimedia Card Interface Driver
[    3.194168] meson-gx-mmc d0074000.mmc: allocated mmc-pwrseq
[    3.224100] sdhci-pltfm: SDHCI platform and OF driver helper
[    3.225017] ledtrig-cpu: registered to indicate activity on CPUs
[    3.230747] meson-sm: secure-monitor enabled
[    3.235180] gxl-crypto c883e000.crypto: will run requests pump with realtime priority
[    3.242250] gxl-crypto c883e000.crypto: will run requests pump with realtime priority
[    3.265456] hid: raw HID events driver (C) Jiri Kosina
[    3.265673] usbcore: registered new interface driver usbhid
[    3.270505] usbhid: USB HID core driver
[    3.275191] platform-mhu c883c404.mailbox: Platform MHU Mailbox registered
[BL31]: tee size: 0
[    3.284135] no UART detected at 0x1
[    3.289327] NET: Registered protocol family 17
[    3.290975] Key type dns_resolver registered
[    3.295546] registered taskstats version 1
[    3.299143] Loading compiled-in X.509 certificates
[    3.304031] zswap: loaded using pool lzo/zbud
[    3.308613] Key type ._fscrypt registered
[    3.312114] Key type .fscrypt registered
[    3.316029] Key type fscrypt-provisioning registered
[    3.321934] Btrfs loaded, crc32c=crc32c-generic
[    3.347482] Key type encrypted registered
[    3.352554] mmc0: new HS200 MMC card at address 0001
[    3.353324] mmcblk0: mmc0:0001 8WPD3R 7.28 GiB 
[    3.356833] mmcblk0boot0: mmc0:0001 8WPD3R partition 1 4.00 MiB
[    3.362736] mmcblk0boot1: mmc0:0001 8WPD3R partition 2 4.00 MiB
[    3.368324] mmcblk0rpmb: mmc0:0001 8WPD3R partition 3 512 KiB, chardev (241:0)
[    3.370718] [drm] Supports vblank timestamp caching Rev 2 (21.10.2013).
[    3.382418] [drm] Initialized meson 1.0.0 20161109 for d0100000.vpu on minor 0
[    3.416333] Console: switching to colour frame buffer device 90x36
[    3.436726] meson-drm d0100000.vpu: fb0: mesondrmfb frame buffer device
[    3.444269] libphy: mdio_mux: probed
[    3.454715] libphy: mdio_mux: probed
[    3.456624] meson-gx-mmc d0072000.mmc: Got CD GPIO
[    3.483588] scpi_protocol scpi: SCP Protocol legacy pre-1.0 firmware
domain-0 init dvfs: 4

[    3.498497] printk: console [netcon0] enabled
[    3.500409] netconsole: network logging started
[    3.503834] ALSA device list:
[    3.506503]   No soundcards found.
[    3.512467] Freeing unused kernel memory: 3456K
[    3.514683] Run /init as init process
[    3.902111] random: fast init done
[   33.758990] VDDAO_3V3: disabling
[   33.767511] VDDIO_CARD: disabling
[  119.201585] random: crng init done
