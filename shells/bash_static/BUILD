(

   bad_flags -malign-double -s

   OPTS+=" --bindir=/bin                 \
           --without-bash-malloc         \
           --without-installed-readline  \
           --with-curses                 \
           --enable-static-link          \
           --disable-profiling"         &&

   default_config   &&
   make version.h   &&
   make             &&
   prepare_install  &&

   cp -f bash /bin/bash_static

) > $C_FIFO 2>&1
