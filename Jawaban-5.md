# 5

cat << EOF > file.sh
useradd -m lemniskett # flag -m untuk membuat home directory (opsional tapi dianjurkan)
sudo apt update && sudo apt upgrade # menggunakan && agar sudo apt upgrade tidak berjalan bila sudo apt update gagal
EOF
