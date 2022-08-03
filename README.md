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
11 git clone https://github.com/Alekc74/FixRoutersploit.git
12 cd FixRoutersploit
13 chmod +x script.sh
14 ./script.sh
15 cd $Home
16 cd routersploit
17 pip install -r requirements.txt
18 pip install -r requirements-dev.txt
19 python3 rsf.py
