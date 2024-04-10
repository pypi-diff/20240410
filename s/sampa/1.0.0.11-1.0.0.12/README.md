# Comparing `tmp/sampa-1.0.0.11.tar.gz` & `tmp/sampa-1.0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sampa-1.0.0.11.tar", last modified: Wed Apr 10 01:48:17 2024, max compression
+gzip compressed data, was "sampa-1.0.0.12.tar", last modified: Wed Apr 10 02:02:56 2024, max compression
```

## Comparing `sampa-1.0.0.11.tar` & `sampa-1.0.0.12.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 01:48:17.972560 sampa-1.0.0.11/
--rw-rw-rw-   0        0        0       13 2024-04-09 02:21:11.000000 sampa-1.0.0.11/LICENSE.txt
--rw-rw-rw-   0        0        0      288 2024-04-10 01:48:17.972560 sampa-1.0.0.11/PKG-INFO
--rw-rw-rw-   0        0        0       51 2024-04-09 02:20:56.000000 sampa-1.0.0.11/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 01:48:17.628804 sampa-1.0.0.11/sampa/
--rw-rw-rw-   0        0        0       52 2024-04-09 02:21:40.000000 sampa-1.0.0.11/sampa/__init__.py
--rw-rw-rw-   0        0        0     7300 2024-04-10 01:47:52.000000 sampa-1.0.0.11/sampa/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 01:48:17.691305 sampa-1.0.0.11/sampa/src/
--rw-rw-rw-   0        0        0    67538 2024-04-09 14:15:03.000000 sampa-1.0.0.11/sampa/src/HeteroStructure_Generator-Augusto_Dlelis.py
--rw-rw-rw-   0        0        0    71626 2024-04-09 02:22:18.000000 sampa-1.0.0.11/sampa/src/HeteroStructure_Generator.py
-drwxrwxrwx   0        0        0        0 2024-04-10 01:48:17.706929 sampa-1.0.0.11/sampa/src/INPUTS/
--rw-rw-rw-   0        0        0      228 2024-04-05 14:40:05.000000 sampa-1.0.0.11/sampa/src/INPUTS/INCAR_bader
--rw-rw-rw-   0        0        0      269 2024-04-05 14:40:00.000000 sampa-1.0.0.11/sampa/src/INPUTS/INCAR_bader.SO
--rw-rw-rw-   0        0        0      223 2024-03-27 17:25:45.000000 sampa-1.0.0.11/sampa/src/INPUTS/INCAR_bands
--rw-rw-rw-   0        0        0      264 2024-03-24 14:34:17.000000 sampa-1.0.0.11/sampa/src/INPUTS/INCAR_bands.SO
--rw-rw-rw-   0        0        0      212 2024-04-04 18:32:53.000000 sampa-1.0.0.11/sampa/src/INPUTS/INCAR_dos
--rw-rw-rw-   0        0        0      253 2024-04-04 18:33:02.000000 sampa-1.0.0.11/sampa/src/INPUTS/INCAR_dos.SO
--rw-rw-rw-   0        0        0      201 2024-04-04 18:33:10.000000 sampa-1.0.0.11/sampa/src/INPUTS/INCAR_relax
--rw-rw-rw-   0        0        0      214 2024-04-04 18:33:17.000000 sampa-1.0.0.11/sampa/src/INPUTS/INCAR_scf
--rw-rw-rw-   0        0        0      255 2024-04-04 18:33:33.000000 sampa-1.0.0.11/sampa/src/INPUTS/INCAR_scf.SO
-drwxrwxrwx   0        0        0        0 2024-04-10 01:48:17.722555 sampa-1.0.0.11/sampa/src/INPUTS/inputs_VASProcar/
--rw-rw-rw-   0        0        0     4485 2024-03-20 16:04:46.000000 sampa-1.0.0.11/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.bands
--rw-rw-rw-   0        0        0     3123 2024-04-08 15:25:48.000000 sampa-1.0.0.11/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar
--rw-rw-rw-   0        0        0     2525 2024-03-20 16:04:58.000000 sampa-1.0.0.11/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.dos
--rw-rw-rw-   0        0        0     9603 2024-03-21 16:46:57.000000 sampa-1.0.0.11/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.location
--rw-rw-rw-   0        0        0     1187 2024-03-23 20:35:59.000000 sampa-1.0.0.11/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot
--rw-rw-rw-   0        0        0     6378 2024-03-20 16:05:20.000000 sampa-1.0.0.11/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals
--rw-rw-rw-   0        0        0     7790 2024-03-20 16:06:00.000000 sampa-1.0.0.11/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.spin
-drwxrwxrwx   0        0        0        0 2024-04-10 01:48:17.972560 sampa-1.0.0.11/sampa/src/POTCAR/
--rw-rw-rw-   0        0        0   213736 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ac
--rw-rw-rw-   0        0        0   191992 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ag
--rw-rw-rw-   0        0        0   156798 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Al
--rw-rw-rw-   0        0        0   224618 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Am
--rw-rw-rw-   0        0        0   132587 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ar
--rw-rw-rw-   0        0        0   164635 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_As
--rw-rw-rw-   0        0        0   181002 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_At
--rw-rw-rw-   0        0        0   196481 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Au
--rw-rw-rw-   0        0        0   135569 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_B
--rw-rw-rw-   0        0        0   182570 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ba
--rw-rw-rw-   0        0        0   153387 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Be
--rw-rw-rw-   0        0        0   179838 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Bi
--rw-rw-rw-   0        0        0   164633 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Br
--rw-rw-rw-   0        0        0   140609 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_C
--rw-rw-rw-   0        0        0   184607 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ca
--rw-rw-rw-   0        0        0   181214 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Cd
--rw-rw-rw-   0        0        0   226389 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ce
--rw-rw-rw-   0        0        0   156238 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Cl
--rw-rw-rw-   0        0        0   283773 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Cm
--rw-rw-rw-   0        0        0   200294 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Co
--rw-rw-rw-   0        0        0   201084 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Cr
--rw-rw-rw-   0        0        0   171057 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Cs
--rw-rw-rw-   0        0        0   199387 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Cu
--rw-rw-rw-   0        0        0   182572 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Dy
--rw-rw-rw-   0        0        0   182569 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Er
--rw-rw-rw-   0        0        0   183945 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Eu
--rw-rw-rw-   0        0        0   132929 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_F
--rw-rw-rw-   0        0        0   188072 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Fe
--rw-rw-rw-   0        0        0   232226 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Fr
--rw-rw-rw-   0        0        0   204574 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ga
--rw-rw-rw-   0        0        0   182576 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Gd
--rw-rw-rw-   0        0        0   223350 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ge
--rw-rw-rw-   0        0        0   131047 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_H
--rw-rw-rw-   0        0        0   124230 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_He
--rw-rw-rw-   0        0        0   180541 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Hf
--rw-rw-rw-   0        0        0   179835 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Hg
--rw-rw-rw-   0        0        0   182571 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ho
--rw-rw-rw-   0        0        0   170378 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_I
--rw-rw-rw-   0        0        0   181920 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_In
--rw-rw-rw-   0        0        0   180526 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ir
--rw-rw-rw-   0        0        0   167632 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_K
--rw-rw-rw-   0        0        0   132181 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Kr
--rw-rw-rw-   0        0        0   215441 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_La
--rw-rw-rw-   0        0        0   128657 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Li
--rw-rw-rw-   0        0        0   181889 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Lu
--rw-rw-rw-   0        0        0   187040 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Mg
--rw-rw-rw-   0        0        0   200323 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Mn
--rw-rw-rw-   0        0        0   199419 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Mo
--rw-rw-rw-   0        0        0   144499 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_N
--rw-rw-rw-   0        0        0   168209 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Na
--rw-rw-rw-   0        0        0   198784 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Nb
--rw-rw-rw-   0        0        0   181887 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Nd
--rw-rw-rw-   0        0        0   156765 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ne
--rw-rw-rw-   0        0        0   200288 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ni
--rw-rw-rw-   0        0        0   213739 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Np
--rw-rw-rw-   0        0        0   139971 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_O
--rw-rw-rw-   0        0        0   186889 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Os
--rw-rw-rw-   0        0        0   156259 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_P
--rw-rw-rw-   0        0        0   213756 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Pa
--rw-rw-rw-   0        0        0   179838 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Pb
--rw-rw-rw-   0        0        0   192711 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Pd
--rw-rw-rw-   0        0        0   181907 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Pm
--rw-rw-rw-   0        0        0   181885 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Pr
--rw-rw-rw-   0        0        0   190531 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Pt
--rw-rw-rw-   0        0        0   213736 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Pu
--rw-rw-rw-   0        0        0   231306 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ra
--rw-rw-rw-   0        0        0   165823 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Rb
--rw-rw-rw-   0        0        0   186891 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Re
--rw-rw-rw-   0        0        0   191990 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Rh
--rw-rw-rw-   0        0        0   180090 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Rn
--rw-rw-rw-   0        0        0   191994 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ru
--rw-rw-rw-   0        0        0   156255 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_S
--rw-rw-rw-   0        0        0   164037 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Sb
--rw-rw-rw-   0        0        0   185392 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Sc
--rw-rw-rw-   0        0        0   164627 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Se
--rw-rw-rw-   0        0        0   156807 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Si
--rw-rw-rw-   0        0        0   181908 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Sn
--rw-rw-rw-   0        0        0   182577 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Sr
--rw-rw-rw-   0        0        0   179857 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ta
--rw-rw-rw-   0        0        0   182576 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Tb
--rw-rw-rw-   0        0        0   192707 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Tc
--rw-rw-rw-   0        0        0   170392 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Te
--rw-rw-rw-   0        0        0   213762 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Th
--rw-rw-rw-   0        0        0   201062 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ti
--rw-rw-rw-   0        0        0   179844 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Tl
--rw-rw-rw-   0        0        0   189055 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Tm
--rw-rw-rw-   0        0        0   213749 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_U
--rw-rw-rw-   0        0        0   201062 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_V
--rw-rw-rw-   0        0        0   197244 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_W
--rw-rw-rw-   0        0        0   131729 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Xe
--rw-rw-rw-   0        0        0   183295 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Y
--rw-rw-rw-   0        0        0   181196 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Yb
--rw-rw-rw-   0        0        0   182588 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Zn
--rw-rw-rw-   0        0        0   182594 2024-03-19 13:02:04.000000 sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Zr
--rw-rw-rw-   0        0        0     1092 2024-04-09 02:22:59.000000 sampa-1.0.0.11/sampa/src/POTCAR/_info.py
--rw-rw-rw-   0        0        0     1979 2024-04-09 02:22:53.000000 sampa-1.0.0.11/sampa/src/POTCAR/cut_off_energy.py
--rw-rw-rw-   0        0        0     3968 2024-04-10 01:37:39.000000 sampa-1.0.0.11/sampa/src/SAMBA_HeteroStructure.input
--rw-rw-rw-   0        0        0     1610 2024-04-10 01:37:55.000000 sampa-1.0.0.11/sampa/src/SAMBA_WorkFlow.input
--rw-rw-rw-   0        0        0  4715152 2023-08-19 14:41:30.000000 sampa-1.0.0.11/sampa/src/bader
--rw-rw-rw-   0        0        0     4517 2024-04-09 02:22:42.000000 sampa-1.0.0.11/sampa/src/bader_poscar.py
--rw-rw-rw-   0        0        0     2522 2024-04-09 02:22:36.000000 sampa-1.0.0.11/sampa/src/bader_update.py
--rw-rw-rw-   0        0        0     7055 2024-04-09 02:22:30.000000 sampa-1.0.0.11/sampa/src/charge_transfer.py
--rw-rw-rw-   0        0        0     2139 2019-12-02 15:59:08.000000 sampa-1.0.0.11/sampa/src/chgsum.pl
--rw-rw-rw-   0        0        0      325 2024-04-09 02:22:24.000000 sampa-1.0.0.11/sampa/src/contcar_update.py
--rw-rw-rw-   0        0        0     9936 2024-04-09 12:38:41.000000 sampa-1.0.0.11/sampa/src/job.py
--rw-rw-rw-   0        0        0     6676 2024-04-09 12:37:10.000000 sampa-1.0.0.11/sampa/src/kpoints.py
--rw-rw-rw-   0        0        0    17429 2024-04-10 01:32:58.000000 sampa-1.0.0.11/sampa/src/make_files.py
--rw-rw-rw-   0        0        0     4024 2024-04-09 02:21:55.000000 sampa-1.0.0.11/sampa/src/output.py
--rw-rw-rw-   0        0        0     1048 2024-04-10 01:31:22.000000 sampa-1.0.0.11/sampa/src/potcar.py
-drwxrwxrwx   0        0        0        0 2024-04-10 01:48:17.644434 sampa-1.0.0.11/sampa.egg-info/
--rw-rw-rw-   0        0        0      288 2024-04-10 01:48:17.000000 sampa-1.0.0.11/sampa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3908 2024-04-10 01:48:17.000000 sampa-1.0.0.11/sampa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 01:48:17.000000 sampa-1.0.0.11/sampa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-10 01:48:17.000000 sampa-1.0.0.11/sampa.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2024-04-10 01:48:17.000000 sampa-1.0.0.11/sampa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-10 01:48:17.000000 sampa-1.0.0.11/sampa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      167 2024-04-10 01:48:17.972560 sampa-1.0.0.11/setup.cfg
--rw-rw-rw-   0        0        0      719 2024-04-10 01:48:05.000000 sampa-1.0.0.11/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:02:56.734220 sampa-1.0.0.12/
+-rw-rw-rw-   0        0        0       13 2024-04-09 02:21:11.000000 sampa-1.0.0.12/LICENSE.txt
+-rw-rw-rw-   0        0        0      288 2024-04-10 02:02:56.734220 sampa-1.0.0.12/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2024-04-09 02:20:56.000000 sampa-1.0.0.12/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 02:02:56.374844 sampa-1.0.0.12/sampa/
+-rw-rw-rw-   0        0        0       52 2024-04-09 02:21:40.000000 sampa-1.0.0.12/sampa/__init__.py
+-rw-rw-rw-   0        0        0     7355 2024-04-10 02:02:30.000000 sampa-1.0.0.12/sampa/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:02:56.437343 sampa-1.0.0.12/sampa/src/
+-rw-rw-rw-   0        0        0    67538 2024-04-09 14:15:03.000000 sampa-1.0.0.12/sampa/src/HeteroStructure_Generator-Augusto_Dlelis.py
+-rw-rw-rw-   0        0        0    71626 2024-04-09 02:22:18.000000 sampa-1.0.0.12/sampa/src/HeteroStructure_Generator.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:02:56.452970 sampa-1.0.0.12/sampa/src/INPUTS/
+-rw-rw-rw-   0        0        0      228 2024-04-05 14:40:05.000000 sampa-1.0.0.12/sampa/src/INPUTS/INCAR_bader
+-rw-rw-rw-   0        0        0      269 2024-04-05 14:40:00.000000 sampa-1.0.0.12/sampa/src/INPUTS/INCAR_bader.SO
+-rw-rw-rw-   0        0        0      223 2024-03-27 17:25:45.000000 sampa-1.0.0.12/sampa/src/INPUTS/INCAR_bands
+-rw-rw-rw-   0        0        0      264 2024-03-24 14:34:17.000000 sampa-1.0.0.12/sampa/src/INPUTS/INCAR_bands.SO
+-rw-rw-rw-   0        0        0      212 2024-04-04 18:32:53.000000 sampa-1.0.0.12/sampa/src/INPUTS/INCAR_dos
+-rw-rw-rw-   0        0        0      253 2024-04-04 18:33:02.000000 sampa-1.0.0.12/sampa/src/INPUTS/INCAR_dos.SO
+-rw-rw-rw-   0        0        0      201 2024-04-04 18:33:10.000000 sampa-1.0.0.12/sampa/src/INPUTS/INCAR_relax
+-rw-rw-rw-   0        0        0      214 2024-04-04 18:33:17.000000 sampa-1.0.0.12/sampa/src/INPUTS/INCAR_scf
+-rw-rw-rw-   0        0        0      255 2024-04-04 18:33:33.000000 sampa-1.0.0.12/sampa/src/INPUTS/INCAR_scf.SO
+drwxrwxrwx   0        0        0        0 2024-04-10 02:02:56.468596 sampa-1.0.0.12/sampa/src/INPUTS/inputs_VASProcar/
+-rw-rw-rw-   0        0        0     4485 2024-03-20 16:04:46.000000 sampa-1.0.0.12/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.bands
+-rw-rw-rw-   0        0        0     3123 2024-04-08 15:25:48.000000 sampa-1.0.0.12/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar
+-rw-rw-rw-   0        0        0     2525 2024-03-20 16:04:58.000000 sampa-1.0.0.12/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.dos
+-rw-rw-rw-   0        0        0     9603 2024-03-21 16:46:57.000000 sampa-1.0.0.12/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.location
+-rw-rw-rw-   0        0        0     1187 2024-03-23 20:35:59.000000 sampa-1.0.0.12/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot
+-rw-rw-rw-   0        0        0     6378 2024-03-20 16:05:20.000000 sampa-1.0.0.12/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals
+-rw-rw-rw-   0        0        0     7790 2024-03-20 16:06:00.000000 sampa-1.0.0.12/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.spin
+drwxrwxrwx   0        0        0        0 2024-04-10 02:02:56.734220 sampa-1.0.0.12/sampa/src/POTCAR/
+-rw-rw-rw-   0        0        0   213736 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ac
+-rw-rw-rw-   0        0        0   191992 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ag
+-rw-rw-rw-   0        0        0   156798 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Al
+-rw-rw-rw-   0        0        0   224618 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Am
+-rw-rw-rw-   0        0        0   132587 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ar
+-rw-rw-rw-   0        0        0   164635 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_As
+-rw-rw-rw-   0        0        0   181002 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_At
+-rw-rw-rw-   0        0        0   196481 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Au
+-rw-rw-rw-   0        0        0   135569 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_B
+-rw-rw-rw-   0        0        0   182570 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ba
+-rw-rw-rw-   0        0        0   153387 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Be
+-rw-rw-rw-   0        0        0   179838 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Bi
+-rw-rw-rw-   0        0        0   164633 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Br
+-rw-rw-rw-   0        0        0   140609 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_C
+-rw-rw-rw-   0        0        0   184607 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ca
+-rw-rw-rw-   0        0        0   181214 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Cd
+-rw-rw-rw-   0        0        0   226389 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ce
+-rw-rw-rw-   0        0        0   156238 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Cl
+-rw-rw-rw-   0        0        0   283773 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Cm
+-rw-rw-rw-   0        0        0   200294 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Co
+-rw-rw-rw-   0        0        0   201084 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Cr
+-rw-rw-rw-   0        0        0   171057 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Cs
+-rw-rw-rw-   0        0        0   199387 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Cu
+-rw-rw-rw-   0        0        0   182572 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Dy
+-rw-rw-rw-   0        0        0   182569 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Er
+-rw-rw-rw-   0        0        0   183945 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Eu
+-rw-rw-rw-   0        0        0   132929 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_F
+-rw-rw-rw-   0        0        0   188072 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Fe
+-rw-rw-rw-   0        0        0   232226 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Fr
+-rw-rw-rw-   0        0        0   204574 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ga
+-rw-rw-rw-   0        0        0   182576 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Gd
+-rw-rw-rw-   0        0        0   223350 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ge
+-rw-rw-rw-   0        0        0   131047 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_H
+-rw-rw-rw-   0        0        0   124230 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_He
+-rw-rw-rw-   0        0        0   180541 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Hf
+-rw-rw-rw-   0        0        0   179835 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Hg
+-rw-rw-rw-   0        0        0   182571 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ho
+-rw-rw-rw-   0        0        0   170378 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_I
+-rw-rw-rw-   0        0        0   181920 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_In
+-rw-rw-rw-   0        0        0   180526 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ir
+-rw-rw-rw-   0        0        0   167632 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_K
+-rw-rw-rw-   0        0        0   132181 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Kr
+-rw-rw-rw-   0        0        0   215441 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_La
+-rw-rw-rw-   0        0        0   128657 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Li
+-rw-rw-rw-   0        0        0   181889 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Lu
+-rw-rw-rw-   0        0        0   187040 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Mg
+-rw-rw-rw-   0        0        0   200323 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Mn
+-rw-rw-rw-   0        0        0   199419 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Mo
+-rw-rw-rw-   0        0        0   144499 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_N
+-rw-rw-rw-   0        0        0   168209 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Na
+-rw-rw-rw-   0        0        0   198784 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Nb
+-rw-rw-rw-   0        0        0   181887 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Nd
+-rw-rw-rw-   0        0        0   156765 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ne
+-rw-rw-rw-   0        0        0   200288 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ni
+-rw-rw-rw-   0        0        0   213739 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Np
+-rw-rw-rw-   0        0        0   139971 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_O
+-rw-rw-rw-   0        0        0   186889 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Os
+-rw-rw-rw-   0        0        0   156259 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_P
+-rw-rw-rw-   0        0        0   213756 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Pa
+-rw-rw-rw-   0        0        0   179838 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Pb
+-rw-rw-rw-   0        0        0   192711 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Pd
+-rw-rw-rw-   0        0        0   181907 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Pm
+-rw-rw-rw-   0        0        0   181885 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Pr
+-rw-rw-rw-   0        0        0   190531 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Pt
+-rw-rw-rw-   0        0        0   213736 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Pu
+-rw-rw-rw-   0        0        0   231306 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ra
+-rw-rw-rw-   0        0        0   165823 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Rb
+-rw-rw-rw-   0        0        0   186891 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Re
+-rw-rw-rw-   0        0        0   191990 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Rh
+-rw-rw-rw-   0        0        0   180090 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Rn
+-rw-rw-rw-   0        0        0   191994 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ru
+-rw-rw-rw-   0        0        0   156255 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_S
+-rw-rw-rw-   0        0        0   164037 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Sb
+-rw-rw-rw-   0        0        0   185392 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Sc
+-rw-rw-rw-   0        0        0   164627 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Se
+-rw-rw-rw-   0        0        0   156807 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Si
+-rw-rw-rw-   0        0        0   181908 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Sn
+-rw-rw-rw-   0        0        0   182577 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Sr
+-rw-rw-rw-   0        0        0   179857 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ta
+-rw-rw-rw-   0        0        0   182576 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Tb
+-rw-rw-rw-   0        0        0   192707 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Tc
+-rw-rw-rw-   0        0        0   170392 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Te
+-rw-rw-rw-   0        0        0   213762 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Th
+-rw-rw-rw-   0        0        0   201062 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ti
+-rw-rw-rw-   0        0        0   179844 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Tl
+-rw-rw-rw-   0        0        0   189055 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Tm
+-rw-rw-rw-   0        0        0   213749 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_U
+-rw-rw-rw-   0        0        0   201062 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_V
+-rw-rw-rw-   0        0        0   197244 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_W
+-rw-rw-rw-   0        0        0   131729 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Xe
+-rw-rw-rw-   0        0        0   183295 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Y
+-rw-rw-rw-   0        0        0   181196 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Yb
+-rw-rw-rw-   0        0        0   182588 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Zn
+-rw-rw-rw-   0        0        0   182594 2024-03-19 13:02:04.000000 sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Zr
+-rw-rw-rw-   0        0        0     1094 2024-04-10 02:00:46.000000 sampa-1.0.0.12/sampa/src/POTCAR/_info.py
+-rw-rw-rw-   0        0        0     1979 2024-04-09 02:22:53.000000 sampa-1.0.0.12/sampa/src/POTCAR/cut_off_energy.py
+-rw-rw-rw-   0        0        0     3968 2024-04-10 01:37:39.000000 sampa-1.0.0.12/sampa/src/SAMBA_HeteroStructure.input
+-rw-rw-rw-   0        0        0     1610 2024-04-10 01:37:55.000000 sampa-1.0.0.12/sampa/src/SAMBA_WorkFlow.input
+-rw-rw-rw-   0        0        0  4715152 2023-08-19 14:41:30.000000 sampa-1.0.0.12/sampa/src/bader
+-rw-rw-rw-   0        0        0     4517 2024-04-09 02:22:42.000000 sampa-1.0.0.12/sampa/src/bader_poscar.py
+-rw-rw-rw-   0        0        0     2522 2024-04-09 02:22:36.000000 sampa-1.0.0.12/sampa/src/bader_update.py
+-rw-rw-rw-   0        0        0     7055 2024-04-09 02:22:30.000000 sampa-1.0.0.12/sampa/src/charge_transfer.py
+-rw-rw-rw-   0        0        0     2139 2019-12-02 15:59:08.000000 sampa-1.0.0.12/sampa/src/chgsum.pl
+-rw-rw-rw-   0        0        0      325 2024-04-09 02:22:24.000000 sampa-1.0.0.12/sampa/src/contcar_update.py
+-rw-rw-rw-   0        0        0     9936 2024-04-09 12:38:41.000000 sampa-1.0.0.12/sampa/src/job.py
+-rw-rw-rw-   0        0        0     6676 2024-04-09 12:37:10.000000 sampa-1.0.0.12/sampa/src/kpoints.py
+-rw-rw-rw-   0        0        0    17429 2024-04-10 01:32:58.000000 sampa-1.0.0.12/sampa/src/make_files.py
+-rw-rw-rw-   0        0        0     4024 2024-04-09 02:21:55.000000 sampa-1.0.0.12/sampa/src/output.py
+-rw-rw-rw-   0        0        0     1048 2024-04-10 01:31:22.000000 sampa-1.0.0.12/sampa/src/potcar.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:02:56.390559 sampa-1.0.0.12/sampa.egg-info/
+-rw-rw-rw-   0        0        0      288 2024-04-10 02:02:56.000000 sampa-1.0.0.12/sampa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3908 2024-04-10 02:02:56.000000 sampa-1.0.0.12/sampa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 02:02:56.000000 sampa-1.0.0.12/sampa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-10 02:02:56.000000 sampa-1.0.0.12/sampa.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2024-04-10 02:02:56.000000 sampa-1.0.0.12/sampa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-10 02:02:56.000000 sampa-1.0.0.12/sampa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      167 2024-04-10 02:02:56.734220 sampa-1.0.0.12/setup.cfg
+-rw-rw-rw-   0        0        0      719 2024-04-10 02:02:12.000000 sampa-1.0.0.12/setup.py
```

### Comparing `sampa-1.0.0.11/sampa/__main__.py` & `sampa-1.0.0.12/sampa/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import subprocess
 import pyfiglet
 import shutil
 import time
 import os
 
 
-version = '1.0.0.11'
+version = '1.0.0.12'
 
 
 print(" ")
 print("=============================================================")
 print(f'SAMBA v{version} Copyright (C) 2024 ---------------------------')
 print("Closed source: Adalberto Fazzio's research group (Ilum|CNPEM)")
 print("Author: Augusto de Lelis Araujo -----------------------------")
@@ -116,15 +116,17 @@
 
    # -----------------------------------------------
    # Checking if the "POTCAR" folder exists --------
    # -----------------------------------------------
    if os.path.isdir(dir_files + '/POTCAR'):
       dir_pseudo = dir_files + '/POTCAR'
       shutil.copyfile(dir_codes + '/POTCAR/_info.py', dir_pseudo + '/_info.py')
+      os.chdir(dir_pseudo)
       exec(open(dir_pseudo + '/_info.py').read())
+      os.chdir(dir_sampa)
    else:
       dir_pseudo = dir_codes + '/POTCAR'
    # -----------------------------------
 
    print('')
    print('------------------------------------------------------------------------------')
    print('Verifique os parâmetros no arquivo SAMBA_WorkFlow.input antes de prosseguir --')
```

### Comparing `sampa-1.0.0.11/sampa/src/HeteroStructure_Generator-Augusto_Dlelis.py` & `sampa-1.0.0.12/sampa/src/HeteroStructure_Generator-Augusto_Dlelis.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/HeteroStructure_Generator.py` & `sampa-1.0.0.12/sampa/src/HeteroStructure_Generator.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.bands` & `sampa-1.0.0.12/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.bands`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar` & `sampa-1.0.0.12/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.dos` & `sampa-1.0.0.12/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.dos`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.location` & `sampa-1.0.0.12/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.location`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot` & `sampa-1.0.0.12/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals` & `sampa-1.0.0.12/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.spin` & `sampa-1.0.0.12/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.spin`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ac` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ac`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ag` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ag`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Al` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Al`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Am` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Am`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ar` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ar`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_As` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_As`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_At` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_At`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Au` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Au`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_B` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_B`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ba` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ba`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Be` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Be`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Bi` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Bi`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Br` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Br`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_C` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_C`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ca` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ca`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Cd` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Cd`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ce` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ce`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Cl` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Cl`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Cm` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Cm`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Co` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Co`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Cr` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Cr`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Cs` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Cs`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Cu` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Cu`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Dy` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Dy`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Er` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Er`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Eu` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Eu`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_F` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_F`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Fe` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Fe`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Fr` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Fr`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ga` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ga`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Gd` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Gd`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ge` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ge`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_H` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_H`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_He` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_He`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Hf` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Hf`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Hg` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Hg`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ho` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ho`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_I` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_I`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_In` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_In`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ir` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ir`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_K` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_K`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Kr` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Kr`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_La` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_La`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Li` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Li`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Lu` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Lu`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Mg` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Mg`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Mn` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Mn`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Mo` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Mo`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_N` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_N`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Na` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Na`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Nb` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Nb`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Nd` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Nd`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ne` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ne`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ni` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ni`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Np` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Np`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_O` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_O`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Os` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Os`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_P` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_P`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Pa` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Pa`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Pb` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Pb`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Pd` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Pd`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Pm` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Pm`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Pr` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Pr`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Pt` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Pt`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Pu` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Pu`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ra` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ra`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Rb` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Rb`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Re` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Re`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Rh` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Rh`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Rn` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Rn`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ru` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ru`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_S` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_S`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Sb` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Sb`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Sc` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Sc`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Se` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Se`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Si` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Si`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Sn` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Sn`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Sr` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Sr`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ta` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ta`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Tb` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Tb`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Tc` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Tc`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Te` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Te`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Th` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Th`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Ti` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Ti`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Tl` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Tl`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Tm` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Tm`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_U` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_U`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_V` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_V`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_W` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_W`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Xe` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Xe`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Y` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Y`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Yb` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Yb`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Zn` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Zn`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/POTCAR_Zr` & `sampa-1.0.0.12/sampa/src/POTCAR/POTCAR_Zr`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/_info.py` & `sampa-1.0.0.12/sampa/src/POTCAR/_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # SAMBA Copyright (C) 2024 - Closed source
 
+
 import os
 
 cut_off_energy = open('cut_off_energy.py', "w")
 
 #---------------------------------------------------------
 # Listando os arquivos presentes no diretório 'POTCAR' ---
 #---------------------------------------------------------
```

### Comparing `sampa-1.0.0.11/sampa/src/POTCAR/cut_off_energy.py` & `sampa-1.0.0.12/sampa/src/POTCAR/cut_off_energy.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/SAMBA_HeteroStructure.input` & `sampa-1.0.0.12/sampa/src/SAMBA_HeteroStructure.input`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/SAMBA_WorkFlow.input` & `sampa-1.0.0.12/sampa/src/SAMBA_WorkFlow.input`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/bader` & `sampa-1.0.0.12/sampa/src/bader`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/bader_poscar.py` & `sampa-1.0.0.12/sampa/src/bader_poscar.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/bader_update.py` & `sampa-1.0.0.12/sampa/src/bader_update.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/charge_transfer.py` & `sampa-1.0.0.12/sampa/src/charge_transfer.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/chgsum.pl` & `sampa-1.0.0.12/sampa/src/chgsum.pl`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/job.py` & `sampa-1.0.0.12/sampa/src/job.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/kpoints.py` & `sampa-1.0.0.12/sampa/src/kpoints.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/make_files.py` & `sampa-1.0.0.12/sampa/src/make_files.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/output.py` & `sampa-1.0.0.12/sampa/src/output.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa/src/potcar.py` & `sampa-1.0.0.12/sampa/src/potcar.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/sampa.egg-info/SOURCES.txt` & `sampa-1.0.0.12/sampa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.11/setup.py` & `sampa-1.0.0.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 import json
 from pathlib import Path
 from typing import Optional
 
 setup(
     name = "sampa",
-    version = "1.0.0.11",
+    version = "1.0.0.12",
     entry_points={'console_scripts': ['sampa = sampa:main']},
     description = "...",
     author = "Augusto de Lelis Araujo", 
     author_email = "augusto-lelis@outlook.com",
     license = "Closed source",
     install_requires=['numpy',
                       'requests',
```

