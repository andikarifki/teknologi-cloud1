# 215611102 - Andika Rifqi IStanto

# Materi
## Data as a service
Dalam komputasi, data sebagai layanan, atau DaaS, adalah istilah yang digunakan untuk menggambarkan perangkat lunak berbasis cloud yang digunakan untuk bekerja dengan data, seperti mengelola data di gudang data atau menganalisis data dengan kecerdasan bisnis. Ini diaktifkan oleh perangkat lunak sebagai layanan (SaaS).[1] Seperti semua teknologi "sebagai layanan" (aaS), DaaS dibangun di atas konsep bahwa produk datanya dapat diberikan kepada pengguna sesuai permintaan, [2] terlepas dari pemisahan geografis atau organisasi antara penyedia dan konsumen. Arsitektur berorientasi layanan (SOA) dan meluasnya penggunaan API telah menjadikan platform tempat data berada sebagai tidak relevan.[3]

Data sebagai layanan sebagai model bisnis adalah konsep ketika dua atau lebih organisasi membeli, menjual, atau memperdagangkan data yang dapat dibaca mesin dengan imbalan sesuatu yang bernilai.[4]
# Sofware Yang Diperlukan
- [Download Go]()
- [Download MySQL](https://www.nesabamedia.com/download-mysql/)
- [Download MongoDB](https://www.mongodb.com/try/download/community)

> Latihan

Install go, mysql, dan mongoDB
 
mongodb
 
Golang connection to PHPMySQL 
1.	Buat direktori “ mkdir project-pertama”
2.	Masuk ke direktori “cd project-pertama”
3.	Untuk membuat go.mod ketik “go init project-pertama”
4.	Cek file terlebih dahulu ketik “dir”
 
5.	Setting path variabel terlebih dahulu
 
Install gopath
 

Koneksi mysql
1.	Instalasi driver terlebih dahulu ketik “ go get  github.com/go-sql-driver/mysql”
2.	Buat database dan tabel di MySQL
3.	buat tabel dan isikan data


Untuk kode koneksi ke mysql seperti berikut
 
```golang
package main

import (
    "context"
    "fmt"
    "log"
    "time"

    "go.mongodb.org/mongo-driver/bson"
    "go.mongodb.org/mongo-driver/mongo"
    "go.mongodb.org/mongo-driver/mongo/options"
    "go.mongodb.org/mongo-driver/mongo/readpref"
)

func connect() (*mongo.Database, error) {
    clientOptions := options.Client()
    clientOptions.ApplyURI("mongodb://localhost:27017")
    client, err := mongo.NewClient(clientOptions)
    if err != nil {
        return nil, err
    }

    err = client.Connect(ctx)
    if err != nil {
        return nil, err
    }

    return client.Database("db_belajar_golang"), nil
```

Jalankan dengan ketik perintah “go run main.go
 
Masuk ke mongodb ketik “mongod”
 
Membuat database ketik use dbdica
 
 
 
Install driver mongoDB

 
```golang
package main

import (
    "context"
    "log"

    "go.mongodb.org/mongo-driver/mongo"
    "go.mongodb.org/mongo-driver/mongo/options"
    "go.mongodb.org/mongo-driver/mongo/readpref"
)

func GetClient() *mongo.Client {
    clientOptions := options.Client().ApplyURI("mongodb://localhost:27017")
    client, err := mongo.NewClient(clientOptions)
    if err != nil {
        log.Fatal(err)
    }
    err = client.Connect(context.Background())
    if err != nil {
        log.Fatal(err)
    }
    return client
}
func main() {
    c := GetClient()
    err := c.Ping(context.Background(), readpref.Primary())
    if err != nil {
        log.Fatal("Couldn't connect to the database", err)
    } else {
        log.Println("Connected!")
    }
}
```
Tampilan berhasil
 
Gin gonic
 

jalankan
 
Hasil running
 
 
API 
 


