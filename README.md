# 1 - Pong

Pong adalah salah satu game komputer awal, yang dikembangkan dari konsep simulasi tenis meja 2D oleh Alan Alcorn, dan dipublikasikan oleh Atari. Game ini dimainkan oleh 2 orang pemain. Masing-masing pemain mengendalikan sebuah raket berbentuk persegi panjang yang terletak di kiri dan kanan scene, serta bisa bergerak secara vertikal. Pada setiap ronde, sebuah bola akan bergerak dari tengah menuju salah satu pemain. Pemain tersebut harus mencegah bola tersebut melewati raketnya. Jika tidak, lawan akan mendapat skor dan bola akan kembali ke tengah. Game scene-nya dibatasi oleh empat buah dinding yang tak terlihat di tiap sisinya. Jika mengenai dinding atas atau bawah, bola akan terpantul. Sementara, jika bola menyentuh dinding di belakang raket seorang pemain, lawannya akan mendapat poin.

## Challenge

Kekurangan dari implementasi bola berdasarkan [tutorial ini](https://academy.dilo.id/side-course/course/view.php?id=59#section-0) adalah lajunya yang tidak stabil, dan bisa berbeda setiap kali bola mendapat gaya yang besarnya berbeda-beda saat bola mulai diluncurkan di set permainan baru.

Petunjuk: lakukan implementasi di metode BallControl.PushBall(), dan ingat bahwa yang dibuat sama adalah besar gayanya, bukan gayanya itu sendiri.

## Solution

Ubah xRandomInitialForce menggunakan rumus vektor ![rumus vektor](https://latex.codecogs.com/gif.latex?v%5E2%20%3D%20v_x%5E2%20&plus;%20v_y%5E2). Sehingga laju bola menjadi konstan.
