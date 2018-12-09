# debiandowngrade
Downgrade debian 10
script:

++


echo '
apt-get install ca-certificates -y;
apt-get update;
apt-get upgrade -y;
apt-get dist-upgrade -y;
apt autoremove -y;
' > downgrade.sh && chmod +x downgrade.sh && sh downgrade.sh && echo "ejecución terminada!" && rm downgrade.sh;

++
