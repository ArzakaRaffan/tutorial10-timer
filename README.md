# Tutorial 10 - Timer

## 1.2 Understanding How It Works

![alt text](image.png)

Ketika dilakukan cargo run, hal pertama yang di-_print_ adalah `Arzaka's Komputer: hey hey`. Hal ini dapat terjadi karena perintah _print_ tersebut terletak di luar async block walaupun berada di bawahnya. Hal ini mennyebabkan perintah tersebut dieksekusi secara _synchronous_ dan langsung. Setelah itu, `executor.run` baru memproses hal-hal yang dilakukan oleh `spawner.spawn()`