# Nomor Induk Kartu Tanda Penduduk (NIK KTP)

## General Contexts
- Last Reference Update: \
  24th May 2019 (by *PP Nomor 40 Tahun 2019*).
- Known keywords: \
  NIK, KTP, NIK KTP, Govt-issued ID.
- Issuer: \
  [Kementrian Dalam Negri (Kemendagri) \
  *Ministry of Home Affairs*](http://www.kemendagri.go.id/)

# Standard

NIK are a 16-digit number that doesn't have any separator. Those number consists
with following components:

- First 6 digits are called as *kode wilayah* (Regional Codes). \
  This notes where the ID issued from. The standard of this code can be checked on
  [`01-regional-codes`](./../1-regional-codes/).

- Next 6 digits are date of birth with date of month section also notes the sex
  of the ID holder. \
  DoB Format are: `DDMMYY` with following details:
  - `DD` is the date of month from the birth date, and add 40 if the holder's sex is female. \
    i.e Killua's birth date is 7th July 1987, the DoB section of the NIK will
    be 070787. Mariya's birth date is 25th September 1988, so the DoB section
    will be **65**0988 (25 + 40 = 65).
  - `MM` is the month of the birth date, padded with zero for month before October. \
    i.e 03 for March, 01 for January, 10 for October, etc.
  - `YY` is the last 2 digits of birth year. \
    i.e 19**98** = 98; 20**44** = 44.

- Next 4 digits are actual unique identifier for each holder, consisting of 4
  digits of number.

NIK number cannot be updated or changed if the data being updated or the holder
moves to another region[^1].

## Known Exceptions/Bugs/Etc

### Anomalies: 15 Digits Instead of The Standard 16 Digits
There's known 15 digit format generated from older SIAK (short for *Sistem
Informasi Administrasi Kependudukan*, translated as Information System for
Citizen Administration). As Indonesian Goverment tries to migrate to eKTP (from
KTP), this migration will invalidate the older 15 digits NIK.

**Fix:**\
Holder may request the NIK update by contacting holder's local Dinas Kependudukan dan
Sipil (Citizenship and Civil Service).


**References:**
- https://www.republika.co.id/berita/lpa7nt/september-785-ribu-warga-tangsel-dapat-nik-baru
- https://jateng.tribunnews.com/2016/11/14/nomor-kk-standarnya-16-digit-bagaimana-jika-ditemukan-hanya-10-angka-ini-fakta-di-dps-salatiga
- https://radartulungagung.jawapos.com/berita-daerah/trenggalek/13/09/2018/awas-nik-tak-valid


## Current Living Standard
- **Peraturan Pemerintah (PP) tentang Pelaksanaan Undang-undang Nomor 23 Tahun
  2006 tentang Administrasi Kependudukan Sebagaimana Telah Diubah dengan
  Undang-undang Nomor 24 Tahun 2013 tentang Perubahan atas Undang-undang Nomor
  23 Tahun 2006 tentang Administrasi Kependudukan** \
  References:
  - Peraturan.go.id Link: \
    https://peraturan.go.id/peraturan/view.html?id=c2c53bc5111538f6ac554a649d3c5027 \
    ([Wayback Machine](https://web.archive.org/web/*/https://peraturan.go.id/peraturan/view.html?id=c2c53bc5111538f6ac554a649d3c5027))
  - BPK (Audit Board of the Republic of Indonesia) link: \
    https://peraturan.bpk.go.id/Home/Details/108801/pp-no-40-tahun-2019 \
    ([Wayback Machine](https://web.archive.org/web/2021*/https://peraturan.bpk.go.id/Home/Details/108801/pp-no-40-tahun-2019))
  - Repo Archive: \
    [PP Nomor 40 Tahun 2019](./archives/PP%20Nomor%2040%20Tahun%202019.pdf)

## Old Standard(s)
- **Peraturan Pemerintah (PP) tentang Perubahan Atas Peraturan Pemerintah Nomor 37
  Tahun 2007 Tentang Pelaksanaan Undang Undang Nomor 23 Tahun 2006 Tentang
  Administrasi Kependudukan** \
  References:
  - Peraturan.go.id Link: \
    https://peraturan.go.id/peraturan/view.html?id=11e44c4f71705be0a034313232313231
    ([Wayback Machine](https://web.archive.org/web/*/https://peraturan.go.id/peraturan/view.html?id=11e44c4f71705be0a034313232313231))
  - BPK (Audit Board of the Republic of Indonesia) link: \
    https://peraturan.bpk.go.id/Home/Details/5317/pp-no-102-tahun-2012 \
    ([Wayback Machine
    Link](https://web.archive.org/web/*/https://peraturan.bpk.go.id/Home/Details/5317/pp-no-102-tahun-2012))
  - Repo Archive: \
    [PP Nomor 102 Tahun 2012](archives/PP%20Nomor%20102%20Tahun%202012.pdf)

- **Peraturan Pemerintah (PP) tentang Pelaksanaan Undang Undang Nomor 23 Tahun
  2006 Tentang Administrasi Kependudukan** \
  References:
  - Peraturan.go.id Link: \
    https://peraturan.go.id/peraturan/view.html?id=11e44c4f066ca940aa6e313231383232
    ([Wayback Machine](https://web.archive.org/web/*/https://peraturan.go.id/peraturan/view.html?id=11e44c4f066ca940aa6e313231383232))
  - BPK (Audit Board of the Republic of Indonesia) link: \
    https://peraturan.bpk.go.id/Home/Details/4759/pp-no-37-tahun-2007 \
    ([Wayback Machine
    Link](https://web.archive.org/web/*/https://peraturan.bpk.go.id/Home/Details/4759/pp-no-37-tahun-2007))
  - Repo Archive: \
    [PP 37 Tahun 2007](archives/PP%2037%20Tahun%202007.pdf)


[^1]: https://dukcapil.kemendagri.go.id/berita/baca/580/dirjen-dukcapil-jelaskan-beda-fungsi-nik-dan-nomor-kk
