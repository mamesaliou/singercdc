curl https://pyenv.run | bash

export PYENV_ROOT="$HOME/.pyenv"
[[ -d $PYENV_ROOT/bin ]] && export PATH="$PYENV_ROOT/bin:$PATH"
eval "$(pyenv init - bash)"

source ~/.bashrc

pyenv install 3.10.0
pyenv global 3.10.0

python3.10 -m venv myenv

source myenv/bin/activate



