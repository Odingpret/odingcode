Update vps
apt-get update && apt-get upgrade -y && update-grub && sleep 2 && reboot

Masukan domain
cat >/root/domain <<EOF
sg3-dev.axsupernet.online
EOF

mkdir -p /etc/xray
cat >/etc/xray/domain <<EOF
sg3-dev.axsupernet.online
EOF

Install

wget https://raw.githubusercontent.com/Odingpret/odingcode/main/setup.sh && chmod +x setup.sh && ./setup.sh
