# docker-machine-doctor

Your Docker MD. A tool that helps debugging problems with docker-machine. For
example, what takes up the virtual hard disk space.


## Limitations

Currently only supporting `virtualbox` driver.


## Installation

    $ curl -O https://raw.githubusercontent.com/djui/docker-machine-doctor/master/docker-machine-doctor && \
          chmod u+x docker-machine-doctor


## Usage

    $ docker-machine-doctor
    Usage: docker-machine-doctor <name>

    $ docker-machine-doctor
    Docker client and server version:
    Client:
     Version:      1.9.0
     API version:  1.21
     Go version:   go1.4.3
     Git commit:   76d6bc9
     Built:        Tue Nov  3 19:20:09 UTC 2015
     OS/Arch:      darwin/amd64

    Server:
     Version:      1.9.0
     API version:  1.21
     Go version:   go1.4.3
     Git commit:   76d6bc9
     Built:        Tue Nov  3 19:20:09 UTC 2015
     OS/Arch:      linux/amd64


    Docker machine version:
    docker-machine version 0.5.1 (7e8e38e)


    Intermediate images:


    Containers:
    CONTAINER ID        IMAGE               SIZE
    83e8ce72d772        ubuntu              0 B
    68b061a29aa9        ubuntu              0 B


    Docker machine store path:
    /Users/uwe/.docker/machine


    Virtual hard drive mounted:
    Yes.


    Filesystem mounts:
    Filesystem           Type            Size      Used Available Use% Mounted on
    none                 vboxsf        232.7G    215.6G     17.1G  93% /Users
    /dev/sda1            ext4           18.2G      5.6G     11.6G  32% /mnt/sda1/var/lib/docker/aufs
    /dev/sda1            ext4           18.2G      5.6G     11.6G  32% /mnt/sda1
    tmpfs                tmpfs         896.6M    123.8M    772.8M  14% /
    fusectl              fusectl            0         0         0   0% /sys/fs/fuse/connections
    cgroup               cgroup             0         0         0   0% /sys/fs/cgroup/perf_event
    cgroup               cgroup             0         0         0   0% /sys/fs/cgroup/net_prio
    cgroup               cgroup             0         0         0   0% /sys/fs/cgroup/net_cls
    cgroup               cgroup             0         0         0   0% /sys/fs/cgroup/memory
    cgroup               cgroup             0         0         0   0% /sys/fs/cgroup/hugetlb
    cgroup               cgroup             0         0         0   0% /sys/fs/cgroup/freezer
    cgroup               cgroup             0         0         0   0% /sys/fs/cgroup/devices
    cgroup               cgroup             0         0         0   0% /sys/fs/cgroup/cpuset
    cgroup               cgroup             0         0         0   0% /sys/fs/cgroup/cpuacct
    cgroup               cgroup             0         0         0   0% /sys/fs/cgroup/cpu
    cgroup               cgroup             0         0         0   0% /sys/fs/cgroup/blkio
    cgroup               tmpfs         498.1M         0    498.1M   0% /sys/fs/cgroup
    sysfs                sysfs              0         0         0   0% /sys
    proc                 proc               0         0         0   0% /proc
    tmpfs                tmpfs         498.1M         0    498.1M   0% /dev/shm
    devpts               devpts             0         0         0   0% /dev/pts


    Disk space usage: Containers:
    92.0K	/mnt/sda1/var/lib/docker/containers/


    Disk space usage: Volumes:
    2.6G	/mnt/sda1/var/lib/docker/volumes/

    16M	/mnt/sda1/var/lib/docker/volumes/6a5765eda4e7b16c2b7bb811acc2cf5e89b0231b6901ad490c001ccdbb6d681c/_data/pg_xlog/000000010000000000000001
    6M	/mnt/sda1/var/lib/docker/volumes/fd9dbf6af869ff62f56b0b51b830db7923f11d45524343732b3ba42bf76f024d/_data/cde-package/cde-root/usr/lib/lapack/liblapack.so.3.0
    6M	/mnt/sda1/var/lib/docker/volumes/f75dc365db96d1388bea66645a226f6128d03e46d6c06e3aca258b0d1ef84f49/_data/cde-package/cde-root/usr/lib/lapack/liblapack.so.3.0
    6M	/mnt/sda1/var/lib/docker/volumes/f5c05e5433c0bd2d16238a03f5b86d7725c2b203ce09a26cf5bda5876fe78d42/_data/cde-package/cde-root/usr/lib/lapack/liblapack.so.3.0
    6M	/mnt/sda1/var/lib/docker/volumes/f2c2b932fa82876e66bb07096ad87d66b10485fc99cef755599855176b52a271/_data/cde-package/cde-root/usr/lib/lapack/liblapack.so.3.0
    6M	/mnt/sda1/var/lib/docker/volumes/ee44f1441f29dc440b3bab01b35a856cc1d830a81d75f6072249c69b9ea17178/_data/cde-package/cde-root/usr/lib/lapack/liblapack.so.3.0
    6M	/mnt/sda1/var/lib/docker/volumes/e3e96cf15013917b8ceef50a38ca3478618ac8d7366837352595ccde9f946d66/_data/cde-package/cde-root/usr/lib/lapack/liblapack.so.3.0
    6M	/mnt/sda1/var/lib/docker/volumes/dd93dc68fe94b74af0f0ad3c196575079dd9c226c1726d52d38b8c400b394148/_data/cde-package/cde-root/usr/lib/lapack/liblapack.so.3.0


    Disk space usage: Filesystem:
    2.7G	/mnt/sda1/var/lib/docker/aufs/diff/

    62M	/mnt/sda1/var/lib/docker/aufs/diff/74afa1361abd1e949e88e2e6e42e2162a70db0dd73ec1511988beddbe0566400/usr/lib/jvm/java-8-openjdk-amd64/jre/lib/rt.jar
    29M	/mnt/sda1/var/lib/docker/aufs/diff/74afa1361abd1e949e88e2e6e42e2162a70db0dd73ec1511988beddbe0566400/usr/lib/x86_64-linux-gnu/libLLVM-3.5.so.1
    24M	/mnt/sda1/var/lib/docker/aufs/diff/8f1dd6bff9f9e343df2637a8655615ff1e89ef8f42ad6037d9643e357c696ea1/var/cache/yum/x86_64/7/updates/gen/primary_db.sqlite
    24M	/mnt/sda1/var/lib/docker/aufs/diff/8f1dd6bff9f9e343df2637a8655615ff1e89ef8f42ad6037d9643e357c696ea1/var/cache/yum/x86_64/7/base/gen/primary_db.sqlite
    22M	/mnt/sda1/var/lib/docker/aufs/diff/95d5449d9dc1f8e354542adcb5b8c81e8a1c0f9823ea62f6678fd060153d148f/usr/src/dist/vnu.jar
    22M	/mnt/sda1/var/lib/docker/aufs/diff/8ca313dfa777e3bb99605e2b520b76a21c956145db4a7338436868570c56c4f8/usr/lib/x86_64-linux-gnu/libicudata.so.52.1
    22M	/mnt/sda1/var/lib/docker/aufs/diff/88405815da081388c311e7171f1b7b858737ce71b07db6df75b565f66719be3a/usr/src/vnu.jar.zip
    20M	/mnt/sda1/var/lib/docker/aufs/diff/8f1dd6bff9f9e343df2637a8655615ff1e89ef8f42ad6037d9643e357c696ea1/usr/lib64/libicudata.so.50.1.2
    19M	/mnt/sda1/var/lib/docker/aufs/diff/74afa1361abd1e949e88e2e6e42e2162a70db0dd73ec1511988beddbe0566400/usr/lib/jvm/java-8-openjdk-amd64/jre/lib/amd64/server/classes.jsa
    17M	/mnt/sda1/var/lib/docker/aufs/diff/8f1dd6bff9f9e343df2637a8655615ff1e89ef8f42ad6037d9643e357c696ea1/var/lib/rpm/Packages


    Disk space usage: Temporary files:
    16.0K	/mnt/sda1/lost+found/
    16.0K	/mnt/sda1/tmp/
    148.0M	/mnt/sda1/var/lib/docker/tmp/

    74M	/mnt/sda1/var/lib/docker/tmp/docker-builder251338753/cde-package/sanitized-root.tar
    7M	/mnt/sda1/var/lib/docker/tmp/docker-builder251338753/pkg/formats/xlsx/mapping/calibri.ttx
    6M	/mnt/sda1/var/lib/docker/tmp/docker-builder251338753/cde-package/cde-root/usr/lib/lapack/liblapack.so.3.0
    4M	/mnt/sda1/var/lib/docker/tmp/docker-builder251338753/cde-package/cde-root/usr/lib/x86_64-linux-gnu/libgtk-x11-2.0.so.0.2400.25
    4M	/mnt/sda1/var/lib/docker/tmp/docker-builder251338753/cde-package/cde-root/usr/bin/python2.7
    3M	/mnt/sda1/var/lib/docker/tmp/docker-builder251338753/cde-package/cde-root/usr/lib/x86_64-linux-gnu/libpoppler.so.46.0.0
    3M	/mnt/sda1/var/lib/docker/tmp/docker-builder251338753/cde-package/cde-root/usr/lib/python2.7/dist-packages/gtk-2.0/gtk/_gtk.so
    2M	/mnt/sda1/var/lib/docker/tmp/docker-builder251338753/cde-package/cde-root/usr/lib/x86_64-linux-gnu/libcrypto.so.1.0.0
    2M	/mnt/sda1/var/lib/docker/tmp/docker-builder251338753/cde-package/cde-root/usr/bin/git
    2M	/mnt/sda1/var/lib/docker/tmp/docker-builder251338753/cde-package/cde-root/lib/x86_64-linux-gnu/libc-2.19.so
