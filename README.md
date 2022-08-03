Fix RouterSploit Termux
1 termux-change-repo
2 pkg upgrade
3 termux-change-repo
4 pkg install python
5 pkg install wget
6 pkg install git
7 pip install wheel
8 pkg install rust
9 export CARGO_BUILD_TARGET="$(rustc -Vv | grep "host" | awk '{print $2}')"
10 pip install cryptography
