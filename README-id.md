# fedora-id fork

## Purpose / Tujuan
### In English

This is a fork of <https://github.com/fedora-infra/asknot-ng/>, with
Indonesian questions aimed to direct newcomers to Indonesian-language
resources.

### Dalam Bahasa Indonesia

Ini fork dari <https://github.com/fedora-infra/asknot-ng/>, yang
menambahkan pertanyaan-pertanyaan dalam bahasa Indonesia untuk
mengarahkan orang baru ke sarana-sarana bantuan dalam bahasa
Indonesia.

## Contributing / Kontribusi

* [Fork and pull request guide][patches]

To ease the development workflow, it's advisable to create a feature
branch based on the `develop-id` branch, and submit a pull request
when you are ready. Rebase often to make sure your work can be merged
easily!

### Dalam Bahasa Indonesia

* [Pedoman forking dan pull request][patches]

Untuk mempermudah alur kerja, disarankan membuat feature branch yang
berdasarkan branch `develop-id`, dan mengirim pull request setelah
siap. Tolong melakukan rebase sesering mungkin untuk memastikan karya
Anda dapat di-merge balik secara mudah!

[patches]: https://help.github.com/articles/editing-files-in-another-user-s-repository/

## Pasang Dan Jalankan

Pasang pustaka yang dibutuhkan lebih dulu

```
$ pip install -r requirements.txt
```

Clone kode sumber dari repo

```
$ git clone https://github.com/fedora-id/asknot-ng.git
$ cd asknot-ng
```

Jalankan

```
$ ./asknot-ng.py templates/index.html questions/bantuan.yml --theme fedora
$ xdg-open asknot.html
```
