# 1

Dev Ops adalah sebuah set praktik dan para pengembang yang bekerja sama untuk men-*support* sebuah layanan, dimulai dari selama pengembangan sampai ke bagian *production*.

Tanpa Dev Ops, 

# 2

Docker adalah sebuah container yang fungsi utamanya untuk menge-*ship* sebuah software tanpa perlu memikirkan dependensi, semua dependensi software di-*bundle* menjadi sebuah *image* dan *image* ini bisa di-transfer ke host apapun tanpa menginstall dependensi di host tersebut, mirip seperti virtual machine namun host dan guest docker menggunakan kernel yang sama (dan *optionally* resource lain yang sama), jauh lebih sedikit *overhead*-nya dibandingkan virtual machine. Sedangkan Kubernetes adalah container manager, Kubernetes seperti layaknya orkestra yang memandu container-container yang di-*manage*, Kubernetes dapat mengatur *scale*, *deploy* otomatis, dan mengatur container-container.

# 3

Untuk mencari sebuah command yang pernah dijalankan, kita bisa menggunakan Tombol up untuk menampilkan command sebelumnya. Kita juga bisa melihat histori command yang pernah dijalankan, umumnya file histori terletak pada $HOME/.bash_history (dimana ```$HOME``` adalah ```/home/<nama user>``` bagi user biasa dan ```/root``` bagi root user), untuk melihatnya kita bisa execute command ```cat ~/.bash_history``` atau ```less ~/.bash_history```, untuk mencari command di histori, execute command ```grep "$search" ~/.bash_history``` (dimana $search merupakan apa yang kita ingin cari)

# 5
```
cat << EOF > file.sh
useradd -m lemniskett                 # flag -m untuk membuat home directory (opsional tapi dianjurkan)
sudo apt update && sudo apt upgrade   # menggunakan && agar sudo apt upgrade tidak berjalan bila sudo apt update gagal
EOF
```
# 6
```
cd path/to/repo                                                   # change directory ke git repo lokal
git remote                                                        # check bila sudah ada remote atau tidak
git remote add origin https://github.com/lemniskett/Dumbways.git  # Bila tidak, tambahkan remote dengan nama origin
git commit -m "Commit message"                                    # Commit perubahan
git push origin master                                            # Upload perubahan ke remote origin branch master
```
