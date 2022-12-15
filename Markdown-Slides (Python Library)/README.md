# Markdown-Slides (Python)
Library ini berguna untuk mengcompile file markdown menjadi slide slide presentasi

## Sebelum Menggunakan, sebelumnya komputer anda harus terinstall :
- python (minimal 3.8)
- GIT

## Install Library
Buka terminal anda kemudian ketikkan perintah berikut :
```
python -m pip install git+https://gitlab.com/da_doomer/markdown-slides.git
 
```

## Penggunaan
#### Untuk mengcompile file markdown menjadi slide slide presentasi bisa menggunakan perintah berikut :
```md
mdslides [-h] [--include RESOURCE] [--pdf] [--output_dir DIR] FILE

```
- #### mdslide file
  - Untuk mengcompile file md secara sederhana
    ```md
    mdslide ./namafile.md
    ```
  
- #### --include RESOURCE
  - Opsi RESOURCE digunakan untuk mengcompile RESOURCE yang digunakan untuk presentasi, contohnya seperti foto, video dll. Dimasukkan kedalam folder 
    ```md
    mdslide ./namafile.md --include namaFolder
    ```

- #### --output_dir DIR
  - Secara default output hasil compile akan dibuatkan folder dengan nama yang sama dengan nama file, penggunaan --output_dir memungkinkan kita untuk menempatkan hasil compile kedalam folder secara manual.
    ```md
    mdslide ./namafile.md --output_dir namaFolder
    ```


#### ini adalah CommonMark
```md
[comment]: # ("CommonMark") 
```
Syntax tersebut tidak akan terikut kedalam presentasi

#### Untuk menset tema presentasi bisa menggunakan perintah berikut :
```md
[comment]: # ("THEME = black") 
```
kumpulan tema bisa anda dilihat pada link berikut [link tema](https://revealjs.com/themes/)

#### Untuk menampilkan tombol kontrol pada presentasi  :
```md
[comment]: # ("controls: true")
```
Config lainnya bisa anda lihat [disini](https://revealjs.com/config/).

#### Gunakan ! tiga kali sebagai batas dari slide
```md
[comment]: # ("!!!")
```

#### Contoh Penggunaan Sederhana
- Buat 1 file berekstensi .md kemudian salin kode di bawah

    ```md
    # Ini adalah slide Pertama 
    [comment]: # ("!!!")
    # Ini adalah slide Kedua 
    ```
- Buka terminal kemudian compile.

# LaTex Math Syntax
Dalam markdown anda bisa menggunakan LaTex Math Syntax untuk membuat simbol simbol matematika dengan cara mengapit syntax LaTex dengan backtick 1 
```
`$$ J(\theta_0,\theta_1) = \sum_{i=0} $$`
```
Hasil presentasi akan menghasil simbol matematika.