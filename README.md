Fix RouterSploit Termux
python -m pip install wheel
pkg install rust
export CARGO_BUILD_TARGET=arm7-linux-androideabi && pip install cryptography
termux-fix-shebang rsf.py
python3 rsf.py
