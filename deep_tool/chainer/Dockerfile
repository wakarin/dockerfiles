From chainer/chainer:latest-python3
MAINTAINER Kenta Yamazaki

RUN apt update -q && apt install -y git vim

# install open cv
RUN apt install -y libglib2.0.0 \
                libsm-dev \
                libxrender1
RUN pip3 install cython
RUN pip3 install opencv-python

RUN pip3 install Pillow \
                argparse \
                ipython \
                matplotlib



CMD ["/bin/bash"]
