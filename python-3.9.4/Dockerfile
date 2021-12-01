FROM gcr.io/python-containers/python-builder:v0.2.0

ENV PYENV_ROOT="$HOME/pyenv"
ENV PATH="$PYENV_ROOT/bin:$PATH"
RUN git clone https://github.com/pyenv/pyenv.git $PYENV_ROOT
RUN git clone https://github.com/pyenv/pyenv-virtualenv.git $PYENV_ROOT/plugins/pyenv-virtualenv

RUN pyenv install 3.9.4
ENV PATH="$PYENV_ROOT/versions/3.9.4/bin:$PATH"
RUN pip install --upgrade pip
