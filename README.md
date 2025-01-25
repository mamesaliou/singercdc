curl https://pyenv.run | bash

export PATH="$HOME/.pyenv/bin:$PATH"
eval "$(pyenv init --path)"
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"

source ~/.bashrc

pyenv install 3.10.0
pyenv global 3.10.0

python3.10 -m venv myenv

source myenv/bin/activate



