# Comparing `tmp/qepy-0.0.3.tar.gz` & `tmp/qepy-0.0.3rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qepy-0.0.3.tar", last modified: Sun Jun  4 21:50:20 2023, max compression
+gzip compressed data, was "qepy-0.0.3rc0.tar", last modified: Thu Apr 27 00:05:36 2023, max compression
```

## Comparing `qepy-0.0.3.tar` & `qepy-0.0.3rc0.tar`

### file list

```diff
@@ -1,258 +1,249 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.179441 qepy-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.143441 qepy-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-04 21:49:50.000000 qepy-0.0.3/.github/workflows/linux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-04 21:49:50.000000 qepy-0.0.3/.github/workflows/macos_arm64.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-04 21:49:50.000000 qepy-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-04 21:49:50.000000 qepy-0.0.3/.github/workflows/wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-04 21:49:50.000000 qepy-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-04 21:49:50.000000 qepy-0.0.3/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-04 21:49:50.000000 qepy-0.0.3/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-04 21:50:20.179441 qepy-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-04 21:49:50.000000 qepy-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/QEpy.bib
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/contact.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/doc/source/development/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/development/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/development/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/install.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/doc/source/qepy/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/qepy/calculator.rst
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/qepy/driver.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/qepy/io.rst
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/qepy/qepy.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/doc/source/static/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/doc/source/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/templates/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/templates/footer.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/doc/source/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.151441 qepy-0.0.3/doc/source/tutorials/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/tutorials/jupyter/dirac_exchange.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    87060 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/tutorials/jupyter/dos_band_graphene.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/tutorials/jupyter/qepy_scf.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/tutorials/jupyter/qepy_scf_iterative.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    17252 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/tutorials/jupyter/test_ecutwfc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23113 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/tutorials/jupyter/test_eos_vc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/tutorials/jupyter/test_kpoints.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/tutorials/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.151441 qepy-0.0.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.151441 qepy-0.0.3/examples/ase/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/ase/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/ase/qe_in.in
--rwxr-xr-x   0 runner    (1001) docker     (123)     1187 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/ase/test_ase_nvt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3360 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/ase/test_ase_scf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      140 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/clean.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.143441 qepy-0.0.3/examples/develop/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.151441 qepy-0.0.3/examples/develop/pw/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/develop/pw/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/develop/pw/qe_in.in
--rwxr-xr-x   0 runner    (1001) docker     (123)      508 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/develop/pw/scf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1024 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/develop/pw/test_pwscf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      946 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/develop/pw/test_pwscf_scf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      786 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/develop/pw/tmp2energy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1016 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/develop/pw/tmp2energy_pw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/examples/jupyter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.155441 qepy-0.0.3/examples/jupyter/DATA/
--rw-r--r--   0 runner    (1001) docker     (123)   964489 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/DATA/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/DATA/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)   264541 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/DATA/C.pbe-rrkjus.UPF
--rw-r--r--   0 runner    (1001) docker     (123)    64999 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/DATA/H_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)    90153 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/DATA/O_ONCV_PBE-1.2.upf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.155441 qepy-0.0.3/examples/jupyter/band/
--rw-r--r--   0 runner    (1001) docker     (123)   264541 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/band/C.pbe-rrkjus.UPF
--rw-r--r--   0 runner    (1001) docker     (123)    87060 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/band/dos_band_graphene.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.155441 qepy-0.0.3/examples/jupyter/colab/
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/colab/qepy_colab.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.155441 qepy-0.0.3/examples/jupyter/eos/
--rw-r--r--   0 runner    (1001) docker     (123)   964489 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/eos/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
--rw-r--r--   0 runner    (1001) docker     (123)    23324 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/eos/test_eos_slow.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23113 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/eos/test_eos_vc.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.155441 qepy-0.0.3/examples/jupyter/ext/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/ext/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/ext/dftpy_xc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/ext/dirac_exchange.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.155441 qepy-0.0.3/examples/jupyter/nvt/
--rw-r--r--   0 runner    (1001) docker     (123)    64999 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/nvt/H_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)    90153 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/nvt/O_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/nvt/ase_nvt.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/nvt/qe_in.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.159441 qepy-0.0.3/examples/jupyter/pp/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/pp/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/pp/pp.in
--rw-r--r--   0 runner    (1001) docker     (123)    33477 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/pp/qepy_elf_rdg.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/pp/qepy_parse_output.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    28575 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/pp/qepy_potentials.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.159441 qepy-0.0.3/examples/jupyter/scf/
--rw-r--r--   0 runner    (1001) docker     (123)   964489 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/scf/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/scf/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/scf/dftpy_mixer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/scf/qe_in.in
--rw-r--r--   0 runner    (1001) docker     (123)    20039 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/scf/qepy_iterative.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8394 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/scf/qepy_qeinput.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/scf/qepy_scf.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/scf/qepy_scf_iterative.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.159441 qepy-0.0.3/examples/jupyter/testing/
--rw-r--r--   0 runner    (1001) docker     (123)   964489 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/testing/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
--rw-r--r--   0 runner    (1001) docker     (123)    32639 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/testing/test_degauss.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    17252 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/testing/test_ecutwfc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/testing/test_kpoints.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/examples/opt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.163441 qepy-0.0.3/examples/opt/ase/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.163441 qepy-0.0.3/examples/opt/ase/out/
--rw-r--r--   0 runner    (1001) docker     (123)    74363 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/opt/ase/out/ase.out
--rw-r--r--   0 runner    (1001) docker     (123)    88204 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/opt/ase/out/qepy.out
--rw-r--r--   0 runner    (1001) docker     (123)   577736 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/opt/ase/si_pbe_v1.uspp.F.UPF
--rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/opt/ase/test_ase_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/opt/ase/vcrelax.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.163441 qepy-0.0.3/examples/opt/qe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.163441 qepy-0.0.3/examples/opt/qe/out/
--rw-r--r--   0 runner    (1001) docker     (123)    88204 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/opt/qe/out/qepy.out
--rw-r--r--   0 runner    (1001) docker     (123)    90822 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/opt/qe/out/ref.out
--rwxr-xr-x   0 runner    (1001) docker     (123)     2171 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/opt/qe/qe_relax.py
--rw-r--r--   0 runner    (1001) docker     (123)   577736 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/opt/qe/si_pbe_v1.uspp.F.UPF
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/opt/qe/vcrelax.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/examples/original/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.163441 qepy-0.0.3/examples/original/6.5/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/original/6.5/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/original/6.5/qe_in.in
--rwxr-xr-x   0 runner    (1001) docker     (123)      835 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/original/6.5/run_pwscf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.163441 qepy-0.0.3/examples/original/6.8/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/original/6.8/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/original/6.8/qe_in.in
--rwxr-xr-x   0 runner    (1001) docker     (123)      426 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/original/6.8/run_pwscf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.167441 qepy-0.0.3/examples/scf/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/scf/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/scf/qe_in.in
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/scf/test_pwscf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      708 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/scf/test_pwscf_iterative.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/scf/test_readfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      398 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/scf/test_readfile_pw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.167441 qepy-0.0.3/examples/tddft/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/tddft/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/tddft/qe_in.in
--rwxr-xr-x   0 runner    (1001) docker     (123)      743 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/tddft/test_ce_tddft.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/tddft/test_ce_tddft_restart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.167441 qepy-0.0.3/examples/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.167441 qepy-0.0.3/examples/test/DATA/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/al_md_3.traj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.167441 qepy-0.0.3/examples/test/DATA/oldxml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.167441 qepy-0.0.3/examples/test/DATA/oldxml/al_oldxml.save/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml/al_oldxml.save/Al_ONCV_PBE-1.2.upf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.167441 qepy-0.0.3/examples/test/DATA/oldxml/al_oldxml.save/K00001/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml/al_oldxml.save/K00001/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (123)   266316 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml/al_oldxml.save/charge-density.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml/al_oldxml.save/data-file.xml
--rw-r--r--   0 runner    (1001) docker     (123)   804960 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml/al_oldxml.wfc1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/examples/test/DATA/oldxml_collect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.167441 qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/Al_ONCV_PBE-1.2.upf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.171441 qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (123)   808502 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/evc.dat
--rw-r--r--   0 runner    (1001) docker     (123)    32091 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/gkvectors.dat
--rw-r--r--   0 runner    (1001) docker     (123)   266316 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/charge-density.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/data-file.xml
--rw-r--r--   0 runner    (1001) docker     (123)   185540 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/gvectors.dat
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/qe_fake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/qe_in.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.171441 qepy-0.0.3/examples/test/qe-6.5/
--rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/qe-6.5/test.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1799 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/qe-6.5/test_ce_tddft.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1613 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/qe-6.5/test_comm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1461 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/qe-6.5/test_oldxml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1360 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/qe-6.5/test_pwscf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1364 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/qe-6.5/test_pwscf_scf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2110 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/qe-6.5/test_readfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      715 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/test.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/test_ase_md.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1711 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/test_ce_tddft.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/test_oldxml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/test_pwscf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      972 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/test_pwscf_iterative.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1022 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/test_readfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.171441 qepy-0.0.3/install/
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-06-04 21:49:50.000000 qepy-0.0.3/install/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-04 21:49:50.000000 qepy-0.0.3/install/Makefile.cetddft
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-04 21:49:50.000000 qepy-0.0.3/install/kind_map.json
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-04 21:49:50.000000 qepy-0.0.3/install/make.depend
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-04 21:49:50.000000 qepy-0.0.3/install/make.depend.cetddft
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-04 21:49:50.000000 qepy-0.0.3/install/make.qe.inc
--rwxr-xr-x   0 runner    (1001) docker     (123)      274 2023-06-04 21:49:50.000000 qepy-0.0.3/install/makedeps.sh
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-04 21:49:50.000000 qepy-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.171441 qepy-0.0.3/qepy/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-04 21:49:50.000000 qepy-0.0.3/qepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 21:49:50.000000 qepy-0.0.3/qepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-04 21:49:50.000000 qepy-0.0.3/qepy/__new__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-06-04 21:49:50.000000 qepy-0.0.3/qepy/calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-04 21:49:50.000000 qepy-0.0.3/qepy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.171441 qepy-0.0.3/qepy/cui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 21:49:50.000000 qepy-0.0.3/qepy/cui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-04 21:49:50.000000 qepy-0.0.3/qepy/cui/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-04 21:49:50.000000 qepy-0.0.3/qepy/cui/pwx.py
--rw-r--r--   0 runner    (1001) docker     (123)    35135 2023-06-04 21:49:50.000000 qepy-0.0.3/qepy/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-06-04 21:49:50.000000 qepy-0.0.3/qepy/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.171441 qepy-0.0.3/qepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-04 21:50:20.000000 qepy-0.0.3/qepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-06-04 21:50:20.000000 qepy-0.0.3/qepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 21:50:20.000000 qepy-0.0.3/qepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 21:50:19.000000 qepy-0.0.3/qepy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-04 21:50:20.000000 qepy-0.0.3/qepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-04 21:50:20.000000 qepy-0.0.3/qepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 21:50:20.179441 qepy-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-06-04 21:49:50.000000 qepy-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.171441 qepy-0.0.3/src/api/
--rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-06-04 21:49:50.000000 qepy-0.0.3/src/api/qepy_common.f90
--rw-r--r--   0 runner    (1001) docker     (123)    26027 2023-06-04 21:49:50.000000 qepy-0.0.3/src/api/qepy_mod.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.175441 qepy-0.0.3/src/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-06-04 21:49:50.000000 qepy-0.0.3/src/cmd/command_line_options.f90
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-04 21:49:50.000000 qepy-0.0.3/src/cmd/pwscf.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.175441 qepy-0.0.3/src/fix/
--rw-r--r--   0 runner    (1001) docker     (123)    66035 2023-06-04 21:49:50.000000 qepy-0.0.3/src/fix/funct.f90
--rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-06-04 21:49:50.000000 qepy-0.0.3/src/fix/potinit.f90
--rw-r--r--   0 runner    (1001) docker     (123)    56596 2023-06-04 21:49:50.000000 qepy-0.0.3/src/fix/pw_restart_new.f90
--rw-r--r--   0 runner    (1001) docker     (123)   360829 2023-06-04 21:49:50.000000 qepy-0.0.3/src/fix/qes_read_module.f90
--rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-06-04 21:49:50.000000 qepy-0.0.3/src/fix/read_file_new.f90
--rw-r--r--   0 runner    (1001) docker     (123)    50735 2023-06-04 21:49:50.000000 qepy-0.0.3/src/fix/scatter_mod.f90
--rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-06-04 21:49:50.000000 qepy-0.0.3/src/fix/wfcinit.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.175441 qepy-0.0.3/src/ldau/
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-04 21:49:50.000000 qepy-0.0.3/src/ldau/qepy_econf.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)     6276 2023-06-04 21:49:50.000000 qepy-0.0.3/src/ldau/qepy_ldau_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.175441 qepy-0.0.3/src/oldxml/
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-06-04 21:49:50.000000 qepy-0.0.3/src/oldxml/oldxml_io_rho_xml.f90
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-06-04 21:49:50.000000 qepy-0.0.3/src/oldxml/oldxml_potinit.f90
--rw-r--r--   0 runner    (1001) docker     (123)   105084 2023-06-04 21:49:50.000000 qepy-0.0.3/src/oldxml/oldxml_pw_restart.f90
--rw-r--r--   0 runner    (1001) docker     (123)   176393 2023-06-04 21:49:50.000000 qepy-0.0.3/src/oldxml/oldxml_qexml.f90
--rw-r--r--   0 runner    (1001) docker     (123)    17352 2023-06-04 21:49:50.000000 qepy-0.0.3/src/oldxml/oldxml_read_file.f90
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-06-04 21:49:50.000000 qepy-0.0.3/src/oldxml/oldxml_wfcinit.f90
--rw-r--r--   0 runner    (1001) docker     (123)    40621 2023-06-04 21:49:50.000000 qepy-0.0.3/src/oldxml/oldxml_xml_io_base.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.175441 qepy-0.0.3/src/qe/
--rw-r--r--   0 runner    (1001) docker     (123)    61363 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_electrons.f90
--rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_electrons_nscf.f90
--rw-r--r--   0 runner    (1001) docker     (123)    14880 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_forces.f90
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_hinit1.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_init_run.f90
--rw-r--r--   0 runner    (1001) docker     (123)    61917 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_pw2casino_write.f90
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_pwscf.f90
--rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_run_pwscf.f90
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_setlocal.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_stop_run.f90
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_stress.f90
--rw-r--r--   0 runner    (1001) docker     (123)    38870 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_v_of_rho.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.179441 qepy-0.0.3/src/tddft/
--rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-06-04 21:49:50.000000 qepy-0.0.3/src/tddft/qepy_molecule_optical_absorption.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-04 21:49:50.000000 qepy-0.0.3/src/tddft/qepy_tddft_common.f90
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-06-04 21:49:50.000000 qepy-0.0.3/src/tddft/qepy_tddft_main.f90
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-04 21:49:50.000000 qepy-0.0.3/src/tddft/qepy_tddft_mod.f90
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-06-04 21:49:50.000000 qepy-0.0.3/src/tddft/qepy_tddft_routines.f90
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-06-04 21:49:50.000000 qepy-0.0.3/src/tddft/qepy_tddft_setup.f90
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-06-04 21:49:50.000000 qepy-0.0.3/src/tddft/qepy_update_ham.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.770805 qepy-0.0.3rc0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.674802 qepy-0.0.3rc0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.690802 qepy-0.0.3rc0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/.github/workflows/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/.github/workflows/wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-27 00:05:36.766805 qepy-0.0.3rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.690802 qepy-0.0.3rc0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.690802 qepy-0.0.3rc0/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/QEpy.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/contact.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.694802 qepy-0.0.3rc0/doc/source/development/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/development/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/development/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/install.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.694802 qepy-0.0.3rc0/doc/source/qepy/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/qepy/calculator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/qepy/driver.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/qepy/io.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/qepy/qepy.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.694802 qepy-0.0.3rc0/doc/source/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.694802 qepy-0.0.3rc0/doc/source/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/templates/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/templates/footer.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.694802 qepy-0.0.3rc0/doc/source/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.698803 qepy-0.0.3rc0/doc/source/tutorials/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/tutorials/jupyter/dirac_exchange.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    87060 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/tutorials/jupyter/dos_band_graphene.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/tutorials/jupyter/qepy_scf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/tutorials/jupyter/qepy_scf_iterative.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    17252 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/tutorials/jupyter/test_ecutwfc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23113 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/tutorials/jupyter/test_eos_vc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/tutorials/jupyter/test_kpoints.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/tutorials/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.698803 qepy-0.0.3rc0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.698803 qepy-0.0.3rc0/examples/ase/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/ase/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/ase/qe_in.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1187 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/ase/test_ase_nvt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3360 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/ase/test_ase_scf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      140 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/clean.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.678802 qepy-0.0.3rc0/examples/develop/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.702803 qepy-0.0.3rc0/examples/develop/pw/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/develop/pw/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/develop/pw/qe_in.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)      508 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/develop/pw/scf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1024 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/develop/pw/test_pwscf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      946 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/develop/pw/test_pwscf_scf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      786 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/develop/pw/tmp2energy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1016 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/develop/pw/tmp2energy_pw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.678802 qepy-0.0.3rc0/examples/jupyter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.706803 qepy-0.0.3rc0/examples/jupyter/DATA/
+-rw-r--r--   0 runner    (1001) docker     (123)   964489 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/DATA/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/DATA/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)   264541 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/DATA/C.pbe-rrkjus.UPF
+-rw-r--r--   0 runner    (1001) docker     (123)    64999 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/DATA/H_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)    90153 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/DATA/O_ONCV_PBE-1.2.upf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.706803 qepy-0.0.3rc0/examples/jupyter/band/
+-rw-r--r--   0 runner    (1001) docker     (123)   264541 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/band/C.pbe-rrkjus.UPF
+-rw-r--r--   0 runner    (1001) docker     (123)    87060 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/band/dos_band_graphene.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.706803 qepy-0.0.3rc0/examples/jupyter/colab/
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/colab/qepy_colab.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.710803 qepy-0.0.3rc0/examples/jupyter/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)   964489 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/eos/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
+-rw-r--r--   0 runner    (1001) docker     (123)    23324 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/eos/test_eos_slow.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23113 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/eos/test_eos_vc.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.710803 qepy-0.0.3rc0/examples/jupyter/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/ext/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/ext/dftpy_xc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/ext/dirac_exchange.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.714803 qepy-0.0.3rc0/examples/jupyter/nvt/
+-rw-r--r--   0 runner    (1001) docker     (123)    64999 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/nvt/H_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)    90153 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/nvt/O_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/nvt/ase_nvt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/nvt/qe_in.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.714803 qepy-0.0.3rc0/examples/jupyter/pp/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/pp/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/pp/pp.in
+-rw-r--r--   0 runner    (1001) docker     (123)    33477 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/pp/qepy_elf_rdg.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/pp/qepy_parse_output.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    28575 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/pp/qepy_potentials.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.718803 qepy-0.0.3rc0/examples/jupyter/scf/
+-rw-r--r--   0 runner    (1001) docker     (123)   964489 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/scf/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/scf/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/scf/dftpy_mixer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/scf/qe_in.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20039 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/scf/qepy_iterative.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8394 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/scf/qepy_qeinput.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/scf/qepy_scf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/scf/qepy_scf_iterative.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.722803 qepy-0.0.3rc0/examples/jupyter/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)   964489 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/testing/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
+-rw-r--r--   0 runner    (1001) docker     (123)    32639 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/testing/test_degauss.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    17252 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/testing/test_ecutwfc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/testing/test_kpoints.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.678802 qepy-0.0.3rc0/examples/opt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.722803 qepy-0.0.3rc0/examples/opt/ase/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.726804 qepy-0.0.3rc0/examples/opt/ase/out/
+-rw-r--r--   0 runner    (1001) docker     (123)    74363 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/opt/ase/out/ase.out
+-rw-r--r--   0 runner    (1001) docker     (123)    88204 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/opt/ase/out/qepy.out
+-rw-r--r--   0 runner    (1001) docker     (123)   577736 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/opt/ase/si_pbe_v1.uspp.F.UPF
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/opt/ase/test_ase_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/opt/ase/vcrelax.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.726804 qepy-0.0.3rc0/examples/opt/qe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.726804 qepy-0.0.3rc0/examples/opt/qe/out/
+-rw-r--r--   0 runner    (1001) docker     (123)    88204 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/opt/qe/out/qepy.out
+-rw-r--r--   0 runner    (1001) docker     (123)    90822 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/opt/qe/out/ref.out
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2171 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/opt/qe/qe_relax.py
+-rw-r--r--   0 runner    (1001) docker     (123)   577736 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/opt/qe/si_pbe_v1.uspp.F.UPF
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/opt/qe/vcrelax.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.682802 qepy-0.0.3rc0/examples/original/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.730804 qepy-0.0.3rc0/examples/original/6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/original/6.5/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/original/6.5/qe_in.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)      835 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/original/6.5/run_pwscf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.730804 qepy-0.0.3rc0/examples/original/6.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/original/6.8/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/original/6.8/qe_in.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)      426 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/original/6.8/run_pwscf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.734804 qepy-0.0.3rc0/examples/scf/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/scf/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/scf/qe_in.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/scf/test_pwscf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      708 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/scf/test_pwscf_iterative.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/scf/test_readfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      398 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/scf/test_readfile_pw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.734804 qepy-0.0.3rc0/examples/tddft/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/tddft/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/tddft/qe_in.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)      743 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/tddft/test_ce_tddft.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/tddft/test_ce_tddft_restart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.734804 qepy-0.0.3rc0/examples/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.738804 qepy-0.0.3rc0/examples/test/DATA/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/al_md_3.traj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.738804 qepy-0.0.3rc0/examples/test/DATA/oldxml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.742804 qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.save/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.save/Al_ONCV_PBE-1.2.upf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.742804 qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.save/K00001/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.save/K00001/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   266316 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.save/charge-density.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.save/data-file.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   804960 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.wfc1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.682802 qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.742804 qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/Al_ONCV_PBE-1.2.upf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.746804 qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   808502 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    32091 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/gkvectors.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   266316 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/charge-density.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/data-file.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   185540 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/gvectors.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/qe_fake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/qe_in.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.750805 qepy-0.0.3rc0/examples/test/qe-6.5/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/qe-6.5/test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1799 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/qe-6.5/test_ce_tddft.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1613 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/qe-6.5/test_comm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1461 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/qe-6.5/test_oldxml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1360 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/qe-6.5/test_pwscf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1364 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/qe-6.5/test_pwscf_scf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2110 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/qe-6.5/test_readfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      715 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/test_ase_md.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1711 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/test_ce_tddft.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/test_oldxml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/test_pwscf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      972 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/test_pwscf_iterative.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1022 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/test_readfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.750805 qepy-0.0.3rc0/install/
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/install/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/install/Makefile.cetddft
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/install/kind_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/install/make.depend
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/install/make.depend.cetddft
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/install/make.qe.inc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      274 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/install/makedeps.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.754804 qepy-0.0.3rc0/qepy/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/qepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/qepy/__new__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/qepy/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/qepy/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34766 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/qepy/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/qepy/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.754804 qepy-0.0.3rc0/qepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-27 00:05:36.000000 qepy-0.0.3rc0/qepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-27 00:05:36.000000 qepy-0.0.3rc0/qepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 00:05:36.000000 qepy-0.0.3rc0/qepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 00:05:36.000000 qepy-0.0.3rc0/qepy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-27 00:05:36.000000 qepy-0.0.3rc0/qepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-27 00:05:36.000000 qepy-0.0.3rc0/qepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 00:05:36.770805 qepy-0.0.3rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.686802 qepy-0.0.3rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.754804 qepy-0.0.3rc0/src/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/api/qepy_common.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    26027 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/api/qepy_mod.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.758805 qepy-0.0.3rc0/src/fix/
+-rw-r--r--   0 runner    (1001) docker     (123)    66035 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/fix/funct.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/fix/potinit.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    56596 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/fix/pw_restart_new.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   360829 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/fix/qes_read_module.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/fix/read_file_new.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    50735 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/fix/scatter_mod.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/fix/wfcinit.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.758805 qepy-0.0.3rc0/src/ldau/
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/ldau/qepy_econf.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6276 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/ldau/qepy_ldau_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.762805 qepy-0.0.3rc0/src/oldxml/
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/oldxml/oldxml_io_rho_xml.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/oldxml/oldxml_potinit.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   105084 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/oldxml/oldxml_pw_restart.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   176393 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/oldxml/oldxml_qexml.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    17352 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/oldxml/oldxml_read_file.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/oldxml/oldxml_wfcinit.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    40621 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/oldxml/oldxml_xml_io_base.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.766805 qepy-0.0.3rc0/src/qe/
+-rw-r--r--   0 runner    (1001) docker     (123)    61363 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_electrons.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_electrons_nscf.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    14880 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_forces.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_hinit1.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_init_run.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    61917 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_pw2casino_write.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_pwscf.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_run_pwscf.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_setlocal.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_stop_run.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_stress.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    38870 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_v_of_rho.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.766805 qepy-0.0.3rc0/src/tddft/
+-rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/tddft/qepy_molecule_optical_absorption.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/tddft/qepy_tddft_common.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/tddft/qepy_tddft_main.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/tddft/qepy_tddft_mod.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/tddft/qepy_tddft_routines.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/tddft/qepy_tddft_setup.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/tddft/qepy_update_ham.f90
```

### Comparing `qepy-0.0.3/.github/workflows/linux.yml` & `qepy-0.0.3rc0/.github/workflows/linux.yml`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/.github/workflows/macos_arm64.yml` & `qepy-0.0.3rc0/.github/workflows/wheels.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,97 @@
-name: Build wheels on Macos-arm64
+name: Build wheels
 
 on:
   push:
     branches:
-      - action
+      - github
+    paths-ignore:
+      - '.github/workflows/publish.yml'
   pull_request:
     branches:
-      - action
+      - github
 
 jobs:
-  build_wheels_macos_arm64:
+  build_wheels:
     name: Build wheel for ${{ matrix.python }}-${{ matrix.buildplat[1] }}-${{ matrix.buildplat[2] }}
     runs-on: ${{ matrix.buildplat[0] }}
     strategy:
       fail-fast: false
       matrix:
         buildplat:
+        - [ubuntu-20.04, manylinux, x86_64]
+        - [macos-latest, macosx, x86_64]
         - [macos-12, macosx, arm64]
-        python: ["cp39"]
+        python: ["cp37", "cp38", "cp39", "cp310", "cp311"]
+        exclude:
+        - buildplat: [macos-12, macosx, arm64]
+          python: "cp37"
     steps:
       - name: Checkout repo
         uses: actions/checkout@v3
         with:
           submodules: recursive
 
       - name: Set up Python
         uses: actions/setup-python@v3
         with:
           python-version: '3.x'
 
+      - name: Build wheels on linux
+        if: ${{ matrix.buildplat[1] == 'manylinux' }}
+        uses: pypa/cibuildwheel@v2.12.1
+        env:
+          CIBW_BUILD: ${{ matrix.python }}-${{ matrix.buildplat[1] }}*
+          CIBW_ENVIRONMENT: FFLAGS='-fPIC -fallow-argument-mismatch' oldxml=yes SETUPTOOLS_USE_DISTUTILS=stdlib
+          CIBW_ENVIRONMENT_PASS_LINUX: FFLAGS oldxml SETUPTOOLS_USE_DISTUTILS
+          CIBW_ARCHS_LINUX: "auto"
+          CIBW_BEFORE_BUILD: |
+            yum install -y blas-devel lapack-devel fftw-devel
+
+      - name: Build wheels on macos
+        if: ${{ matrix.buildplat[1] == 'macosx' && matrix.buildplat[2] == 'x86_64' }}
+        uses: pypa/cibuildwheel@v2.12.1
+        env:
+          CIBW_BUILD: ${{ matrix.python }}-${{ matrix.buildplat[1] }}*
+          CIBW_ENVIRONMENT: FFLAGS='-fPIC -fallow-argument-mismatch' oldxml=yes SETUPTOOLS_USE_DISTUTILS=stdlib
+          CIBW_ENVIRONMENT_PASS_LINUX: FFLAGS oldxml SETUPTOOLS_USE_DISTUTILS
+          CIBW_ARCHS_MACOS: "x86_64"
+          CIBW_BEFORE_BUILD: |
+            brew install gfortran && brew unlink gfortran && brew link gfortran
+            brew install openblas lapack
+
       - name: Build wheels on macos_arm64
         if: ${{ matrix.buildplat[1] == 'macosx' && matrix.buildplat[2] == 'arm64' }}
-        uses: pypa/cibuildwheel@v2.12.3
+        uses: pypa/cibuildwheel@v2.12.1
         env:
           CIBW_BUILD: ${{ matrix.python }}-${{ matrix.buildplat[1] }}*
-          CIBW_BUILD_VERBOSITY: 3
-          CIBW_ENVIRONMENT: FFLAGS='-fPIC -fallow-argument-mismatch' oldxml=yes SETUPTOOLS_USE_DISTUTILS=stdlib QE_INSTALL_FLAGS='--host=host' NPY_DISTUTILS_APPEND_FLAGS=1 MACOSX_DEPLOYMENT_TARGET=11.0 LDFLAGS='-L/usr/local/lib/libdir -Wl,-rpath,/usr/local/lib/libdir -arch x86_64' SDKROOT=/Applications/Xcode_14.2.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX.sdk build_alias=arm-apple-darwin20.0.0 host_alias=x86_64-unknown-linux-gnu CFLAGS='-fPIC -arch arm64'
+          CIBW_ENVIRONMENT: FFLAGS='-fPIC -fallow-argument-mismatch' oldxml=yes SETUPTOOLS_USE_DISTUTILS=stdlib QE_INSTALL_FLAGS='--host=host' NPY_DISTUTILS_APPEND_FLAGS=1 MACOSX_DEPLOYMENT_TARGET=11.0 LDFLAGS='-L/usr/local/lib/libdir -Wl,-rpath,/usr/local/lib/libdir -arch x86_64' SDKROOT=/Applications/Xcode_13.2.1.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX12.1.sdk build_alias=arm-apple-darwin20.0.0 host_alias=x86_64-unknown-linux-gnu CFLAGS='-fPIC -arch arm64'
           CIBW_ENVIRONMENT_PASS_LINUX: FFLAGS oldxml SETUPTOOLS_USE_DISTUTILS QE_INSTALL_FLAGS NPY_DISTUTILS_APPEND_FLAGS MACOSX_DEPLOYMENT_TARGET SDKROOT LDFLAGS build_alias host_alias CFLAGS
           CIBW_ARCHS_MACOS: "arm64"
           CIBW_BEFORE_BUILD: |
             #
             brew install openblas lapack
             #
-            curl -L -O https://github.com/isuruf/gcc/releases/download/gcc-10-arm-20210728/gfortran-darwin-arm64.tar.gz
-            export GFORTRAN_SHA=4a1354e61294d5163609e83b6b2b082bd9a9bbdf
+            curl -L -O https://github.com/isuruf/gcc/releases/download/gcc-10-arm-20210228/gfortran-darwin-arm64.tar.gz
+            export GFORTRAN_SHA=f26990f6f08e19b2ec150b9da9d59bd0558261dd
             if [[ "$(shasum gfortran-darwin-arm64.tar.gz)" != "${GFORTRAN_SHA}  gfortran-darwin-arm64.tar.gz" ]]; then
                 echo "shasum mismatch for gfortran-darwin-arm64"
                 exit 1
             fi
             sudo mkdir -p /opt/
             sudo cp "gfortran-darwin-arm64.tar.gz" /opt/gfortran-darwin-arm64.tar.gz
             pushd /opt
                 sudo tar -xvf gfortran-darwin-arm64.tar.gz
                 sudo rm gfortran-darwin-arm64.tar.gz
             popd
             FC_ARM64="$(find /opt/gfortran-darwin-arm64/bin -name "*-gfortran")"
-            libgfortran="$(find /opt/gfortran-darwin-arm64/lib -name "libgfortran.dylib")"
+            libgfortran="$(find /opt/gfortran-darwin-arm64/lib -name libgfortran.dylib)"
             libdir=$(dirname $libgfortran)
             FC_ARM64_LDFLAGS="-L$libdir -Wl,-rpath,$libdir"
             #
             sudo ln -s $FC_ARM64 /usr/local/bin/gfortran
             sudo ln -s $libdir /usr/local/lib/libdir
-            echo ${SDKROOT:-$(xcrun --show-sdk-path)}
             #
-            #gfortran -v
-            #export FFLAGS='-fPIC -fallow-argument-mismatch' oldxml=yes SETUPTOOLS_USE_DISTUTILS=stdlib QE_INSTALL_FLAGS='--host=host' NPY_DISTUTILS_APPEND_FLAGS=1 MACOSX_DEPLOYMENT_TARGET=11.0 LDFLAGS='-L/usr/local/lib/libdir -Wl,-rpath,/usr/local/lib/libdir -arch x86_64' SDKROOT=${SDKROOT:-$(xcrun --show-sdk-path)} build_alias=arm-apple-darwin20.0.0 host_alias=x86_64-unknown-linux-gnu CFLAGS='-fPIC -arch arm64'
-            #python -m pip install setuptools==59.8.0 f90wrap==0.2.11 oldest-supported-numpy
-            #ls *
-            #python setup.py build
       - uses: actions/upload-artifact@v3
         with:
           name: qepy-wheels
           path: ./wheelhouse/*.whl
```

### Comparing `qepy-0.0.3/.github/workflows/publish.yml` & `qepy-0.0.3rc0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/.gitlab-ci.yml` & `qepy-0.0.3rc0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/PKG-INFO` & `qepy-0.0.3rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qepy
-Version: 0.0.3
+Version: 0.0.3rc0
 Summary: QEpy: Quantum ESPRESSO Python interface
 Home-page: https://gitlab.com/shaoxc/qepy
 Author: Pavanello Research Group
 Author-email: m.pavanello@rutgers.edu
 License: GPL
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `qepy-0.0.3/README.md` & `qepy-0.0.3rc0/README.md`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/doc/Makefile` & `qepy-0.0.3rc0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/doc/make.bat` & `qepy-0.0.3rc0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/doc/source/QEpy.bib` & `qepy-0.0.3rc0/doc/source/QEpy.bib`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/doc/source/conf.py` & `qepy-0.0.3rc0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/doc/source/contact.rst` & `qepy-0.0.3rc0/doc/source/contact.rst`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/doc/source/development/documentation.rst` & `qepy-0.0.3rc0/doc/source/development/documentation.rst`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/doc/source/faq.rst` & `qepy-0.0.3rc0/doc/source/faq.rst`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/doc/source/index.rst` & `qepy-0.0.3rc0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/doc/source/install.rst` & `qepy-0.0.3rc0/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/doc/source/qepy/calculator.rst` & `qepy-0.0.3rc0/doc/source/qepy/calculator.rst`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/doc/source/templates/breadcrumbs.html` & `qepy-0.0.3rc0/doc/source/templates/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/doc/source/templates/footer.html` & `qepy-0.0.3rc0/doc/source/templates/footer.html`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/doc/source/tutorials/jupyter/dirac_exchange.ipynb` & `qepy-0.0.3rc0/doc/source/tutorials/jupyter/dirac_exchange.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/doc/source/tutorials/jupyter/dos_band_graphene.ipynb` & `qepy-0.0.3rc0/doc/source/tutorials/jupyter/dos_band_graphene.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/doc/source/tutorials/jupyter/qepy_scf.ipynb` & `qepy-0.0.3rc0/doc/source/tutorials/jupyter/qepy_scf.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/doc/source/tutorials/jupyter/qepy_scf_iterative.ipynb` & `qepy-0.0.3rc0/doc/source/tutorials/jupyter/qepy_scf_iterative.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/doc/source/tutorials/jupyter/test_ecutwfc.ipynb` & `qepy-0.0.3rc0/doc/source/tutorials/jupyter/test_ecutwfc.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/doc/source/tutorials/jupyter/test_eos_vc.ipynb` & `qepy-0.0.3rc0/doc/source/tutorials/jupyter/test_eos_vc.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/doc/source/tutorials/jupyter/test_kpoints.ipynb` & `qepy-0.0.3rc0/doc/source/tutorials/jupyter/test_kpoints.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/ase/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/ase/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/ase/qe_in.in` & `qepy-0.0.3rc0/examples/ase/qe_in.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/ase/test_ase_nvt.py` & `qepy-0.0.3rc0/examples/ase/test_ase_nvt.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/ase/test_ase_scf.py` & `qepy-0.0.3rc0/examples/ase/test_ase_scf.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/develop/pw/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/develop/pw/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/develop/pw/qe_in.in` & `qepy-0.0.3rc0/examples/develop/pw/qe_in.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/develop/pw/test_pwscf.py` & `qepy-0.0.3rc0/examples/develop/pw/test_pwscf.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/develop/pw/test_pwscf_scf.py` & `qepy-0.0.3rc0/examples/develop/pw/test_pwscf_scf.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/develop/pw/tmp2energy.py` & `qepy-0.0.3rc0/examples/develop/pw/tmp2energy.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/develop/pw/tmp2energy_pw.py` & `qepy-0.0.3rc0/examples/develop/pw/tmp2energy_pw.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/DATA/Al.pbe-nl-kjpaw_psl.1.0.0.UPF` & `qepy-0.0.3rc0/examples/jupyter/DATA/Al.pbe-nl-kjpaw_psl.1.0.0.UPF`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/DATA/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/jupyter/DATA/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/DATA/C.pbe-rrkjus.UPF` & `qepy-0.0.3rc0/examples/jupyter/DATA/C.pbe-rrkjus.UPF`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/DATA/H_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/jupyter/DATA/H_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/DATA/O_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/jupyter/DATA/O_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/band/C.pbe-rrkjus.UPF` & `qepy-0.0.3rc0/examples/jupyter/band/C.pbe-rrkjus.UPF`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/band/dos_band_graphene.ipynb` & `qepy-0.0.3rc0/examples/jupyter/band/dos_band_graphene.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/colab/qepy_colab.ipynb` & `qepy-0.0.3rc0/examples/jupyter/colab/qepy_colab.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/eos/Al.pbe-nl-kjpaw_psl.1.0.0.UPF` & `qepy-0.0.3rc0/examples/jupyter/eos/Al.pbe-nl-kjpaw_psl.1.0.0.UPF`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/eos/test_eos_slow.ipynb` & `qepy-0.0.3rc0/examples/jupyter/eos/test_eos_slow.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/eos/test_eos_vc.ipynb` & `qepy-0.0.3rc0/examples/jupyter/eos/test_eos_vc.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/ext/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/jupyter/ext/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/ext/dftpy_xc.ipynb` & `qepy-0.0.3rc0/examples/jupyter/ext/dftpy_xc.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/ext/dirac_exchange.ipynb` & `qepy-0.0.3rc0/examples/jupyter/ext/dirac_exchange.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/nvt/H_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/jupyter/nvt/H_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/nvt/O_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/jupyter/nvt/O_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/nvt/ase_nvt.ipynb` & `qepy-0.0.3rc0/examples/jupyter/nvt/ase_nvt.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/nvt/qe_in.in` & `qepy-0.0.3rc0/examples/jupyter/nvt/qe_in.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/pp/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/jupyter/pp/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/pp/qepy_elf_rdg.ipynb` & `qepy-0.0.3rc0/examples/jupyter/pp/qepy_elf_rdg.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/pp/qepy_parse_output.ipynb` & `qepy-0.0.3rc0/examples/jupyter/pp/qepy_parse_output.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/pp/qepy_potentials.ipynb` & `qepy-0.0.3rc0/examples/jupyter/pp/qepy_potentials.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/scf/Al.pbe-nl-kjpaw_psl.1.0.0.UPF` & `qepy-0.0.3rc0/examples/jupyter/scf/Al.pbe-nl-kjpaw_psl.1.0.0.UPF`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/scf/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/jupyter/scf/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/scf/dftpy_mixer.ipynb` & `qepy-0.0.3rc0/examples/jupyter/scf/dftpy_mixer.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/scf/qe_in.in` & `qepy-0.0.3rc0/examples/jupyter/scf/qe_in.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/scf/qepy_iterative.ipynb` & `qepy-0.0.3rc0/examples/jupyter/scf/qepy_iterative.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/scf/qepy_qeinput.ipynb` & `qepy-0.0.3rc0/examples/jupyter/scf/qepy_qeinput.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/scf/qepy_scf.ipynb` & `qepy-0.0.3rc0/examples/jupyter/scf/qepy_scf.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/scf/qepy_scf_iterative.ipynb` & `qepy-0.0.3rc0/examples/jupyter/scf/qepy_scf_iterative.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/testing/Al.pbe-nl-kjpaw_psl.1.0.0.UPF` & `qepy-0.0.3rc0/examples/jupyter/testing/Al.pbe-nl-kjpaw_psl.1.0.0.UPF`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/testing/test_degauss.ipynb` & `qepy-0.0.3rc0/examples/jupyter/testing/test_degauss.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/testing/test_ecutwfc.ipynb` & `qepy-0.0.3rc0/examples/jupyter/testing/test_ecutwfc.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/jupyter/testing/test_kpoints.ipynb` & `qepy-0.0.3rc0/examples/jupyter/testing/test_kpoints.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/opt/ase/out/ase.out` & `qepy-0.0.3rc0/examples/opt/ase/out/ase.out`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/opt/ase/out/qepy.out` & `qepy-0.0.3rc0/examples/opt/ase/out/qepy.out`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/opt/ase/si_pbe_v1.uspp.F.UPF` & `qepy-0.0.3rc0/examples/opt/ase/si_pbe_v1.uspp.F.UPF`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/opt/ase/test_ase_opt.py` & `qepy-0.0.3rc0/examples/opt/ase/test_ase_opt.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/opt/ase/vcrelax.in` & `qepy-0.0.3rc0/examples/opt/ase/vcrelax.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/opt/qe/out/qepy.out` & `qepy-0.0.3rc0/examples/opt/qe/out/qepy.out`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/opt/qe/out/ref.out` & `qepy-0.0.3rc0/examples/opt/qe/out/ref.out`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/opt/qe/qe_relax.py` & `qepy-0.0.3rc0/examples/opt/qe/qe_relax.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/opt/qe/si_pbe_v1.uspp.F.UPF` & `qepy-0.0.3rc0/examples/opt/qe/si_pbe_v1.uspp.F.UPF`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/opt/qe/vcrelax.in` & `qepy-0.0.3rc0/examples/opt/qe/vcrelax.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/original/6.5/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/original/6.5/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/original/6.5/qe_in.in` & `qepy-0.0.3rc0/examples/original/6.5/qe_in.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/original/6.5/run_pwscf.py` & `qepy-0.0.3rc0/examples/original/6.5/run_pwscf.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/original/6.8/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/original/6.8/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/original/6.8/qe_in.in` & `qepy-0.0.3rc0/examples/original/6.8/qe_in.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/scf/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/scf/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/scf/qe_in.in` & `qepy-0.0.3rc0/examples/scf/qe_in.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/scf/test_pwscf.py` & `qepy-0.0.3rc0/examples/scf/test_pwscf.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/scf/test_pwscf_iterative.py` & `qepy-0.0.3rc0/examples/scf/test_pwscf_iterative.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/tddft/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/tddft/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/tddft/qe_in.in` & `qepy-0.0.3rc0/examples/tddft/qe_in.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/tddft/test_ce_tddft.py` & `qepy-0.0.3rc0/examples/tddft/test_ce_tddft.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/tddft/test_ce_tddft_restart.py` & `qepy-0.0.3rc0/examples/tddft/test_ce_tddft_restart.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/DATA/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/test/DATA/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/DATA/al_md_3.traj` & `qepy-0.0.3rc0/examples/test/DATA/al_md_3.traj`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/DATA/oldxml/al_oldxml.save/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.save/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/DATA/oldxml/al_oldxml.save/K00001/eigenval.xml` & `qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.save/K00001/eigenval.xml`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/DATA/oldxml/al_oldxml.save/charge-density.dat` & `qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.save/charge-density.dat`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/DATA/oldxml/al_oldxml.save/data-file.xml` & `qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.save/data-file.xml`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/DATA/oldxml/al_oldxml.wfc1` & `qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.wfc1`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/eigenval.xml` & `qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/eigenval.xml`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/evc.dat` & `qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/evc.dat`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/gkvectors.dat` & `qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/gkvectors.dat`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/charge-density.dat` & `qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/charge-density.dat`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/data-file.xml` & `qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/data-file.xml`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/gvectors.dat` & `qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/gvectors.dat`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/DATA/qe_fake.in` & `qepy-0.0.3rc0/examples/test/DATA/qe_fake.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/DATA/qe_in.in` & `qepy-0.0.3rc0/examples/test/DATA/qe_in.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/qe-6.5/test.sh` & `qepy-0.0.3rc0/examples/test/qe-6.5/test.sh`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/qe-6.5/test_ce_tddft.py` & `qepy-0.0.3rc0/examples/test/qe-6.5/test_ce_tddft.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/qe-6.5/test_comm.py` & `qepy-0.0.3rc0/examples/test/qe-6.5/test_comm.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/qe-6.5/test_oldxml.py` & `qepy-0.0.3rc0/examples/test/qe-6.5/test_oldxml.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/qe-6.5/test_pwscf.py` & `qepy-0.0.3rc0/examples/test/qe-6.5/test_pwscf.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/qe-6.5/test_pwscf_scf.py` & `qepy-0.0.3rc0/examples/test/qe-6.5/test_pwscf_scf.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/qe-6.5/test_readfile.py` & `qepy-0.0.3rc0/examples/test/qe-6.5/test_readfile.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/test.sh` & `qepy-0.0.3rc0/examples/test/test.sh`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/test_ase_md.py` & `qepy-0.0.3rc0/examples/test/test_ase_md.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/test_ce_tddft.py` & `qepy-0.0.3rc0/examples/test/test_ce_tddft.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/test_oldxml.py` & `qepy-0.0.3rc0/examples/test/test_oldxml.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/test_pwscf.py` & `qepy-0.0.3rc0/examples/test/test_pwscf.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/test_pwscf_iterative.py` & `qepy-0.0.3rc0/examples/test/test_pwscf_iterative.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/examples/test/test_readfile.py` & `qepy-0.0.3rc0/examples/test/test_readfile.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/install/Makefile` & `qepy-0.0.3rc0/install/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 QEINC := $(QEINC:%/Makefile=%/) -I.
 
 TDDFT_SOURCES = tddft_module.f90
 TDDFT_FILES = ${TDDFT_SOURCES}
 
 QEPY_ADD := qepy_common.f90 qepy_mod.f90 \
 			scatter_mod.f90 funct.f90 potinit.f90 wfcinit.f90\
-			pw_restart_new.f90 read_file_new.f90 qes_read_module.f90 \
-			pwscf.f90 command_line_options.f90
+			pw_restart_new.f90 read_file_new.f90 qes_read_module.f90
 
 QEPY_SOURCES := qepy_setlocal.f90 qepy_v_of_rho.f90 qepy_pw2casino_write.f90 \
               qepy_init_run.f90 qepy_pwscf.f90 qepy_run_pwscf.f90 qepy_electrons.f90 \
               qepy_electrons_nscf.f90 qepy_hinit1.f90 qepy_forces.f90 qepy_stop_run.f90 \
               qepy_stress.f90 
 
 OLDXML_SOURCES := oldxml_qexml.f90 oldxml_xml_io_base.f90 \
```

### Comparing `qepy-0.0.3/install/Makefile.cetddft` & `qepy-0.0.3rc0/install/Makefile.cetddft`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/install/kind_map.json` & `qepy-0.0.3rc0/install/kind_map.json`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/install/make.depend` & `qepy-0.0.3rc0/install/make.depend`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/install/make.qe.inc` & `qepy-0.0.3rc0/install/make.qe.inc`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/qepy/__init__.py` & `qepy-0.0.3rc0/qepy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,17 @@
                     attr = mod + '.' + item
                     operator.attrgetter(attr)(qepy).clear()
 
 
 qepy_clean_saved()
 __author__ = "Pavanello Research Group"
 __contact__ = "m.pavanello@rutgers.edu"
-__version__ = "0.0.3"
+__version__ = "0.0.3rc0"
 __license__ = "GPL"
-__date__ = "2023-06-03"
+__date__ = "2023-04-26"
 
 try:
     from importlib.metadata import version # python >= 3.8
 except Exception :
     try:
         from importlib_metadata import version
     except Exception :
```

### Comparing `qepy-0.0.3/qepy/__new__.py` & `qepy-0.0.3rc0/qepy/__new__.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/qepy/calculator.py` & `qepy-0.0.3rc0/qepy/calculator.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/qepy/core.py` & `qepy-0.0.3rc0/qepy/core.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/qepy/driver.py` & `qepy-0.0.3rc0/qepy/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,18 +68,14 @@
         The output directory of QE
     qe_options : dict
         A dictionary with input parameters for QE to generate QE input file.
     prog : str
         The name of QE program, default is `pw` which is pw.x in QE.
     progress : bool
         If True, will continue run the QE without clean the workspace, most times used for TDDFT after scf.
-    atoms : object
-        An ase Atoms to generate input file.
-    needwf : bool
-        If False, will not read wavefunctions and skip wavefunction-related initialization.
     kwargs : dict
         Other options
 
 
     .. note::
 
          - The bool `gather` parameter in functions means the data is gathered in root or distributed in all cpus.
@@ -93,31 +89,29 @@
              + potential : Ry
              + density : 1.0/Bohr**3
 
     """
 
     def __init__(self, inputfile = None, comm = None, ldescf = False, iterative = False,
              task = 'scf', embed = None, prefix = None, outdir = None, logfile = None,
-             qe_options = None, prog = 'pw', progress = False, atoms = None, needwf = True,
-             **kwargs):
+             qe_options = None, prog = 'pw', progress = False, atoms = None, **kwargs):
         if embed is None :
             embed = qepy.qepy_common.embed_base()
         self.task = task
         self.embed = embed
         self.comm = comm
         self.inputfile = inputfile
         self.iterative = iterative
         self.prefix = prefix
         self.outdir = outdir
         self.logfile = logfile
         self.qe_options = qe_options
         self.prog = prog
         self.progress = progress
         self.atoms = atoms
-        self.needwf = needwf
         #
         self.embed.ldescf = ldescf
         #
         self.comm = comm
         self.qepy = qepy
         self.qeinput = QEInput()
         #
@@ -233,20 +227,16 @@
             qepy.qepy_initial(inputobj)
             tmpdir = inputobj.tmp_dir.decode().strip() + inputobj.prefix.decode().strip() + '.save' + '/'
             if os.path.isfile(tmpdir + 'data-file.xml'): # only works for qe-6.5 !
                 if not hasattr(qepy, 'oldxml_read_file') :
                     raise AttributeError("Please reinstall the QEpy with 'oldxml=yes'.")
                 qepy.oldxml_read_file()
             else :
-                if self.needwf :
-                    qepy.read_file()
-                else :
-                    qepy.read_file_new(False)
-            if self.needwf :
-                qepy.qepy_mod.qepy_open_files()
+                qepy.read_file()
+            qepy.qepy_mod.qepy_open_files()
         else :
             qepy.qepy_pwscf(inputfile, commf)
             self.embed.iterative = self.iterative
             if self.embed.iterative :
                 qepy.control_flags.set_niter(1)
         #
         self.density = np.zeros((1, 1))
@@ -677,15 +667,15 @@
         v_obj.of_r[:] = 0.0
         ehart, etxc, vtxc, eth, charge = qepy.qepy_v_of_rho(rho_obj, rho_core, rhog_core, etotefield, v_obj)
         info = [ehart, etxc, vtxc, eth, etotefield, charge]
         if add :
             out += v_obj.of_r
         else :
             out[:] = v_obj.of_r
-        return out, info
+        return out, *info
 
     def get_hartree_potential(self, gather = True, out = None, **kwargs):
         return self.get_hartree(gather=gather, out=out, **kwargs)[0]
 
     def get_exchange_correlation_potential(self, gather = True, out = None, **kwargs):
         return self.get_exchange_correlation(gather=gather, out=out, **kwargs)[0]
```

### Comparing `qepy-0.0.3/qepy/io.py` & `qepy-0.0.3rc0/qepy/io.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/qepy.egg-info/PKG-INFO` & `qepy-0.0.3rc0/qepy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qepy
-Version: 0.0.3
+Version: 0.0.3rc0
 Summary: QEpy: Quantum ESPRESSO Python interface
 Home-page: https://gitlab.com/shaoxc/qepy
 Author: Pavanello Research Group
 Author-email: m.pavanello@rutgers.edu
 License: GPL
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `qepy-0.0.3/qepy.egg-info/SOURCES.txt` & `qepy-0.0.3rc0/qepy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .gitignore
 .gitlab-ci.yml
 .gitmodules
 README.md
 pyproject.toml
 setup.py
 .github/workflows/linux.yml
-.github/workflows/macos_arm64.yml
 .github/workflows/publish.yml
 .github/workflows/wheels.yml
 doc/Makefile
 doc/make.bat
 doc/source/QEpy.bib
 doc/source/conf.py
 doc/source/contact.rst
@@ -141,33 +140,27 @@
 install/Makefile.cetddft
 install/kind_map.json
 install/make.depend
 install/make.depend.cetddft
 install/make.qe.inc
 install/makedeps.sh
 qepy/__init__.py
-qepy/__main__.py
 qepy/__new__.py
 qepy/calculator.py
 qepy/core.py
 qepy/driver.py
 qepy/io.py
 qepy.egg-info/PKG-INFO
 qepy.egg-info/SOURCES.txt
 qepy.egg-info/dependency_links.txt
 qepy.egg-info/not-zip-safe
 qepy.egg-info/requires.txt
 qepy.egg-info/top_level.txt
-qepy/cui/__init__.py
-qepy/cui/main.py
-qepy/cui/pwx.py
 src/api/qepy_common.f90
 src/api/qepy_mod.f90
-src/cmd/command_line_options.f90
-src/cmd/pwscf.f90
 src/fix/funct.f90
 src/fix/potinit.f90
 src/fix/pw_restart_new.f90
 src/fix/qes_read_module.f90
 src/fix/read_file_new.f90
 src/fix/scatter_mod.f90
 src/fix/wfcinit.f90
```

### Comparing `qepy-0.0.3/setup.py` & `qepy-0.0.3rc0/setup.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/api/qepy_common.f90` & `qepy-0.0.3rc0/src/api/qepy_common.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/api/qepy_mod.f90` & `qepy-0.0.3rc0/src/api/qepy_mod.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/fix/funct.f90` & `qepy-0.0.3rc0/src/fix/funct.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/fix/potinit.f90` & `qepy-0.0.3rc0/src/fix/potinit.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/fix/pw_restart_new.f90` & `qepy-0.0.3rc0/src/fix/pw_restart_new.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/fix/qes_read_module.f90` & `qepy-0.0.3rc0/src/fix/qes_read_module.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/fix/read_file_new.f90` & `qepy-0.0.3rc0/src/fix/read_file_new.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/fix/scatter_mod.f90` & `qepy-0.0.3rc0/src/fix/scatter_mod.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/fix/wfcinit.f90` & `qepy-0.0.3rc0/src/fix/wfcinit.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/ldau/qepy_econf.ini` & `qepy-0.0.3rc0/src/ldau/qepy_econf.ini`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/ldau/qepy_ldau_patch.py` & `qepy-0.0.3rc0/src/ldau/qepy_ldau_patch.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/oldxml/oldxml_io_rho_xml.f90` & `qepy-0.0.3rc0/src/oldxml/oldxml_io_rho_xml.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/oldxml/oldxml_potinit.f90` & `qepy-0.0.3rc0/src/oldxml/oldxml_potinit.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/oldxml/oldxml_pw_restart.f90` & `qepy-0.0.3rc0/src/oldxml/oldxml_pw_restart.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/oldxml/oldxml_qexml.f90` & `qepy-0.0.3rc0/src/oldxml/oldxml_qexml.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/oldxml/oldxml_read_file.f90` & `qepy-0.0.3rc0/src/oldxml/oldxml_read_file.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/oldxml/oldxml_wfcinit.f90` & `qepy-0.0.3rc0/src/oldxml/oldxml_wfcinit.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/oldxml/oldxml_xml_io_base.f90` & `qepy-0.0.3rc0/src/oldxml/oldxml_xml_io_base.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/qe/qepy_electrons.f90` & `qepy-0.0.3rc0/src/qe/qepy_electrons.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/qe/qepy_electrons_nscf.f90` & `qepy-0.0.3rc0/src/qe/qepy_electrons_nscf.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/qe/qepy_forces.f90` & `qepy-0.0.3rc0/src/qe/qepy_forces.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/qe/qepy_hinit1.f90` & `qepy-0.0.3rc0/src/qe/qepy_hinit1.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/qe/qepy_init_run.f90` & `qepy-0.0.3rc0/src/qe/qepy_init_run.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/qe/qepy_pw2casino_write.f90` & `qepy-0.0.3rc0/src/qe/qepy_pw2casino_write.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/qe/qepy_pwscf.f90` & `qepy-0.0.3rc0/src/qe/qepy_pwscf.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/qe/qepy_run_pwscf.f90` & `qepy-0.0.3rc0/src/qe/qepy_run_pwscf.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/qe/qepy_setlocal.f90` & `qepy-0.0.3rc0/src/qe/qepy_setlocal.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/qe/qepy_stop_run.f90` & `qepy-0.0.3rc0/src/qe/qepy_stop_run.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/qe/qepy_stress.f90` & `qepy-0.0.3rc0/src/qe/qepy_stress.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/qe/qepy_v_of_rho.f90` & `qepy-0.0.3rc0/src/qe/qepy_v_of_rho.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/tddft/qepy_molecule_optical_absorption.f90` & `qepy-0.0.3rc0/src/tddft/qepy_molecule_optical_absorption.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/tddft/qepy_tddft_common.f90` & `qepy-0.0.3rc0/src/tddft/qepy_tddft_common.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/tddft/qepy_tddft_main.f90` & `qepy-0.0.3rc0/src/tddft/qepy_tddft_main.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/tddft/qepy_tddft_mod.f90` & `qepy-0.0.3rc0/src/tddft/qepy_tddft_mod.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/tddft/qepy_tddft_routines.f90` & `qepy-0.0.3rc0/src/tddft/qepy_tddft_routines.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/tddft/qepy_tddft_setup.f90` & `qepy-0.0.3rc0/src/tddft/qepy_tddft_setup.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/src/tddft/qepy_update_ham.f90` & `qepy-0.0.3rc0/src/tddft/qepy_update_ham.f90`

 * *Files identical despite different names*

