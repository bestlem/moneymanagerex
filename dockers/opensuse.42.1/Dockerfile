FROM opensuse:42.1
MAINTAINER developers@moneymanagerex.org
RUN zypper install -y --no-recommends \
      cmake gettext-tools gcc-c++ git make rpm-build lsb-release \
      wxWidgets-3_0-devel libcurl-devel \
      automake libtool ccache \
 && zypper clean --all

ENV MMEX_INST_CMD zypper --no-refresh --no-gpg-checks install -y ./mmex-*.rpm
