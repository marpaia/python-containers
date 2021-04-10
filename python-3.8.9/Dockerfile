FROM gcr.io/python-containers/python-builder:v0.1.0

ENV PYENV_ROOT="$HOME/pyenv"
ENV PATH="$PYENV_ROOT/bin:$PATH"
RUN git clone https://github.com/pyenv/pyenv.git $PYENV_ROOT
RUN git clone https://github.com/pyenv/pyenv-virtualenv.git $PYENV_ROOT/plugins/pyenv-virtualenv

RUN pyenv install 3.8.9
ENV PATH="$PYENV_ROOT/versions/3.8.9/bin:$PATH"
RUN pip install --upgrade pip