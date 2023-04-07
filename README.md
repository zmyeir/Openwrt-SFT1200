# Openwrt for GL.iNET SFT1200

編譯方法
cd openwrt-18.06

./scripts/feeds update -a && ./scripts/feeds install -a

make menuconfig

load載入SFT1200設定檔: .config.sft1200

然後選擇自己要的app

make -j8 download && make V=s -j$(nproc)
