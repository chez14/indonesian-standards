# Nomor Induk Kartu Tanda Penduduk (NIK KTP)

## General Contexts
- Last Reference Update: \
  24th May 2019 (by *PP Nomor 40 Tahun 2019*).
- Known keywords: \
  NIK, KTP, NIK KTP, Govt-issued ID.
- Issuer: \
  [Ministry of Home Affairs](http://www.kemendagri.go.id/)

# Standard

NIK are a 16-digit number that doesn't have any separator. Those number consists
with following components:

- First 6 digits are called as *kode wilayah* (Regional Codes). \
  This notes where the KTP issued from. The standard of this code can be checked on
  [`01-regional-codes`](./../1-regional-codes/).

- Next 6 digits are date of birth with date notes the sex of the ID holder. \
  DoB Format are: `YYMMDD` with following details:
  - `YY` is the last 2 digits of birth year. \
    i.e 19**98** = 98; 20**44** = 44.
  - `MM` is the month of the birth date, padded with zero for month before October. \
    i.e 03 for March, 01 for January, 10 for October, etc.
  - `DD` is the day of month from the birth date, and add 40 if the holder's sex is female. \
    i.e Killua Zoldyck's birth date is 7th July 1987, the DoB section of the NIK will
    be 870707. Mariya's birth date is 25th September 1988, so the DoB section
    will be 8809**65** (25 + 40 = 65).

- Next 4 digits are actual unique identifier for each holder, consisting of 4
  digits of number.

As noted from the reference, this number cannot be updated or changed while the
holder still alive as a human being even if the data being updated. However,
there's no details on how the NIK expire even if the holder is no longer alive.

## Known Exceptions/Bugs/Etc

[@chez14](https://github.com/chez14) has seen some of his friends that have 15
digits NIK. We don't actually know how often this exception occurs, but bear in
mind that this may happens.

## Current Living Standard
- **Peraturan Pemerintah (PP) tentang Pelaksanaan Undang-undang Nomor 23 Tahun
  2006 tentang Administrasi Kependudukan Sebagaimana Telah Diubah dengan
  Undang-undang Nomor 24 Tahun 2013 tentang Perubahan atas Undang-undang Nomor
  23 Tahun 2006 tentang Administrasi Kependudukan** \
  References:
  - Original link: \
    https://peraturan.bpk.go.id/Home/Details/108801/pp-no-40-tahun-2019 \
    ([Wayback Machine](https://web.archive.org/web/2021*/https://peraturan.bpk.go.id/Home/Details/108801/pp-no-40-tahun-2019))
  - Repo Archive: \
    [PP Nomor 40 Tahun 2019](./archives/PP%20Nomor%2040%20Tahun%202019.pdf)

## Old Standard(s)
- **Peraturan Pemerintah (PP) tentang Perubahan Atas Peraturan Pemerintah Nomor 37
  Tahun 2007 Tentang Pelaksanaan Undang Undang Nomor 23 Tahun 2006 Tentang
  Administrasi Kependudukan** \
  References:
  - Original link: \
    https://peraturan.bpk.go.id/Home/Details/5317/pp-no-102-tahun-2012 \
    ([Wayback Machine
    Link](https://web.archive.org/web/*/https://peraturan.bpk.go.id/Home/Details/5317/pp-no-102-tahun-2012))
  - Repo Archive: \
    [PP Nomor 102 Tahun 2012](archives/PP%20Nomor%20102%20Tahun%202012.pdf)

- **Peraturan Pemerintah (PP) tentang Pelaksanaan Undang Undang Nomor 23 Tahun
  2006 Tentang Administrasi Kependudukan** \
  References:
  - Original link: \
    https://peraturan.bpk.go.id/Home/Details/4759/pp-no-37-tahun-2007 \
    ([Wayback Machine
    Link](https://web.archive.org/web/*/https://peraturan.bpk.go.id/Home/Details/4759/pp-no-37-tahun-2007))
  - Repo Archive: \
    [PP 37 Tahun 2007](archives/PP%2037%20Tahun%202007.pdf)