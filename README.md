Fix RouterSploit Termux
pip install rust
export CARGO_BUILD_TARGET=arm7-linux-androideabi && pip install cryptography
termux-fix-shebang rsf.py
python3 rsf.py
