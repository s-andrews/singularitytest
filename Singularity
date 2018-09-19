Bootstrap: yum
OSVersion: 7
MirrorURL: http://mirror.centos.org/centos-%{OSVERSION}/%{OSVERSION}/os/$basearch/
Include: yum

%help
  This is a test image we're building just to make sure we know how

%setup
  touch ${SINGULARITY_ROOTFS}/i_made_a_file.txt
  
%post
  yum -y install numpy
  
%runscript
  python -c "import numpy; print numpy.__version__"
  
  

