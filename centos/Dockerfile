FROM centos:7.6.1810
LABEL author="HongXunPan&ChenKun <me@kangxuanpeng.com>"
RUN yum -y install gcc automake autoconf libtool make unzip initscripts.x86_64 vim epel-release wget && \
yum clean all && export LANG=C.UTF-8 && \
echo $'# .bashrc\n\
# User specific aliases and functions\n\
\n\
alias rm=\'rm -i\'\n\
alias cp=\'cp -i\'\n\
alias mv=\'mv -i\'\n\
alias cdsbin=\'cd /usr/local/sbin\'\n\
\n\
# Source global definitions\n\
if [ -f /etc/bashrc ]; then\n\
        . /etc/bashrc\n\
fi\n'> /root/.bashrc
ENTRYPOINT /bin/bash