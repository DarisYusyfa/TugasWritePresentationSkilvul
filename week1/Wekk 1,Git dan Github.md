# **Rangkuman Week 1**

## Git & github
Pengenalan git :
Git adalah version system kontrol
apa itu version system kontrol? yaitu untuk membuat setiap perubahan pada file baik dikerjakan secara individu maupun tim
Git adalah tools untuk para programmer sebagai tempat penyimpanan project mereka karena lebih efektif dengan begitu akan terlihat semua perubahannya dan siapa yang telah mengubah nya
-Dengan menggunakan GIT dan Github, kita bekerja dalam sebuat tim. Tujuan besarnya adalah kamu bisa berkolaborasi mengerjakan proyek yang sama tanpa harus repot copy paste folder aplikasi yang terupdate.

## Setup Awal
kita bisa melakukan perintah dalam gitbash yaitu dengan mengetikan
git config --global user.name "nama anda" > fungsinya yaitu untuk menambahkan nama kita kedalam program gitbash tersebut
git condif --global user.email emailanda@gamil.com > fungsinya yaitu untuk menambahkan gmail kita

adapun cara mengecek apakah berhasil yaitu dengan mengetikan git config --list

## Membuat Repository
kita bisa mengetikan perintah git ini namaRepository dengan mengetikan perintah
- git clone <https://link-repositori> =Git clone adalah perintah untuk mengunduh kode sumber yang ada dari repositori jarak jauh (seperti Github, misalnya). Dengan kata lain, git clone pada dasarnya membuat salinan identik dari versi terbaru proyek dalam repositori dan menyimpannya ke komputer
- git branch <nama-branch> = Dengan menggunakan branch, beberapa pengembang dapat bekerja secara paralel pada proyek yang sama secara bersamaan. Kita dapat menggunakan perintah git branch untuk membuat, mendaftar dan menghapus branch.
- git push -u <remote> <nama-branch> = Perintah ini akan membuat branch secara lokal. Untuk melakukan push branch baru ke repositori jarak jauh
- git branch atau git branch --list = untuk melihat branch
- git branch -d <nama-branch> = untuk menghapus branch = 
- git checkout <nama-cabang-kamu> = untuk berpindah dari satu branch ke branch lain
- git checkout -b <nama-cabang-anda> = untuk berpindah dan membuat branch sekaligus

Kita dapat mengumpulkan informasi seperti:
Apakah branch saat ini adalah yang terbaru
Apakah ada sesuatu untuk di commit, push atau pull
Apakah ada file yang dipentaskan, tidak dipentaskan, atau tidak dilacak
Apakah ada file yang dibuat, dimodifikasi atau dihapus
yaitu dengan mengetikan perintah
- git status

Saat kita membuat, memodifikasi, atau menghapus file, perubahan ini akan terjadi di lokal dan tidak akan dimasukkan dalam commit berikutnya (kecuali kita mengubah konfigurasi).
Kita perlu menggunakan perintah git add untuk memasukkan perubahan file ke commit selanjutnya

- git add <file> = Untuk menambahkan satu file
- git add -A = untuk menambahkan semua file sekaligus
- git commit -m "pesan commit" = untuk menyimpan perubahan pada penyimpanan lokal kita
- git push <remote> <nama-branch> = Setelah melakukan perubahan, hal berikutnya yang ingin Anda lakukan adalah mengirim perubahan ke server jauh (remote). Git push mengunggah commit Anda ke repositori jarak jauh

Namun, jika cabang Anda baru dibuat, maka Anda juga perlu mengunggah cabang dengan perintah berikut:
- git push --set-upstream <remote> <nama-branch-anda>
atau
git push -u origin <nama-branch
- git pull <remote> = Perintah git pull digunakan untuk mendapatkan pembaruan dari repo jarak jauh
- git revert = untuk membatalkan namun sebaum melakukan perintah tersebut kita harus melihat kode dari file yang kita upload dengan mengetikan 
- git log--oneline
- git merge = yaitu untuk menggabungkan branch dev dengan master

Misalnya, ketika Anda ingin menggabungkan fitur branch Anda ke branch dev:
Pertama, Anda harus beralih ke branch dev:

- git checkout dev
Sebelum melakukan merging, Anda harus memperbarui branch dev lokal Anda:
- git fetch
Terakhir, Anda dapat menggabungkan branch fitur Anda menjadi dev:
- git merge <nama-branch>
