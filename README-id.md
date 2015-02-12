# asknot-ng -- edisi Bantuan Fedora-ID

Program oleh [@ralphbean][threebean]. Terinspirasi [versi
semula][wcidfm] oleh [Josh Matthews][jdm], [Henri Koivuneva][wham],
dan [lainnya][asknot-contribs].

Rewrite ini lebih fleksibel dari versi awalnya. Script utama,
``asknot-ng.py``, berfungsi seperti static-site generator. Inputnya
terdiri dari tiga hal:

- File pertanyaan, ditulis dalam yaml (lihat
  [contoh][example-questions]) atau [file pertanyaan
  Fedora][fedora-questions]). Untuk situs Bantuan Fedora-ID gunakan
  [file pertanyaan Bantuan][fedora-id-bantuan].
- File template, ditulis dalam mako (template
  [default][default-template] seharusnya bisa dipakai semua orang).
- Argumen 'theme' menentukan CSS mana yang dipakai. Default-nya cukup
  menarik, Anda mungkin ingin membuat versi derivatif untuk keperluan
  Anda.

Untuk melihat hasil program ini, bisa melihat [situs versi Fedora][wcidff].

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

[threebean]: http://threebean.org
[fedora]: http://getfedora.org
[example-questions]: https://github.com/fedora-infra/asknot-ng/blob/develop/questions/example.yml
[fedora-questions]: https://github.com/fedora-infra/asknot-ng/blob/develop/questions/fedora.yml
[default-template]: https://github.com/fedora-infra/asknot-ng/blob/develop/templates/index.html
[requirements]: https://github.com/fedora-infra/asknot-ng/blob/develop/requirements.txt
[patches]: https://help.github.com/articles/editing-files-in-another-user-s-repository/
[wcidfm]: http://whatcanidoformozilla.org
[wcidff]: http://whatcanidoforfedora.org
[jdm]: http://www.joshmatthews.net
[wham]: http://wham.fi
[asknot-contribs]: https://github.com/jdm/asknot/contributors