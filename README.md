# MergedSymbolsKannada
Benchmarking dataset of merged symbols in Kannada along with their associated ground truth Unicode text

The [GroundTruthUnicode.txt](GroundTruthUnicode.txt) file contains the ground truth Unicode text for each of the test images in [TestImages](TestImages) folder.

The following conventions are used in Unicode representation:

A [zero-width non-joner (ZWNJ)](https://en.wikipedia.org/wiki/Zero-width_non-joiner) is used when a pure-consonant needs to be represented in un-modified form. For example,

  [214_P001_B5_L01_W06_C01.tif](TestImages/214_P001_B5_L01_W06_C01.tif): ಜೆಟ್‌ನಿ

When a vowel modifier such as `anusvara` or `vowel_sign_ii` appear at the beginning of the merged symbol sequence, the ground truth will have the Unicode of that depenent vowel at the beginning. For example:

  [214_P001_B5_L01_W06_C02.tif](TestImages/214_P001_B5_L01_W06_C02.tif): ಂದಾದ

  [214_P004_B3_L07_W03_C02.tif](TestImages/214_P004_B3_L07_W03_C02.tif) -> ೀಳುತಿದ

An exception to the above rule is for `arkaa ottu`, which for simplicity, is represented using Kannada digit nine (೯) in the ground truth. For example:

  [214_P003_B2_L02_W01_C02.tif](TestImages/214_P003_B2_L02_W01_C02.tif): ೯ಸಂ

