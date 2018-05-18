FROM archlinux/base:latest

RUN pacman -Sy --noconfirm neovim git \
                python python-pip \
                gcc make && \
RUN pip install neovim
# python for deoperate, make for vimporc

RUN git clone https://github.com/wakarin/vimconfig ~/.config/nvim
RUN git clone https://github.com/Shougo/dein.vim.git ~/.config/nvim/dein/repos/github.com/Shougo/dein.vim
RUN mkdir ~/.config/nvim/backup
RUN echo "alias vi='nvim'" >> ~/.bashrc

CMD /bin/bash
