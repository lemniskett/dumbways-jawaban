# 3

Untuk mencari sebuah command yang pernah dijalankan, kita bisa menggunakan Tombol up untuk menampilkan command sebelumnya. Kita juga bisa melihat histori command yang pernah dijalankan, umumnya file histori terletak pada $HOME/.bash_history (dimana $HOME adalah /home/<nama user> bagi user biasa dan /root bagi root user), untuk melihatnya kita bisa execute command ```cat ~/.bash_history``` atau ```less ~/.bash_history```, untuk mencari command di histori, execute command ```grep "$search" ~/.bash_history``` (dimana $search merupakan apa yang kita ingin cari)
