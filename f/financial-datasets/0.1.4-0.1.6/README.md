# Comparing `tmp/financial_datasets-0.1.4.tar.gz` & `tmp/financial_datasets-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financial_datasets-0.1.4.tar", max compression
+gzip compressed data, was "financial_datasets-0.1.6.tar", max compression
```

## Comparing `financial_datasets-0.1.4.tar` & `financial_datasets-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1068 2024-03-29 00:57:03.662287 financial_datasets-0.1.4/LICENSE
--rw-r--r--   0        0        0     3077 2024-04-06 13:31:16.695273 financial_datasets-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-03-29 00:57:47.261649 financial_datasets-0.1.4/financial_datasets/__init__.py
--rw-r--r--   0        0        0      201 2024-04-03 12:06:00.779549 financial_datasets-0.1.4/financial_datasets/dataset.py
--rw-r--r--   0        0        0      687 2024-04-07 22:00:07.915325 financial_datasets-0.1.4/financial_datasets/filings.py
--rw-r--r--   0        0        0     6619 2024-04-07 22:01:00.814058 financial_datasets-0.1.4/financial_datasets/generator.py
--rw-r--r--   0        0        0      642 2024-04-07 22:02:05.481404 financial_datasets-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3931 1970-01-01 00:00:00.000000 financial_datasets-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-29 00:57:03.662287 financial_datasets-0.1.6/LICENSE
+-rw-r--r--   0        0        0     4307 2024-04-10 12:21:55.239116 financial_datasets-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-03-29 00:57:47.261649 financial_datasets-0.1.6/financial_datasets/__init__.py
+-rw-r--r--   0        0        0      201 2024-04-03 12:06:00.779549 financial_datasets-0.1.6/financial_datasets/dataset.py
+-rw-r--r--   0        0        0      687 2024-04-07 22:00:07.915325 financial_datasets-0.1.6/financial_datasets/filings.py
+-rw-r--r--   0        0        0     6616 2024-04-10 12:02:39.104303 financial_datasets-0.1.6/financial_datasets/generator.py
+-rw-r--r--   0        0        0     1457 2024-04-10 12:02:30.195140 financial_datasets-0.1.6/financial_datasets/prompts.py
+-rw-r--r--   0        0        0      660 2024-04-10 12:22:09.681746 financial_datasets-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5200 1970-01-01 00:00:00.000000 financial_datasets-0.1.6/PKG-INFO
```

### Comparing `financial_datasets-0.1.4/LICENSE` & `financial_datasets-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `financial_datasets-0.1.4/README.md` & `financial_datasets-0.1.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,193 +1,270 @@
 00000000: 2320 4669 6e61 6e63 6961 6c20 4461 7461  # Financial Data
 00000010: 7365 7473 20f0 9fa7 aa0a 0a46 696e 616e  sets ......Finan
 00000020: 6369 616c 2044 6174 6173 6574 7320 6973  cial Datasets is
 00000030: 2061 6e20 6f70 656e 2d73 6f75 7263 6520   an open-source 
 00000040: 5079 7468 6f6e 206c 6962 7261 7279 200a  Python library .
-00000050: 7468 6174 2061 6c6c 6f77 7320 6465 7665  that allows deve
-00000060: 6c6f 7065 7273 2074 6f20 6372 6561 7465  lopers to create
-00000070: 2073 796e 7468 6574 6963 2066 696e 616e   synthetic finan
-00000080: 6369 616c 2064 6174 6173 6574 730a 7573  cial datasets.us
-00000090: 696e 6720 4c61 7267 6520 4c61 6e67 7561  ing Large Langua
-000000a0: 6765 204d 6f64 656c 7320 284c 4c4d 7329  ge Models (LLMs)
-000000b0: 2e20 5769 7468 2074 6869 7320 6c69 6272  . With this libr
-000000c0: 6172 792c 0a79 6f75 2063 616e 2067 656e  ary,.you can gen
-000000d0: 6572 6174 6520 7265 616c 6973 7469 6320  erate realistic 
-000000e0: 6669 6e61 6e63 6961 6c20 6461 7461 7365  financial datase
-000000f0: 7473 2062 6173 6564 206f 6e20 5345 4320  ts based on SEC 
-00000100: 6669 6c69 6e67 730a 7375 6368 2061 7320  filings.such as 
-00000110: 3130 2d4b 732c 2031 302d 5173 2c20 616e  10-Ks, 10-Qs, an
-00000120: 6420 6f74 6865 7220 6669 6e61 6e63 6961  d other financia
-00000130: 6c20 7265 706f 7274 732e 0a0a 5b21 5b54  l reports...[![T
-00000140: 7769 7474 6572 2046 6f6c 6c6f 775d 2868  witter Follow](h
-00000150: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000160: 6473 2e69 6f2f 7477 6974 7465 722f 666f  ds.io/twitter/fo
-00000170: 6c6c 6f77 2f76 6972 6174 7474 3f73 7479  llow/virattt?sty
-00000180: 6c65 3d73 6f63 6961 6c29 5d28 6874 7470  le=social)](http
-00000190: 733a 2f2f 7477 6974 7465 722e 636f 6d2f  s://twitter.com/
-000001a0: 7669 7261 7474 7429 0a0a 2323 2046 6561  virattt)..## Fea
-000001b0: 7475 7265 730a 0a2d 2047 656e 6572 6174  tures..- Generat
-000001c0: 6520 7379 6e74 6865 7469 6320 6669 6e61  e synthetic fina
-000001d0: 6e63 6961 6c20 6461 7461 7365 7473 2075  ncial datasets u
-000001e0: 7369 6e67 204c 4c4d 730a 2d20 5375 7070  sing LLMs.- Supp
-000001f0: 6f72 7473 2076 6172 696f 7573 2053 4543  orts various SEC
-00000200: 2066 696c 696e 6773 2028 3130 2d4b 732c   filings (10-Ks,
-00000210: 2031 302d 5173 2c20 6574 632e 290a 2d20   10-Qs, etc.).- 
-00000220: 4561 7379 2069 6e74 6567 7261 7469 6f6e  Easy integration
-00000230: 2077 6974 6820 5079 7468 6f6e 2070 726f   with Python pro
-00000240: 6a65 6374 730a 2d20 4375 7374 6f6d 697a  jects.- Customiz
-00000250: 6162 6c65 2064 6174 6120 6765 6e65 7261  able data genera
-00000260: 7469 6f6e 206f 7074 696f 6e73 0a0a 2323  tion options..##
-00000270: 2055 7361 6765 0a0a 2a2a 4578 616d 706c   Usage..**Exampl
-00000280: 6520 636f 6465 3a2a 2a0a 6060 6070 7974  e code:**.```pyt
-00000290: 686f 6e0a 6672 6f6d 2066 696e 616e 6369  hon.from financi
-000002a0: 616c 5f64 6174 6173 6574 732e 6765 6e65  al_datasets.gene
-000002b0: 7261 746f 7220 696d 706f 7274 2044 6174  rator import Dat
-000002c0: 6173 6574 4765 6e65 7261 746f 720a 0a74  asetGenerator..t
-000002d0: 6578 7473 203d 202e 2e2e 2020 2320 4c69  exts = ...  # Li
-000002e0: 7374 206f 6620 7465 7874 7320 6672 6f6d  st of texts from
-000002f0: 2053 4543 2066 696c 696e 670a 6765 6e65   SEC filing.gene
-00000300: 7261 746f 7220 3d20 4461 7461 7365 7447  rator = DatasetG
-00000310: 656e 6572 6174 6f72 280a 2020 206d 6f64  enerator(.   mod
-00000320: 656c 3d22 6770 742d 342d 3031 3235 2d70  el="gpt-4-0125-p
-00000330: 7265 7669 6577 222c 0a20 2020 6170 695f  review",.   api_
-00000340: 6b65 793d 2259 4f55 525f 4f50 454e 4149  key="YOUR_OPENAI
-00000350: 5f41 5049 5f4b 4559 222c 0a29 0a64 6174  _API_KEY",.).dat
-00000360: 6173 6574 203d 2067 656e 6572 6174 6f72  aset = generator
-00000370: 2e67 656e 6572 6174 655f 6672 6f6d 5f74  .generate_from_t
-00000380: 6578 7473 2874 6578 7473 2c20 6d61 785f  exts(texts, max_
-00000390: 7175 6573 7469 6f6e 733d 3130 3029 0a60  questions=100).`
-000003a0: 6060 0a0a 2a2a 4578 616d 706c 6520 6765  ``..**Example ge
-000003b0: 6e65 7261 7465 6420 6461 7461 7365 743a  nerated dataset:
-000003c0: 2a2a 0a60 6060 6a73 6f6e 0a5b 0a20 207b  **.```json.[.  {
-000003d0: 0a20 2020 2022 7175 6573 7469 6f6e 223a  .    "question":
-000003e0: 2022 5768 6174 2077 6173 2041 6972 626e   "What was Airbn
-000003f0: 6227 7320 7265 7665 6e75 6520 696e 2032  b's revenue in 2
-00000400: 3032 333f 222c 0a20 2020 2022 616e 7377  023?",.    "answ
-00000410: 6572 223a 2022 2439 2e39 2062 696c 6c69  er": "$9.9 billi
-00000420: 6f6e 222c 0a20 2020 2022 636f 6e74 6578  on",.    "contex
-00000430: 7422 3a20 2249 6e20 3230 3233 2c20 7265  t": "In 2023, re
-00000440: 7665 6e75 6520 696e 6372 6561 7365 6420  venue increased 
-00000450: 6279 2031 3825 2074 6f20 2439 2e39 2062  by 18% to $9.9 b
-00000460: 696c 6c69 6f6e 2063 6f6d 7061 7265 6420  illion compared 
-00000470: 746f 2032 3032 322c 2070 7269 6d61 7269  to 2022, primari
-00000480: 6c79 2064 7565 2074 6f20 6120 3134 2520  ly due to a 14% 
-00000490: 696e 6372 6561 7365 2069 6e20 4e69 6768  increase in Nigh
-000004a0: 7473 2061 6e64 2045 7870 6572 6965 6e63  ts and Experienc
-000004b0: 6573 2042 6f6f 6b65 6420 6f66 2035 342e  es Booked of 54.
-000004c0: 3520 6d69 6c6c 696f 6e20 636f 6d62 696e  5 million combin
-000004d0: 6564 2077 6974 6820 6869 6768 6572 2061  ed with higher a
-000004e0: 7665 7261 6765 2064 6169 6c79 2072 6174  verage daily rat
-000004f0: 6573 2064 7269 7669 6e67 2061 2031 3625  es driving a 16%
-00000500: 2069 6e63 7265 6173 6520 696e 2047 726f   increase in Gro
-00000510: 7373 2042 6f6f 6b69 6e67 2056 616c 7565  ss Booking Value
-00000520: 206f 6620 2431 302e 3020 6269 6c6c 696f   of $10.0 billio
-00000530: 6e2e 220a 2020 7d2c 0a20 207b 0a20 2020  n.".  },.  {.   
-00000540: 2022 7175 6573 7469 6f6e 223a 2022 4279   "question": "By
-00000550: 2077 6861 7420 7065 7263 656e 7461 6765   what percentage
-00000560: 2064 6964 2041 6972 626e 6227 7320 6e65   did Airbnb's ne
-00000570: 7420 696e 636f 6d65 2069 6e63 7265 6173  t income increas
-00000580: 6520 696e 2032 3032 3320 636f 6d70 6172  e in 2023 compar
-00000590: 6564 2074 6f20 7468 6520 7072 696f 7220  ed to the prior 
-000005a0: 7965 6172 3f22 2c0a 2020 2020 2261 6e73  year?",.    "ans
-000005b0: 7765 7222 3a20 2231 3533 2522 2c0a 2020  wer": "153%",.  
-000005c0: 2020 2263 6f6e 7465 7874 223a 2022 4e65    "context": "Ne
-000005d0: 7420 696e 636f 6d65 2069 6e20 3230 3233  t income in 2023
-000005e0: 2069 6e63 7265 6173 6564 2062 7920 3135   increased by 15
-000005f0: 3325 2074 6f20 2434 2e38 2062 696c 6c69  3% to $4.8 billi
-00000600: 6f6e 2c20 636f 6d70 6172 6564 2074 6f20  on, compared to 
-00000610: 7468 6520 7072 696f 7220 7965 6172 2c20  the prior year, 
-00000620: 6472 6976 656e 2062 7920 6f75 7220 7265  driven by our re
-00000630: 7665 6e75 6520 6772 6f77 7468 2c20 696e  venue growth, in
-00000640: 6372 6561 7365 6420 696e 7465 7265 7374  creased interest
-00000650: 2069 6e63 6f6d 652c 2064 6973 6369 706c   income, discipl
-00000660: 696e 6520 696e 206d 616e 6167 696e 6720  ine in managing 
-00000670: 6f75 7220 636f 7374 2073 7472 7563 7475  our cost structu
-00000680: 7265 2c20 616e 6420 7468 6520 7265 6c65  re, and the rele
-00000690: 6173 6520 6f66 2061 2070 6f72 7469 6f6e  ase of a portion
-000006a0: 206f 6620 6f75 7220 7661 6c75 6174 696f   of our valuatio
-000006b0: 6e20 616c 6c6f 7761 6e63 6520 6f6e 2064  n allowance on d
-000006c0: 6566 6572 7265 6420 7461 7820 6173 7365  eferred tax asse
-000006d0: 7473 206f 6620 2432 2e39 2062 696c 6c69  ts of $2.9 billi
-000006e0: 6f6e 2e22 0a20 207d 0a5d 0a60 6060 0a0a  on.".  }.].```..
-000006f0: 4120 6675 6c6c 2065 6e64 2d74 6f2d 656e  A full end-to-en
-00000700: 6420 636f 6465 2065 7861 6d70 6c65 2063  d code example c
-00000710: 616e 2062 6520 666f 756e 6420 5b68 6572  an be found [her
-00000720: 655d 2868 7474 7073 3a2f 2f63 6f6c 6162  e](https://colab
-00000730: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
-00000740: 2e63 6f6d 2f67 6973 742f 7669 7261 7474  .com/gist/viratt
-00000750: 742f 6639 6235 6130 6165 3832 6363 3063  t/f9b5a0ae82cc0c
-00000760: 6161 6235 3764 6635 6465 6463 3239 3237  aab57df5dedc2927
-00000770: 6339 2f69 6e74 726f 2d66 696e 616e 6369  c9/intro-financi
-00000780: 616c 2d64 6174 6173 6574 732e 6970 796e  al-datasets.ipyn
-00000790: 6229 2e0a 2323 2049 6e73 7461 6c6c 6174  b)..## Installat
-000007a0: 696f 6e0a 0a23 2323 2055 7369 6e67 2070  ion..### Using p
-000007b0: 6970 0a0a 596f 7520 6361 6e20 696e 7374  ip..You can inst
-000007c0: 616c 6c20 7468 6520 4669 6e61 6e63 6961  all the Financia
-000007d0: 6c20 4461 7461 7365 7473 206c 6962 7261  l Datasets libra
-000007e0: 7279 2075 7369 6e67 2070 6970 3a0a 0a60  ry using pip:..`
-000007f0: 6060 0a70 6970 2069 6e73 7461 6c6c 2066  ``.pip install f
-00000800: 696e 616e 6369 616c 2d64 6174 6173 6574  inancial-dataset
-00000810: 730a 6060 600a 0a23 2323 2055 7369 6e67  s.```..### Using
-00000820: 2050 6f65 7472 790a 0a49 6620 796f 7520   Poetry..If you 
-00000830: 7072 6566 6572 2074 6f20 7573 6520 506f  prefer to use Po
-00000840: 6574 7279 2066 6f72 2064 6570 656e 6465  etry for depende
-00000850: 6e63 7920 6d61 6e61 6765 6d65 6e74 2c20  ncy management, 
-00000860: 796f 7520 6361 6e20 6164 6420 4669 6e61  you can add Fina
-00000870: 6e63 6961 6c20 4461 7461 7365 7473 2074  ncial Datasets t
-00000880: 6f20 796f 7572 2070 726f 6a65 6374 3a0a  o your project:.
-00000890: 0a60 6060 0a70 6f65 7472 7920 6164 6420  .```.poetry add 
-000008a0: 6669 6e61 6e63 6961 6c2d 6461 7461 7365  financial-datase
-000008b0: 7473 0a60 6060 0a0a 2323 2320 4672 6f6d  ts.```..### From
-000008c0: 2074 6865 2052 6570 6f73 6974 6f72 790a   the Repository.
-000008d0: 0a49 6620 796f 7520 7761 6e74 2074 6f20  .If you want to 
-000008e0: 696e 7374 616c 6c20 7468 6520 6c69 6272  install the libr
-000008f0: 6172 7920 6469 7265 6374 6c79 2066 726f  ary directly fro
-00000900: 6d20 7468 6520 7265 706f 7369 746f 7279  m the repository
-00000910: 2c20 666f 6c6c 6f77 2074 6865 7365 2073  , follow these s
-00000920: 7465 7073 3a0a 0a31 2e20 436c 6f6e 6520  teps:..1. Clone 
-00000930: 7468 6520 7265 706f 7369 746f 7279 3a0a  the repository:.
-00000940: 2020 2060 6060 0a20 2020 6769 7420 636c     ```.   git cl
-00000950: 6f6e 6520 6874 7470 733a 2f2f 6769 7468  one https://gith
-00000960: 7562 2e63 6f6d 2f79 6f75 7275 7365 726e  ub.com/yourusern
-00000970: 616d 652f 6669 6e61 6e63 6961 6c2d 6461  ame/financial-da
-00000980: 7461 7365 7473 2e67 6974 0a20 2020 6060  tasets.git.   ``
-00000990: 600a 0a32 2e20 4e61 7669 6761 7465 2074  `..2. Navigate t
-000009a0: 6f20 7468 6520 7072 6f6a 6563 7420 6469  o the project di
-000009b0: 7265 6374 6f72 793a 0a20 2020 6060 600a  rectory:.   ```.
-000009c0: 2020 2063 6420 6669 6e61 6e63 6961 6c2d     cd financial-
-000009d0: 6461 7461 7365 7473 0a20 2020 6060 600a  datasets.   ```.
-000009e0: 2020 200a 332e 2049 6e73 7461 6c6c 2074     .3. Install t
-000009f0: 6865 2064 6570 656e 6465 6e63 6965 7320  he dependencies 
-00000a00: 7573 696e 6720 506f 6574 7279 3a0a 2020  using Poetry:.  
-00000a10: 2060 6060 0a20 2020 706f 6574 7279 2069   ```.   poetry i
-00000a20: 6e73 7461 6c6c 0a20 2020 6060 600a 0a34  nstall.   ```..4
-00000a30: 2e20 596f 7520 6361 6e20 6e6f 7720 7573  . You can now us
-00000a40: 6520 7468 6520 6c69 6272 6172 7920 696e  e the library in
-00000a50: 2079 6f75 7220 5079 7468 6f6e 2070 726f   your Python pro
-00000a60: 6a65 6374 732e 0a0a 2323 2043 6f6e 7472  jects...## Contr
-00000a70: 6962 7574 696e 670a 0a43 6f6e 7472 6962  ibuting..Contrib
-00000a80: 7574 696f 6e73 2061 7265 2077 656c 636f  utions are welco
-00000a90: 6d65 2120 4966 2079 6f75 2066 696e 6420  me! If you find 
-00000aa0: 616e 7920 6973 7375 6573 206f 7220 6861  any issues or ha
-00000ab0: 7665 2073 7567 6765 7374 696f 6e73 2066  ve suggestions f
-00000ac0: 6f72 2069 6d70 726f 7665 6d65 6e74 732c  or improvements,
-00000ad0: 200a 706c 6561 7365 206f 7065 6e20 616e   .please open an
-00000ae0: 2069 7373 7565 206f 7220 7375 626d 6974   issue or submit
-00000af0: 2061 2070 756c 6c20 7265 7175 6573 742e   a pull request.
-00000b00: 0a0a 2323 204c 6963 656e 7365 0a0a 5468  ..## License..Th
-00000b10: 6973 2070 726f 6a65 6374 2069 7320 6c69  is project is li
-00000b20: 6365 6e73 6564 2075 6e64 6572 2074 6865  censed under the
-00000b30: 205b 4d49 5420 4c69 6365 6e73 655d 286c   [MIT License](l
-00000b40: 696e 6b2d 746f 2d6c 6963 656e 7365 2d66  ink-to-license-f
-00000b50: 696c 6529 2e0a 0a23 2320 436f 6e74 7269  ile)...## Contri
-00000b60: 6275 746f 7273 0a0a 3c61 2068 7265 663d  butors..<a href=
-00000b70: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00000b80: 636f 6d2f 7669 7261 7474 742f 6669 6e61  com/virattt/fina
-00000b90: 6e63 6961 6c2d 6461 7461 7365 7473 2f67  ncial-datasets/g
-00000ba0: 7261 7068 732f 636f 6e74 7269 6275 746f  raphs/contributo
-00000bb0: 7273 223e 0a20 203c 696d 6720 7372 633d  rs">.  <img src=
-00000bc0: 2268 7474 7073 3a2f 2f63 6f6e 7472 6962  "https://contrib
-00000bd0: 2e72 6f63 6b73 2f69 6d61 6765 3f72 6570  .rocks/image?rep
-00000be0: 6f3d 7669 7261 7474 742f 6669 6e61 6e63  o=virattt/financ
-00000bf0: 6961 6c2d 6461 7461 7365 7473 2220 2f3e  ial-datasets" />
-00000c00: 0a3c 2f61 3e                             .</a>
+00000050: 7468 6174 206c 6574 7320 796f 7520 6372  that lets you cr
+00000060: 6561 7465 2071 7565 7374 696f 6e20 2620  eate question & 
+00000070: 616e 7377 6572 2066 696e 616e 6369 616c  answer financial
+00000080: 2064 6174 6173 6574 730a 7573 696e 6720   datasets.using 
+00000090: 4c61 7267 6520 4c61 6e67 7561 6765 204d  Large Language M
+000000a0: 6f64 656c 7320 284c 4c4d 7329 2e20 5769  odels (LLMs). Wi
+000000b0: 7468 2074 6869 7320 6c69 6272 6172 792c  th this library,
+000000c0: 0a79 6f75 2063 616e 2065 6173 696c 7920  .you can easily 
+000000d0: 6765 6e65 7261 7465 2072 6561 6c69 7374  generate realist
+000000e0: 6963 2066 696e 616e 6369 616c 2064 6174  ic financial dat
+000000f0: 6173 6574 7320 6672 6f6d 2061 2031 302d  asets from a 10-
+00000100: 4b2c 200a 3130 2d51 2c20 5044 462c 2061  K, .10-Q, PDF, a
+00000110: 6e64 206f 7468 6572 2066 696e 616e 6369  nd other financi
+00000120: 616c 2074 6578 7473 2e0a 0a5b 215b 5477  al texts...[![Tw
+00000130: 6974 7465 7220 466f 6c6c 6f77 5d28 6874  itter Follow](ht
+00000140: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000150: 732e 696f 2f74 7769 7474 6572 2f66 6f6c  s.io/twitter/fol
+00000160: 6c6f 772f 7669 7261 7474 743f 7374 796c  low/virattt?styl
+00000170: 653d 736f 6369 616c 295d 2868 7474 7073  e=social)](https
+00000180: 3a2f 2f74 7769 7474 6572 2e63 6f6d 2f76  ://twitter.com/v
+00000190: 6972 6174 7474 290a 0a23 2320 4665 6174  irattt)..## Feat
+000001a0: 7572 6573 0a0a 2d20 4765 6e65 7261 7465  ures..- Generate
+000001b0: 2073 796e 7468 6574 6963 2066 696e 616e   synthetic finan
+000001c0: 6369 616c 2064 6174 6173 6574 7320 7573  cial datasets us
+000001d0: 696e 6720 4c4c 4d73 0a2d 2053 7570 706f  ing LLMs.- Suppo
+000001e0: 7274 7320 7661 7269 6f75 7320 5345 4320  rts various SEC 
+000001f0: 6669 6c69 6e67 7320 2831 302d 4b73 2c20  filings (10-Ks, 
+00000200: 3130 2d51 732c 2065 7463 2e29 0a2d 2045  10-Qs, etc.).- E
+00000210: 6173 7920 696e 7465 6772 6174 696f 6e20  asy integration 
+00000220: 7769 7468 2050 7974 686f 6e20 7072 6f6a  with Python proj
+00000230: 6563 7473 0a2d 2043 7573 746f 6d69 7a61  ects.- Customiza
+00000240: 626c 6520 6461 7461 2067 656e 6572 6174  ble data generat
+00000250: 696f 6e20 6f70 7469 6f6e 730a 0a23 2320  ion options..## 
+00000260: 5573 6167 650a 0a2a 2a45 7861 6d70 6c65  Usage..**Example
+00000270: 2067 656e 6572 6174 6564 2064 6174 6173   generated datas
+00000280: 6574 3a2a 2a0a 6060 606a 736f 6e0a 5b0a  et:**.```json.[.
+00000290: 2020 7b0a 2020 2020 2271 7565 7374 696f    {.    "questio
+000002a0: 6e22 3a20 2257 6861 7420 7761 7320 4169  n": "What was Ai
+000002b0: 7262 6e62 2773 2072 6576 656e 7565 2069  rbnb's revenue i
+000002c0: 6e20 3230 3233 3f22 2c0a 2020 2020 2261  n 2023?",.    "a
+000002d0: 6e73 7765 7222 3a20 2224 392e 3920 6269  nswer": "$9.9 bi
+000002e0: 6c6c 696f 6e22 2c0a 2020 2020 2263 6f6e  llion",.    "con
+000002f0: 7465 7874 223a 2022 496e 2032 3032 332c  text": "In 2023,
+00000300: 2072 6576 656e 7565 2069 6e63 7265 6173   revenue increas
+00000310: 6564 2062 7920 3138 2520 746f 2024 392e  ed by 18% to $9.
+00000320: 3920 6269 6c6c 696f 6e20 636f 6d70 6172  9 billion compar
+00000330: 6564 2074 6f20 3230 3232 2c20 7072 696d  ed to 2022, prim
+00000340: 6172 696c 7920 6475 6520 746f 2061 2031  arily due to a 1
+00000350: 3425 2069 6e63 7265 6173 6520 696e 204e  4% increase in N
+00000360: 6967 6874 7320 616e 6420 4578 7065 7269  ights and Experi
+00000370: 656e 6365 7320 426f 6f6b 6564 206f 6620  ences Booked of 
+00000380: 3534 2e35 206d 696c 6c69 6f6e 2063 6f6d  54.5 million com
+00000390: 6269 6e65 6420 7769 7468 2068 6967 6865  bined with highe
+000003a0: 7220 6176 6572 6167 6520 6461 696c 7920  r average daily 
+000003b0: 7261 7465 7320 6472 6976 696e 6720 6120  rates driving a 
+000003c0: 3136 2520 696e 6372 6561 7365 2069 6e20  16% increase in 
+000003d0: 4772 6f73 7320 426f 6f6b 696e 6720 5661  Gross Booking Va
+000003e0: 6c75 6520 6f66 2024 3130 2e30 2062 696c  lue of $10.0 bil
+000003f0: 6c69 6f6e 2e22 0a20 207d 2c0a 2020 7b0a  lion.".  },.  {.
+00000400: 2020 2020 2271 7565 7374 696f 6e22 3a20      "question": 
+00000410: 2242 7920 7768 6174 2070 6572 6365 6e74  "By what percent
+00000420: 6167 6520 6469 6420 4169 7262 6e62 2773  age did Airbnb's
+00000430: 206e 6574 2069 6e63 6f6d 6520 696e 6372   net income incr
+00000440: 6561 7365 2069 6e20 3230 3233 2063 6f6d  ease in 2023 com
+00000450: 7061 7265 6420 746f 2074 6865 2070 7269  pared to the pri
+00000460: 6f72 2079 6561 723f 222c 0a20 2020 2022  or year?",.    "
+00000470: 616e 7377 6572 223a 2022 3135 3325 222c  answer": "153%",
+00000480: 0a20 2020 2022 636f 6e74 6578 7422 3a20  .    "context": 
+00000490: 224e 6574 2069 6e63 6f6d 6520 696e 2032  "Net income in 2
+000004a0: 3032 3320 696e 6372 6561 7365 6420 6279  023 increased by
+000004b0: 2031 3533 2520 746f 2024 342e 3820 6269   153% to $4.8 bi
+000004c0: 6c6c 696f 6e2c 2063 6f6d 7061 7265 6420  llion, compared 
+000004d0: 746f 2074 6865 2070 7269 6f72 2079 6561  to the prior yea
+000004e0: 722c 2064 7269 7665 6e20 6279 206f 7572  r, driven by our
+000004f0: 2072 6576 656e 7565 2067 726f 7774 682c   revenue growth,
+00000500: 2069 6e63 7265 6173 6564 2069 6e74 6572   increased inter
+00000510: 6573 7420 696e 636f 6d65 2c20 6469 7363  est income, disc
+00000520: 6970 6c69 6e65 2069 6e20 6d61 6e61 6769  ipline in managi
+00000530: 6e67 206f 7572 2063 6f73 7420 7374 7275  ng our cost stru
+00000540: 6374 7572 652c 2061 6e64 2074 6865 2072  cture, and the r
+00000550: 656c 6561 7365 206f 6620 6120 706f 7274  elease of a port
+00000560: 696f 6e20 6f66 206f 7572 2076 616c 7561  ion of our valua
+00000570: 7469 6f6e 2061 6c6c 6f77 616e 6365 206f  tion allowance o
+00000580: 6e20 6465 6665 7272 6564 2074 6178 2061  n deferred tax a
+00000590: 7373 6574 7320 6f66 2024 322e 3920 6269  ssets of $2.9 bi
+000005a0: 6c6c 696f 6e2e 220a 2020 7d0a 5d0a 6060  llion.".  }.].``
+000005b0: 600a 0a2a 2a45 7861 6d70 6c65 2023 3120  `..**Example #1 
+000005c0: 2d20 6765 6e65 7261 7465 2066 726f 6d20  - generate from 
+000005d0: 616e 7920 7465 7874 733a 2a2a 0a0a 4d6f  any texts:**..Mo
+000005e0: 7374 2066 6c65 7869 626c 6520 6f70 7469  st flexible opti
+000005f0: 6f6e 2e20 2047 656e 6572 6174 6573 2064  on.  Generates d
+00000600: 6174 6173 6574 2075 7369 6e67 2061 206c  ataset using a l
+00000610: 6973 7420 6f66 2073 7472 696e 6720 6074  ist of string `t
+00000620: 6578 7473 602e 2043 6f6c 6162 2063 6f64  exts`. Colab cod
+00000630: 6520 6578 616d 706c 6520 5b68 6572 655d  e example [here]
+00000640: 2868 7474 7073 3a2f 2f63 6f6c 6162 2e72  (https://colab.r
+00000650: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
+00000660: 6f6d 2f67 6973 742f 7669 7261 7474 742f  om/gist/virattt/
+00000670: 6639 6235 6130 6165 3832 6363 3063 6161  f9b5a0ae82cc0caa
+00000680: 6235 3764 6635 6465 6463 3239 3237 6339  b57df5dedc2927c9
+00000690: 2f69 6e74 726f 2d66 696e 616e 6369 616c  /intro-financial
+000006a0: 2d64 6174 6173 6574 732e 6970 796e 6229  -datasets.ipynb)
+000006b0: 2e0a 0a60 6060 7079 7468 6f6e 0a66 726f  ...```python.fro
+000006c0: 6d20 6669 6e61 6e63 6961 6c5f 6461 7461  m financial_data
+000006d0: 7365 7473 2e67 656e 6572 6174 6f72 2069  sets.generator i
+000006e0: 6d70 6f72 7420 4461 7461 7365 7447 656e  mport DatasetGen
+000006f0: 6572 6174 6f72 0a0a 7465 7874 7320 3d20  erator..texts = 
+00000700: 2e2e 2e20 2023 204c 6973 7420 6f66 2074  ...  # List of t
+00000710: 6578 7473 2066 726f 6d20 5345 4320 6669  exts from SEC fi
+00000720: 6c69 6e67 0a67 656e 6572 6174 6f72 203d  ling.generator =
+00000730: 2044 6174 6173 6574 4765 6e65 7261 746f   DatasetGenerato
+00000740: 7228 6d6f 6465 6c3d 2267 7074 2d34 2d30  r(model="gpt-4-0
+00000750: 3132 352d 7072 6576 6965 7722 2c20 6170  125-preview", ap
+00000760: 695f 6b65 793d 2279 6f75 722d 6f70 656e  i_key="your-open
+00000770: 6169 2d6b 6579 2229 0a0a 2320 4765 6e65  ai-key")..# Gene
+00000780: 7261 7465 2064 6174 6173 6574 2066 726f  rate dataset fro
+00000790: 6d20 7465 7874 730a 6461 7461 7365 7420  m texts.dataset 
+000007a0: 3d20 6765 6e65 7261 746f 722e 6765 6e65  = generator.gene
+000007b0: 7261 7465 5f66 726f 6d5f 7465 7874 7328  rate_from_texts(
+000007c0: 0a20 2020 7465 7874 733d 7465 7874 732c  .   texts=texts,
+000007d0: 200a 2020 206d 6178 5f71 7565 7374 696f   .   max_questio
+000007e0: 6e73 3d31 3030 2c0a 290a 6060 600a 0a2a  ns=100,.).```..*
+000007f0: 2a45 7861 6d70 6c65 2023 3220 2d20 6765  *Example #2 - ge
+00000800: 6e65 7261 7465 2066 726f 6d20 3130 2d4b  nerate from 10-K
+00000810: 3a2a 2a0a 0a47 656e 6572 6174 6520 6120  :**..Generate a 
+00000820: 6461 7461 7365 7420 7573 696e 6720 6120  dataset using a 
+00000830: 6074 6963 6b65 7260 2061 6e64 2060 7965  `ticker` and `ye
+00000840: 6172 602e 2020 436f 6c61 6220 636f 6465  ar`.  Colab code
+00000850: 2065 7861 6d70 6c65 205b 6865 7265 5d28   example [here](
+00000860: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
+00000870: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
+00000880: 6d2f 6769 7374 2f76 6972 6174 7474 2f37  m/gist/virattt/7
+00000890: 3433 3837 3265 3134 3330 3334 3938 3764  43872e143034987d
+000008a0: 3230 6536 6136 6337 6262 3964 3061 312f  20e6a6c7bb9d0a1/
+000008b0: 696e 7472 6f2d 6669 6e61 6e63 6961 6c2d  intro-financial-
+000008c0: 6461 7461 7365 7473 2e69 7079 6e62 292e  datasets.ipynb).
+000008d0: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+000008e0: 2066 696e 616e 6369 616c 5f64 6174 6173   financial_datas
+000008f0: 6574 732e 6765 6e65 7261 746f 7220 696d  ets.generator im
+00000900: 706f 7274 2044 6174 6173 6574 4765 6e65  port DatasetGene
+00000910: 7261 746f 720a 0a74 6578 7473 203d 202e  rator..texts = .
+00000920: 2e2e 2020 2320 4c69 7374 206f 6620 7465  ..  # List of te
+00000930: 7874 7320 6672 6f6d 2053 4543 2066 696c  xts from SEC fil
+00000940: 696e 670a 6765 6e65 7261 746f 7220 3d20  ing.generator = 
+00000950: 4461 7461 7365 7447 656e 6572 6174 6f72  DatasetGenerator
+00000960: 286d 6f64 656c 3d22 6770 742d 342d 3031  (model="gpt-4-01
+00000970: 3235 2d70 7265 7669 6577 222c 2061 7069  25-preview", api
+00000980: 5f6b 6579 3d22 796f 7572 2d6f 7065 6e61  _key="your-opena
+00000990: 692d 6b65 7922 290a 0a23 2047 656e 6572  i-key")..# Gener
+000009a0: 6174 6520 6461 7461 7365 7420 6672 6f6d  ate dataset from
+000009b0: 2031 302d 4b0a 6461 7461 7365 7420 3d20   10-K.dataset = 
+000009c0: 6765 6e65 7261 746f 722e 6765 6e65 7261  generator.genera
+000009d0: 7465 5f66 726f 6d5f 3130 4b28 0a20 2020  te_from_10K(.   
+000009e0: 7469 636b 6572 3d22 4141 504c 222c 0a20  ticker="AAPL",. 
+000009f0: 2020 7965 6172 3d32 3032 332c 0a20 2020    year=2023,.   
+00000a00: 6d61 785f 7175 6573 7469 6f6e 733d 3130  max_questions=10
+00000a10: 302c 0a29 0a60 6060 0a0a 2a2a 4578 616d  0,.).```..**Exam
+00000a20: 706c 6520 2333 202d 2067 656e 6572 6174  ple #3 - generat
+00000a30: 6520 6672 6f6d 2050 4446 3a2a 2a0a 0a47  e from PDF:**..G
+00000a40: 656e 6572 6174 6520 6120 6461 7461 7365  enerate a datase
+00000a50: 7420 7573 696e 6720 6120 5044 4620 6075  t using a PDF `u
+00000a60: 726c 6020 6f6e 6c79 2e20 2043 6f6c 6162  rl` only.  Colab
+00000a70: 2063 6f64 6520 6578 616d 706c 6520 5b68   code example [h
+00000a80: 6572 655d 2868 7474 7073 3a2f 2f63 6f6c  ere](https://col
+00000a90: 6162 2e72 6573 6561 7263 682e 676f 6f67  ab.research.goog
+00000aa0: 6c65 2e63 6f6d 2f67 6973 742f 7669 7261  le.com/gist/vira
+00000ab0: 7474 742f 6230 3434 3432 6565 3763 3663  ttt/b04442ee7c6c
+00000ac0: 3064 3062 6233 6339 3337 3161 6632 3238  0d0bb3c9371af228
+00000ad0: 3361 3230 2f69 6e74 726f 2d66 696e 616e  3a20/intro-finan
+00000ae0: 6369 616c 2d64 6174 6173 6574 732e 6970  cial-datasets.ip
+00000af0: 796e 6229 2e0a 0a60 6060 7079 7468 6f6e  ynb)...```python
+00000b00: 0a66 726f 6d20 6669 6e61 6e63 6961 6c5f  .from financial_
+00000b10: 6461 7461 7365 7473 2e67 656e 6572 6174  datasets.generat
+00000b20: 6f72 2069 6d70 6f72 7420 4461 7461 7365  or import Datase
+00000b30: 7447 656e 6572 6174 6f72 0a0a 7465 7874  tGenerator..text
+00000b40: 7320 3d20 2e2e 2e20 2023 204c 6973 7420  s = ...  # List 
+00000b50: 6f66 2074 6578 7473 2066 726f 6d20 5345  of texts from SE
+00000b60: 4320 6669 6c69 6e67 0a67 656e 6572 6174  C filing.generat
+00000b70: 6f72 203d 2044 6174 6173 6574 4765 6e65  or = DatasetGene
+00000b80: 7261 746f 7228 6d6f 6465 6c3d 2267 7074  rator(model="gpt
+00000b90: 2d34 2d30 3132 352d 7072 6576 6965 7722  -4-0125-preview"
+00000ba0: 2c20 6170 695f 6b65 793d 2279 6f75 722d  , api_key="your-
+00000bb0: 6f70 656e 6169 2d6b 6579 2229 0a0a 2320  openai-key")..# 
+00000bc0: 4765 6e65 7261 7465 2064 6174 6173 6574  Generate dataset
+00000bd0: 2066 726f 6d20 5044 4620 7572 6c0a 6461   from PDF url.da
+00000be0: 7461 7365 7420 3d20 6765 6e65 7261 746f  taset = generato
+00000bf0: 722e 6765 6e65 7261 7465 5f66 726f 6d5f  r.generate_from_
+00000c00: 7064 6628 0a20 2020 7572 6c3d 2268 7474  pdf(.   url="htt
+00000c10: 7073 3a2f 2f77 7777 2e62 6572 6b73 6869  ps://www.berkshi
+00000c20: 7265 6861 7468 6177 6179 2e63 6f6d 2f6c  rehathaway.com/l
+00000c30: 6574 7465 7273 2f32 3032 336c 7472 2e70  etters/2023ltr.p
+00000c40: 6466 222c 0a20 2020 6d61 785f 7175 6573  df",.   max_ques
+00000c50: 7469 6f6e 733d 3130 302c 0a29 0a60 6060  tions=100,.).```
+00000c60: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
+00000c70: 6e0a 0a23 2323 2055 7369 6e67 2070 6970  n..### Using pip
+00000c80: 0a0a 596f 7520 6361 6e20 696e 7374 616c  ..You can instal
+00000c90: 6c20 7468 6520 4669 6e61 6e63 6961 6c20  l the Financial 
+00000ca0: 4461 7461 7365 7473 206c 6962 7261 7279  Datasets library
+00000cb0: 2075 7369 6e67 2070 6970 3a0a 0a60 6060   using pip:..```
+00000cc0: 0a70 6970 2069 6e73 7461 6c6c 2066 696e  .pip install fin
+00000cd0: 616e 6369 616c 2d64 6174 6173 6574 730a  ancial-datasets.
+00000ce0: 6060 600a 0a23 2323 2055 7369 6e67 2050  ```..### Using P
+00000cf0: 6f65 7472 790a 0a49 6620 796f 7520 7072  oetry..If you pr
+00000d00: 6566 6572 2074 6f20 7573 6520 506f 6574  efer to use Poet
+00000d10: 7279 2066 6f72 2064 6570 656e 6465 6e63  ry for dependenc
+00000d20: 7920 6d61 6e61 6765 6d65 6e74 2c20 796f  y management, yo
+00000d30: 7520 6361 6e20 6164 6420 4669 6e61 6e63  u can add Financ
+00000d40: 6961 6c20 4461 7461 7365 7473 2074 6f20  ial Datasets to 
+00000d50: 796f 7572 2070 726f 6a65 6374 3a0a 0a60  your project:..`
+00000d60: 6060 0a70 6f65 7472 7920 6164 6420 6669  ``.poetry add fi
+00000d70: 6e61 6e63 6961 6c2d 6461 7461 7365 7473  nancial-datasets
+00000d80: 0a60 6060 0a0a 2323 2320 4672 6f6d 2074  .```..### From t
+00000d90: 6865 2052 6570 6f73 6974 6f72 790a 0a49  he Repository..I
+00000da0: 6620 796f 7520 7761 6e74 2074 6f20 696e  f you want to in
+00000db0: 7374 616c 6c20 7468 6520 6c69 6272 6172  stall the librar
+00000dc0: 7920 6469 7265 6374 6c79 2066 726f 6d20  y directly from 
+00000dd0: 7468 6520 7265 706f 7369 746f 7279 2c20  the repository, 
+00000de0: 666f 6c6c 6f77 2074 6865 7365 2073 7465  follow these ste
+00000df0: 7073 3a0a 0a31 2e20 436c 6f6e 6520 7468  ps:..1. Clone th
+00000e00: 6520 7265 706f 7369 746f 7279 3a0a 2020  e repository:.  
+00000e10: 2060 6060 0a20 2020 6769 7420 636c 6f6e   ```.   git clon
+00000e20: 6520 6874 7470 733a 2f2f 6769 7468 7562  e https://github
+00000e30: 2e63 6f6d 2f79 6f75 7275 7365 726e 616d  .com/yourusernam
+00000e40: 652f 6669 6e61 6e63 6961 6c2d 6461 7461  e/financial-data
+00000e50: 7365 7473 2e67 6974 0a20 2020 6060 600a  sets.git.   ```.
+00000e60: 0a32 2e20 4e61 7669 6761 7465 2074 6f20  .2. Navigate to 
+00000e70: 7468 6520 7072 6f6a 6563 7420 6469 7265  the project dire
+00000e80: 6374 6f72 793a 0a20 2020 6060 600a 2020  ctory:.   ```.  
+00000e90: 2063 6420 6669 6e61 6e63 6961 6c2d 6461   cd financial-da
+00000ea0: 7461 7365 7473 0a20 2020 6060 600a 2020  tasets.   ```.  
+00000eb0: 200a 332e 2049 6e73 7461 6c6c 2074 6865   .3. Install the
+00000ec0: 2064 6570 656e 6465 6e63 6965 7320 7573   dependencies us
+00000ed0: 696e 6720 506f 6574 7279 3a0a 2020 2060  ing Poetry:.   `
+00000ee0: 6060 0a20 2020 706f 6574 7279 2069 6e73  ``.   poetry ins
+00000ef0: 7461 6c6c 0a20 2020 6060 600a 0a34 2e20  tall.   ```..4. 
+00000f00: 596f 7520 6361 6e20 6e6f 7720 7573 6520  You can now use 
+00000f10: 7468 6520 6c69 6272 6172 7920 696e 2079  the library in y
+00000f20: 6f75 7220 5079 7468 6f6e 2070 726f 6a65  our Python proje
+00000f30: 6374 732e 0a0a 2323 2043 6f6e 7472 6962  cts...## Contrib
+00000f40: 7574 696e 670a 0a43 6f6e 7472 6962 7574  uting..Contribut
+00000f50: 696f 6e73 2061 7265 2077 656c 636f 6d65  ions are welcome
+00000f60: 2120 4966 2079 6f75 2066 696e 6420 616e  ! If you find an
+00000f70: 7920 6973 7375 6573 206f 7220 6861 7665  y issues or have
+00000f80: 2073 7567 6765 7374 696f 6e73 2066 6f72   suggestions for
+00000f90: 2069 6d70 726f 7665 6d65 6e74 732c 200a   improvements, .
+00000fa0: 706c 6561 7365 206f 7065 6e20 616e 2069  please open an i
+00000fb0: 7373 7565 206f 7220 7375 626d 6974 2061  ssue or submit a
+00000fc0: 2070 756c 6c20 7265 7175 6573 742e 0a0a   pull request...
+00000fd0: 2323 204c 6963 656e 7365 0a0a 5468 6973  ## License..This
+00000fe0: 2070 726f 6a65 6374 2069 7320 6c69 6365   project is lice
+00000ff0: 6e73 6564 2075 6e64 6572 2074 6865 205b  nsed under the [
+00001000: 4d49 5420 4c69 6365 6e73 655d 286c 696e  MIT License](lin
+00001010: 6b2d 746f 2d6c 6963 656e 7365 2d66 696c  k-to-license-fil
+00001020: 6529 2e0a 0a23 2320 436f 6e74 7269 6275  e)...## Contribu
+00001030: 746f 7273 0a0a 3c61 2068 7265 663d 2268  tors..<a href="h
+00001040: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001050: 6d2f 7669 7261 7474 742f 6669 6e61 6e63  m/virattt/financ
+00001060: 6961 6c2d 6461 7461 7365 7473 2f67 7261  ial-datasets/gra
+00001070: 7068 732f 636f 6e74 7269 6275 746f 7273  phs/contributors
+00001080: 223e 0a20 203c 696d 6720 7372 633d 2268  ">.  <img src="h
+00001090: 7474 7073 3a2f 2f63 6f6e 7472 6962 2e72  ttps://contrib.r
+000010a0: 6f63 6b73 2f69 6d61 6765 3f72 6570 6f3d  ocks/image?repo=
+000010b0: 7669 7261 7474 742f 6669 6e61 6e63 6961  virattt/financia
+000010c0: 6c2d 6461 7461 7365 7473 2220 2f3e 0a3c  l-datasets" />.<
+000010d0: 2f61 3e                                  /a>
```

### Comparing `financial_datasets-0.1.4/financial_datasets/filings.py` & `financial_datasets-0.1.6/financial_datasets/filings.py`

 * *Files identical despite different names*

### Comparing `financial_datasets-0.1.4/financial_datasets/generator.py` & `financial_datasets-0.1.6/financial_datasets/generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,23 @@
 import re
 import time
+from io import BytesIO
 from typing import List
 
+import requests
+from PyPDF2 import PdfReader
 from edgar import Company, set_identity
 from instructor import patch
 from langchain_text_splitters import TokenTextSplitter
 from openai import OpenAI
 from tqdm import tqdm
 
 from financial_datasets.dataset import DatasetItem, Dataset
 from financial_datasets.filings import filter_filings
-
-system_prompt = """
-You are an expert at understanding and analyzing financial documents. 
-Your role is to generate question and ground truth answer pairs based on the provided financial text. 
-The types of texts you will be working with include 10-Ks, 10-Qs, earnings call transcripts, and other financial documents.
-
-When generating questions and answers, adhere to the following guidelines:
-1. Your ground truth answers must be directly derived from the content within the provided text. Do not make up, hallucinate, or generate answers that are not explicitly supported by the given text.
-2. Ensure that the questions you generate are relevant to the financial context and can be answered based on the information provided in the text.
-3. Include the relevant 'context' paragraph from which you generated each question and ground truth answer pair. The 'context' paragraph MUST contain the specific information that supports the ground truth answer.
-4. If the provided text does not contain sufficient information to generate a question-answer pair, do not attempt to create one.
-5. Your responses should be in the following format:
-   Question: [Generated question]
-   Answer: [Ground truth answer]
-   Context: [Relevant paragraph from the text that supports the answer]
-
-Remember, your primary objective is to create accurate, grounded, and contextually relevant question-answer pairs while strictly avoiding any fabrication or speculation.
-"""
+from financial_datasets.prompts import default_prompt
 
 default_sec_identity = "gary gary@financialdatasets.org"
 
 
 class DatasetGenerator:
     def __init__(self, model: str, api_key: str):
         # Ensure model begins with gpt-
@@ -71,43 +57,85 @@
                     current_max_questions += 1
 
                 # Generate questions
                 response = self._client.chat.completions.create(
                     model=self._model,
                     response_model=Dataset,
                     messages=[
-                        {"role": "system", "content": system_prompt},
+                        {"role": "system", "content": default_prompt},
                         {"role": "user", "content": f"Generate {current_max_questions} questions for the following block of text: {text}"}
                     ],
                 )
 
                 # Add the generated items to our total list of questions
                 items.extend(response.items)
 
                 # Update the progress bar by the number of questions generated
                 progress_bar.update(len(response.items))
 
                 # Stop generating questions if we have reached the maximum number of questions
                 if len(items) == max_questions:
                     break
-                    
+
             except Exception as e:
                 print(f"Failed to generate questions for batch {index + 1}: {e}")
                 continue
 
             # Sleep for 1 second to avoid overloading the LLM
             time.sleep(1)
 
         # Ensure the progress bar is closed
         progress_bar.close()
 
         return Dataset(
             items=items,
         )
 
+    def generate_from_pdf(
+        self,
+        url: str,
+        max_questions=10,
+        **kwargs,
+    ) -> Dataset:
+        """
+        Generate questions from a PDF file.
+
+        :param url: The URL of the PDF file.
+        :param max_questions: Maximum number of questions to generate.
+        :param kwargs: Additional arguments like chunk_size, chunk_overlap, etc.
+        :return: Dataset containing the generated questions.
+        """
+        # Download the PDF file
+        response = requests.get(url)
+        pdf_file = BytesIO(response.content)
+
+        # Extract text from the PDF file
+        reader = PdfReader(pdf_file)
+        text = ""
+        for page in reader.pages:
+            text += page.extract_text()
+
+        # Remove any newline characters
+        text = text.replace("\n", " ")
+
+        # Chunk the text to prevent exceeding the context window of models at the question generation step.
+        chunk_size = kwargs.get("chunk_size", 1024)
+        chunk_overlap = kwargs.get("chunk_overlap", 128)
+
+        # Split by tokens
+        token_splitter = TokenTextSplitter(
+            chunk_size=chunk_size,
+            chunk_overlap=chunk_overlap,
+        )
+
+        # Chunk the text
+        texts = token_splitter.split_text(text)
+
+        return self.generate_from_texts(texts=texts, max_questions=max_questions)
+
     def generate_from_10K(
         self,
         ticker: str,
         year: int,
         max_questions=10,
         sec_identity=default_sec_identity,
     ) -> Dataset:
```

### Comparing `financial_datasets-0.1.4/PKG-INFO` & `financial_datasets-0.1.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6669 6e61  : 2.1.Name: fina
 00000020: 6e63 6961 6c2d 6461 7461 7365 7473 0a56  ncial-datasets.V
-00000030: 6572 7369 6f6e 3a20 302e 312e 340a 5375  ersion: 0.1.4.Su
+00000030: 6572 7369 6f6e 3a20 302e 312e 360a 5375  ersion: 0.1.6.Su
 00000040: 6d6d 6172 793a 2046 696e 616e 6369 616c  mmary: Financial
 00000050: 2064 6174 6173 6574 7320 666f 7220 4c4c   datasets for LL
 00000060: 4d73 0a4c 6963 656e 7365 3a20 4d49 540a  Ms.License: MIT.
 00000070: 4175 7468 6f72 3a20 5669 7261 7420 5369  Author: Virat Si
 00000080: 6e67 680a 4175 7468 6f72 2d65 6d61 696c  ngh.Author-email
 00000090: 3a20 7669 7261 7440 7669 7261 742e 6169  : virat@virat.ai
 000000a0: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
@@ -38,209 +38,288 @@
 00000250: 302e 362e 372c 3c30 2e37 2e30 290a 5265  0.6.7,<0.7.0).Re
 00000260: 7175 6972 6573 2d44 6973 743a 206c 616e  quires-Dist: lan
 00000270: 6763 6861 696e 2028 3e3d 302e 312e 3133  gchain (>=0.1.13
 00000280: 2c3c 302e 322e 3029 0a52 6571 7569 7265  ,<0.2.0).Require
 00000290: 732d 4469 7374 3a20 6f70 656e 6169 2028  s-Dist: openai (
 000002a0: 3e3d 312e 3134 2e33 2c3c 322e 302e 3029  >=1.14.3,<2.0.0)
 000002b0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000002c0: 7469 6b74 6f6b 656e 2028 3e3d 302e 362e  tiktoken (>=0.6.
-000002d0: 302c 3c30 2e37 2e30 290a 5265 7175 6972  0,<0.7.0).Requir
-000002e0: 6573 2d44 6973 743a 2074 7164 6d20 283e  es-Dist: tqdm (>
-000002f0: 3d34 2e36 362e 322c 3c35 2e30 2e30 290a  =4.66.2,<5.0.0).
-00000300: 5265 7175 6972 6573 2d44 6973 743a 2078  Requires-Dist: x
-00000310: 6d6c 746f 6469 6374 2028 3e3d 302e 3133  mltodict (>=0.13
-00000320: 2e30 2c3c 302e 3134 2e30 290a 4465 7363  .0,<0.14.0).Desc
-00000330: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
-00000340: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
-00000350: 6f77 6e0a 0a23 2046 696e 616e 6369 616c  own..# Financial
-00000360: 2044 6174 6173 6574 7320 f09f a7aa 0a0a   Datasets ......
-00000370: 4669 6e61 6e63 6961 6c20 4461 7461 7365  Financial Datase
-00000380: 7473 2069 7320 616e 206f 7065 6e2d 736f  ts is an open-so
-00000390: 7572 6365 2050 7974 686f 6e20 6c69 6272  urce Python libr
-000003a0: 6172 7920 0a74 6861 7420 616c 6c6f 7773  ary .that allows
-000003b0: 2064 6576 656c 6f70 6572 7320 746f 2063   developers to c
-000003c0: 7265 6174 6520 7379 6e74 6865 7469 6320  reate synthetic 
-000003d0: 6669 6e61 6e63 6961 6c20 6461 7461 7365  financial datase
-000003e0: 7473 0a75 7369 6e67 204c 6172 6765 204c  ts.using Large L
-000003f0: 616e 6775 6167 6520 4d6f 6465 6c73 2028  anguage Models (
-00000400: 4c4c 4d73 292e 2057 6974 6820 7468 6973  LLMs). With this
-00000410: 206c 6962 7261 7279 2c0a 796f 7520 6361   library,.you ca
-00000420: 6e20 6765 6e65 7261 7465 2072 6561 6c69  n generate reali
-00000430: 7374 6963 2066 696e 616e 6369 616c 2064  stic financial d
-00000440: 6174 6173 6574 7320 6261 7365 6420 6f6e  atasets based on
-00000450: 2053 4543 2066 696c 696e 6773 0a73 7563   SEC filings.suc
-00000460: 6820 6173 2031 302d 4b73 2c20 3130 2d51  h as 10-Ks, 10-Q
-00000470: 732c 2061 6e64 206f 7468 6572 2066 696e  s, and other fin
-00000480: 616e 6369 616c 2072 6570 6f72 7473 2e0a  ancial reports..
-00000490: 0a5b 215b 5477 6974 7465 7220 466f 6c6c  .[![Twitter Foll
-000004a0: 6f77 5d28 6874 7470 733a 2f2f 696d 672e  ow](https://img.
-000004b0: 7368 6965 6c64 732e 696f 2f74 7769 7474  shields.io/twitt
-000004c0: 6572 2f66 6f6c 6c6f 772f 7669 7261 7474  er/follow/viratt
-000004d0: 743f 7374 796c 653d 736f 6369 616c 295d  t?style=social)]
-000004e0: 2868 7474 7073 3a2f 2f74 7769 7474 6572  (https://twitter
-000004f0: 2e63 6f6d 2f76 6972 6174 7474 290a 0a23  .com/virattt)..#
-00000500: 2320 4665 6174 7572 6573 0a0a 2d20 4765  # Features..- Ge
-00000510: 6e65 7261 7465 2073 796e 7468 6574 6963  nerate synthetic
-00000520: 2066 696e 616e 6369 616c 2064 6174 6173   financial datas
-00000530: 6574 7320 7573 696e 6720 4c4c 4d73 0a2d  ets using LLMs.-
-00000540: 2053 7570 706f 7274 7320 7661 7269 6f75   Supports variou
-00000550: 7320 5345 4320 6669 6c69 6e67 7320 2831  s SEC filings (1
-00000560: 302d 4b73 2c20 3130 2d51 732c 2065 7463  0-Ks, 10-Qs, etc
-00000570: 2e29 0a2d 2045 6173 7920 696e 7465 6772  .).- Easy integr
-00000580: 6174 696f 6e20 7769 7468 2050 7974 686f  ation with Pytho
-00000590: 6e20 7072 6f6a 6563 7473 0a2d 2043 7573  n projects.- Cus
-000005a0: 746f 6d69 7a61 626c 6520 6461 7461 2067  tomizable data g
-000005b0: 656e 6572 6174 696f 6e20 6f70 7469 6f6e  eneration option
-000005c0: 730a 0a23 2320 5573 6167 650a 0a2a 2a45  s..## Usage..**E
-000005d0: 7861 6d70 6c65 2063 6f64 653a 2a2a 0a60  xample code:**.`
-000005e0: 6060 7079 7468 6f6e 0a66 726f 6d20 6669  ``python.from fi
-000005f0: 6e61 6e63 6961 6c5f 6461 7461 7365 7473  nancial_datasets
-00000600: 2e67 656e 6572 6174 6f72 2069 6d70 6f72  .generator impor
-00000610: 7420 4461 7461 7365 7447 656e 6572 6174  t DatasetGenerat
-00000620: 6f72 0a0a 7465 7874 7320 3d20 2e2e 2e20  or..texts = ... 
-00000630: 2023 204c 6973 7420 6f66 2074 6578 7473   # List of texts
-00000640: 2066 726f 6d20 5345 4320 6669 6c69 6e67   from SEC filing
-00000650: 0a67 656e 6572 6174 6f72 203d 2044 6174  .generator = Dat
-00000660: 6173 6574 4765 6e65 7261 746f 7228 0a20  asetGenerator(. 
-00000670: 2020 6d6f 6465 6c3d 2267 7074 2d34 2d30    model="gpt-4-0
-00000680: 3132 352d 7072 6576 6965 7722 2c0a 2020  125-preview",.  
-00000690: 2061 7069 5f6b 6579 3d22 594f 5552 5f4f   api_key="YOUR_O
-000006a0: 5045 4e41 495f 4150 495f 4b45 5922 2c0a  PENAI_API_KEY",.
-000006b0: 290a 6461 7461 7365 7420 3d20 6765 6e65  ).dataset = gene
-000006c0: 7261 746f 722e 6765 6e65 7261 7465 5f66  rator.generate_f
-000006d0: 726f 6d5f 7465 7874 7328 7465 7874 732c  rom_texts(texts,
-000006e0: 206d 6178 5f71 7565 7374 696f 6e73 3d31   max_questions=1
-000006f0: 3030 290a 6060 600a 0a2a 2a45 7861 6d70  00).```..**Examp
-00000700: 6c65 2067 656e 6572 6174 6564 2064 6174  le generated dat
-00000710: 6173 6574 3a2a 2a0a 6060 606a 736f 6e0a  aset:**.```json.
-00000720: 5b0a 2020 7b0a 2020 2020 2271 7565 7374  [.  {.    "quest
-00000730: 696f 6e22 3a20 2257 6861 7420 7761 7320  ion": "What was 
-00000740: 4169 7262 6e62 2773 2072 6576 656e 7565  Airbnb's revenue
-00000750: 2069 6e20 3230 3233 3f22 2c0a 2020 2020   in 2023?",.    
-00000760: 2261 6e73 7765 7222 3a20 2224 392e 3920  "answer": "$9.9 
-00000770: 6269 6c6c 696f 6e22 2c0a 2020 2020 2263  billion",.    "c
-00000780: 6f6e 7465 7874 223a 2022 496e 2032 3032  ontext": "In 202
-00000790: 332c 2072 6576 656e 7565 2069 6e63 7265  3, revenue incre
-000007a0: 6173 6564 2062 7920 3138 2520 746f 2024  ased by 18% to $
-000007b0: 392e 3920 6269 6c6c 696f 6e20 636f 6d70  9.9 billion comp
-000007c0: 6172 6564 2074 6f20 3230 3232 2c20 7072  ared to 2022, pr
-000007d0: 696d 6172 696c 7920 6475 6520 746f 2061  imarily due to a
-000007e0: 2031 3425 2069 6e63 7265 6173 6520 696e   14% increase in
-000007f0: 204e 6967 6874 7320 616e 6420 4578 7065   Nights and Expe
-00000800: 7269 656e 6365 7320 426f 6f6b 6564 206f  riences Booked o
-00000810: 6620 3534 2e35 206d 696c 6c69 6f6e 2063  f 54.5 million c
-00000820: 6f6d 6269 6e65 6420 7769 7468 2068 6967  ombined with hig
-00000830: 6865 7220 6176 6572 6167 6520 6461 696c  her average dail
-00000840: 7920 7261 7465 7320 6472 6976 696e 6720  y rates driving 
-00000850: 6120 3136 2520 696e 6372 6561 7365 2069  a 16% increase i
-00000860: 6e20 4772 6f73 7320 426f 6f6b 696e 6720  n Gross Booking 
-00000870: 5661 6c75 6520 6f66 2024 3130 2e30 2062  Value of $10.0 b
-00000880: 696c 6c69 6f6e 2e22 0a20 207d 2c0a 2020  illion.".  },.  
-00000890: 7b0a 2020 2020 2271 7565 7374 696f 6e22  {.    "question"
-000008a0: 3a20 2242 7920 7768 6174 2070 6572 6365  : "By what perce
-000008b0: 6e74 6167 6520 6469 6420 4169 7262 6e62  ntage did Airbnb
-000008c0: 2773 206e 6574 2069 6e63 6f6d 6520 696e  's net income in
-000008d0: 6372 6561 7365 2069 6e20 3230 3233 2063  crease in 2023 c
-000008e0: 6f6d 7061 7265 6420 746f 2074 6865 2070  ompared to the p
-000008f0: 7269 6f72 2079 6561 723f 222c 0a20 2020  rior year?",.   
-00000900: 2022 616e 7377 6572 223a 2022 3135 3325   "answer": "153%
-00000910: 222c 0a20 2020 2022 636f 6e74 6578 7422  ",.    "context"
-00000920: 3a20 224e 6574 2069 6e63 6f6d 6520 696e  : "Net income in
-00000930: 2032 3032 3320 696e 6372 6561 7365 6420   2023 increased 
-00000940: 6279 2031 3533 2520 746f 2024 342e 3820  by 153% to $4.8 
-00000950: 6269 6c6c 696f 6e2c 2063 6f6d 7061 7265  billion, compare
-00000960: 6420 746f 2074 6865 2070 7269 6f72 2079  d to the prior y
-00000970: 6561 722c 2064 7269 7665 6e20 6279 206f  ear, driven by o
-00000980: 7572 2072 6576 656e 7565 2067 726f 7774  ur revenue growt
-00000990: 682c 2069 6e63 7265 6173 6564 2069 6e74  h, increased int
-000009a0: 6572 6573 7420 696e 636f 6d65 2c20 6469  erest income, di
-000009b0: 7363 6970 6c69 6e65 2069 6e20 6d61 6e61  scipline in mana
-000009c0: 6769 6e67 206f 7572 2063 6f73 7420 7374  ging our cost st
-000009d0: 7275 6374 7572 652c 2061 6e64 2074 6865  ructure, and the
-000009e0: 2072 656c 6561 7365 206f 6620 6120 706f   release of a po
-000009f0: 7274 696f 6e20 6f66 206f 7572 2076 616c  rtion of our val
-00000a00: 7561 7469 6f6e 2061 6c6c 6f77 616e 6365  uation allowance
-00000a10: 206f 6e20 6465 6665 7272 6564 2074 6178   on deferred tax
-00000a20: 2061 7373 6574 7320 6f66 2024 322e 3920   assets of $2.9 
-00000a30: 6269 6c6c 696f 6e2e 220a 2020 7d0a 5d0a  billion.".  }.].
-00000a40: 6060 600a 0a41 2066 756c 6c20 656e 642d  ```..A full end-
-00000a50: 746f 2d65 6e64 2063 6f64 6520 6578 616d  to-end code exam
-00000a60: 706c 6520 6361 6e20 6265 2066 6f75 6e64  ple can be found
-00000a70: 205b 6865 7265 5d28 6874 7470 733a 2f2f   [here](https://
-00000a80: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
-00000a90: 6f6f 676c 652e 636f 6d2f 6769 7374 2f76  oogle.com/gist/v
-00000aa0: 6972 6174 7474 2f66 3962 3561 3061 6538  irattt/f9b5a0ae8
-00000ab0: 3263 6330 6361 6162 3537 6466 3564 6564  2cc0caab57df5ded
-00000ac0: 6332 3932 3763 392f 696e 7472 6f2d 6669  c2927c9/intro-fi
-00000ad0: 6e61 6e63 6961 6c2d 6461 7461 7365 7473  nancial-datasets
-00000ae0: 2e69 7079 6e62 292e 0a23 2320 496e 7374  .ipynb)..## Inst
-00000af0: 616c 6c61 7469 6f6e 0a0a 2323 2320 5573  allation..### Us
-00000b00: 696e 6720 7069 700a 0a59 6f75 2063 616e  ing pip..You can
-00000b10: 2069 6e73 7461 6c6c 2074 6865 2046 696e   install the Fin
-00000b20: 616e 6369 616c 2044 6174 6173 6574 7320  ancial Datasets 
-00000b30: 6c69 6272 6172 7920 7573 696e 6720 7069  library using pi
-00000b40: 703a 0a0a 6060 600a 7069 7020 696e 7374  p:..```.pip inst
-00000b50: 616c 6c20 6669 6e61 6e63 6961 6c2d 6461  all financial-da
-00000b60: 7461 7365 7473 0a60 6060 0a0a 2323 2320  tasets.```..### 
-00000b70: 5573 696e 6720 506f 6574 7279 0a0a 4966  Using Poetry..If
-00000b80: 2079 6f75 2070 7265 6665 7220 746f 2075   you prefer to u
-00000b90: 7365 2050 6f65 7472 7920 666f 7220 6465  se Poetry for de
-00000ba0: 7065 6e64 656e 6379 206d 616e 6167 656d  pendency managem
-00000bb0: 656e 742c 2079 6f75 2063 616e 2061 6464  ent, you can add
-00000bc0: 2046 696e 616e 6369 616c 2044 6174 6173   Financial Datas
-00000bd0: 6574 7320 746f 2079 6f75 7220 7072 6f6a  ets to your proj
-00000be0: 6563 743a 0a0a 6060 600a 706f 6574 7279  ect:..```.poetry
-00000bf0: 2061 6464 2066 696e 616e 6369 616c 2d64   add financial-d
-00000c00: 6174 6173 6574 730a 6060 600a 0a23 2323  atasets.```..###
-00000c10: 2046 726f 6d20 7468 6520 5265 706f 7369   From the Reposi
-00000c20: 746f 7279 0a0a 4966 2079 6f75 2077 616e  tory..If you wan
-00000c30: 7420 746f 2069 6e73 7461 6c6c 2074 6865  t to install the
-00000c40: 206c 6962 7261 7279 2064 6972 6563 746c   library directl
-00000c50: 7920 6672 6f6d 2074 6865 2072 6570 6f73  y from the repos
-00000c60: 6974 6f72 792c 2066 6f6c 6c6f 7720 7468  itory, follow th
-00000c70: 6573 6520 7374 6570 733a 0a0a 312e 2043  ese steps:..1. C
-00000c80: 6c6f 6e65 2074 6865 2072 6570 6f73 6974  lone the reposit
-00000c90: 6f72 793a 0a20 2020 6060 600a 2020 2067  ory:.   ```.   g
-00000ca0: 6974 2063 6c6f 6e65 2068 7474 7073 3a2f  it clone https:/
-00000cb0: 2f67 6974 6875 622e 636f 6d2f 796f 7572  /github.com/your
-00000cc0: 7573 6572 6e61 6d65 2f66 696e 616e 6369  username/financi
-00000cd0: 616c 2d64 6174 6173 6574 732e 6769 740a  al-datasets.git.
-00000ce0: 2020 2060 6060 0a0a 322e 204e 6176 6967     ```..2. Navig
-00000cf0: 6174 6520 746f 2074 6865 2070 726f 6a65  ate to the proje
-00000d00: 6374 2064 6972 6563 746f 7279 3a0a 2020  ct directory:.  
-00000d10: 2060 6060 0a20 2020 6364 2066 696e 616e   ```.   cd finan
-00000d20: 6369 616c 2d64 6174 6173 6574 730a 2020  cial-datasets.  
-00000d30: 2060 6060 0a20 2020 0a33 2e20 496e 7374   ```.   .3. Inst
-00000d40: 616c 6c20 7468 6520 6465 7065 6e64 656e  all the dependen
-00000d50: 6369 6573 2075 7369 6e67 2050 6f65 7472  cies using Poetr
-00000d60: 793a 0a20 2020 6060 600a 2020 2070 6f65  y:.   ```.   poe
-00000d70: 7472 7920 696e 7374 616c 6c0a 2020 2060  try install.   `
-00000d80: 6060 0a0a 342e 2059 6f75 2063 616e 206e  ``..4. You can n
-00000d90: 6f77 2075 7365 2074 6865 206c 6962 7261  ow use the libra
-00000da0: 7279 2069 6e20 796f 7572 2050 7974 686f  ry in your Pytho
-00000db0: 6e20 7072 6f6a 6563 7473 2e0a 0a23 2320  n projects...## 
-00000dc0: 436f 6e74 7269 6275 7469 6e67 0a0a 436f  Contributing..Co
-00000dd0: 6e74 7269 6275 7469 6f6e 7320 6172 6520  ntributions are 
-00000de0: 7765 6c63 6f6d 6521 2049 6620 796f 7520  welcome! If you 
-00000df0: 6669 6e64 2061 6e79 2069 7373 7565 7320  find any issues 
-00000e00: 6f72 2068 6176 6520 7375 6767 6573 7469  or have suggesti
-00000e10: 6f6e 7320 666f 7220 696d 7072 6f76 656d  ons for improvem
-00000e20: 656e 7473 2c20 0a70 6c65 6173 6520 6f70  ents, .please op
-00000e30: 656e 2061 6e20 6973 7375 6520 6f72 2073  en an issue or s
-00000e40: 7562 6d69 7420 6120 7075 6c6c 2072 6571  ubmit a pull req
-00000e50: 7565 7374 2e0a 0a23 2320 4c69 6365 6e73  uest...## Licens
-00000e60: 650a 0a54 6869 7320 7072 6f6a 6563 7420  e..This project 
-00000e70: 6973 206c 6963 656e 7365 6420 756e 6465  is licensed unde
-00000e80: 7220 7468 6520 5b4d 4954 204c 6963 656e  r the [MIT Licen
-00000e90: 7365 5d28 6c69 6e6b 2d74 6f2d 6c69 6365  se](link-to-lice
-00000ea0: 6e73 652d 6669 6c65 292e 0a0a 2323 2043  nse-file)...## C
-00000eb0: 6f6e 7472 6962 7574 6f72 730a 0a3c 6120  ontributors..<a 
-00000ec0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00000ed0: 7468 7562 2e63 6f6d 2f76 6972 6174 7474  thub.com/virattt
-00000ee0: 2f66 696e 616e 6369 616c 2d64 6174 6173  /financial-datas
-00000ef0: 6574 732f 6772 6170 6873 2f63 6f6e 7472  ets/graphs/contr
-00000f00: 6962 7574 6f72 7322 3e0a 2020 3c69 6d67  ibutors">.  <img
-00000f10: 2073 7263 3d22 6874 7470 733a 2f2f 636f   src="https://co
-00000f20: 6e74 7269 622e 726f 636b 732f 696d 6167  ntrib.rocks/imag
-00000f30: 653f 7265 706f 3d76 6972 6174 7474 2f66  e?repo=virattt/f
-00000f40: 696e 616e 6369 616c 2d64 6174 6173 6574  inancial-dataset
-00000f50: 7322 202f 3e0a 3c2f 613e 0a              s" />.</a>.
+000002c0: 7079 7064 6632 2028 3e3d 332e 302e 312c  pypdf2 (>=3.0.1,
+000002d0: 3c34 2e30 2e30 290a 5265 7175 6972 6573  <4.0.0).Requires
+000002e0: 2d44 6973 743a 2074 696b 746f 6b65 6e20  -Dist: tiktoken 
+000002f0: 283e 3d30 2e36 2e30 2c3c 302e 372e 3029  (>=0.6.0,<0.7.0)
+00000300: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000310: 7471 646d 2028 3e3d 342e 3636 2e32 2c3c  tqdm (>=4.66.2,<
+00000320: 352e 302e 3029 0a52 6571 7569 7265 732d  5.0.0).Requires-
+00000330: 4469 7374 3a20 786d 6c74 6f64 6963 7420  Dist: xmltodict 
+00000340: 283e 3d30 2e31 332e 302c 3c30 2e31 342e  (>=0.13.0,<0.14.
+00000350: 3029 0a44 6573 6372 6970 7469 6f6e 2d43  0).Description-C
+00000360: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
+00000370: 742f 6d61 726b 646f 776e 0a0a 2320 4669  t/markdown..# Fi
+00000380: 6e61 6e63 6961 6c20 4461 7461 7365 7473  nancial Datasets
+00000390: 20f0 9fa7 aa0a 0a46 696e 616e 6369 616c   ......Financial
+000003a0: 2044 6174 6173 6574 7320 6973 2061 6e20   Datasets is an 
+000003b0: 6f70 656e 2d73 6f75 7263 6520 5079 7468  open-source Pyth
+000003c0: 6f6e 206c 6962 7261 7279 200a 7468 6174  on library .that
+000003d0: 206c 6574 7320 796f 7520 6372 6561 7465   lets you create
+000003e0: 2071 7565 7374 696f 6e20 2620 616e 7377   question & answ
+000003f0: 6572 2066 696e 616e 6369 616c 2064 6174  er financial dat
+00000400: 6173 6574 730a 7573 696e 6720 4c61 7267  asets.using Larg
+00000410: 6520 4c61 6e67 7561 6765 204d 6f64 656c  e Language Model
+00000420: 7320 284c 4c4d 7329 2e20 5769 7468 2074  s (LLMs). With t
+00000430: 6869 7320 6c69 6272 6172 792c 0a79 6f75  his library,.you
+00000440: 2063 616e 2065 6173 696c 7920 6765 6e65   can easily gene
+00000450: 7261 7465 2072 6561 6c69 7374 6963 2066  rate realistic f
+00000460: 696e 616e 6369 616c 2064 6174 6173 6574  inancial dataset
+00000470: 7320 6672 6f6d 2061 2031 302d 4b2c 200a  s from a 10-K, .
+00000480: 3130 2d51 2c20 5044 462c 2061 6e64 206f  10-Q, PDF, and o
+00000490: 7468 6572 2066 696e 616e 6369 616c 2074  ther financial t
+000004a0: 6578 7473 2e0a 0a5b 215b 5477 6974 7465  exts...[![Twitte
+000004b0: 7220 466f 6c6c 6f77 5d28 6874 7470 733a  r Follow](https:
+000004c0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000004d0: 2f74 7769 7474 6572 2f66 6f6c 6c6f 772f  /twitter/follow/
+000004e0: 7669 7261 7474 743f 7374 796c 653d 736f  virattt?style=so
+000004f0: 6369 616c 295d 2868 7474 7073 3a2f 2f74  cial)](https://t
+00000500: 7769 7474 6572 2e63 6f6d 2f76 6972 6174  witter.com/virat
+00000510: 7474 290a 0a23 2320 4665 6174 7572 6573  tt)..## Features
+00000520: 0a0a 2d20 4765 6e65 7261 7465 2073 796e  ..- Generate syn
+00000530: 7468 6574 6963 2066 696e 616e 6369 616c  thetic financial
+00000540: 2064 6174 6173 6574 7320 7573 696e 6720   datasets using 
+00000550: 4c4c 4d73 0a2d 2053 7570 706f 7274 7320  LLMs.- Supports 
+00000560: 7661 7269 6f75 7320 5345 4320 6669 6c69  various SEC fili
+00000570: 6e67 7320 2831 302d 4b73 2c20 3130 2d51  ngs (10-Ks, 10-Q
+00000580: 732c 2065 7463 2e29 0a2d 2045 6173 7920  s, etc.).- Easy 
+00000590: 696e 7465 6772 6174 696f 6e20 7769 7468  integration with
+000005a0: 2050 7974 686f 6e20 7072 6f6a 6563 7473   Python projects
+000005b0: 0a2d 2043 7573 746f 6d69 7a61 626c 6520  .- Customizable 
+000005c0: 6461 7461 2067 656e 6572 6174 696f 6e20  data generation 
+000005d0: 6f70 7469 6f6e 730a 0a23 2320 5573 6167  options..## Usag
+000005e0: 650a 0a2a 2a45 7861 6d70 6c65 2067 656e  e..**Example gen
+000005f0: 6572 6174 6564 2064 6174 6173 6574 3a2a  erated dataset:*
+00000600: 2a0a 6060 606a 736f 6e0a 5b0a 2020 7b0a  *.```json.[.  {.
+00000610: 2020 2020 2271 7565 7374 696f 6e22 3a20      "question": 
+00000620: 2257 6861 7420 7761 7320 4169 7262 6e62  "What was Airbnb
+00000630: 2773 2072 6576 656e 7565 2069 6e20 3230  's revenue in 20
+00000640: 3233 3f22 2c0a 2020 2020 2261 6e73 7765  23?",.    "answe
+00000650: 7222 3a20 2224 392e 3920 6269 6c6c 696f  r": "$9.9 billio
+00000660: 6e22 2c0a 2020 2020 2263 6f6e 7465 7874  n",.    "context
+00000670: 223a 2022 496e 2032 3032 332c 2072 6576  ": "In 2023, rev
+00000680: 656e 7565 2069 6e63 7265 6173 6564 2062  enue increased b
+00000690: 7920 3138 2520 746f 2024 392e 3920 6269  y 18% to $9.9 bi
+000006a0: 6c6c 696f 6e20 636f 6d70 6172 6564 2074  llion compared t
+000006b0: 6f20 3230 3232 2c20 7072 696d 6172 696c  o 2022, primaril
+000006c0: 7920 6475 6520 746f 2061 2031 3425 2069  y due to a 14% i
+000006d0: 6e63 7265 6173 6520 696e 204e 6967 6874  ncrease in Night
+000006e0: 7320 616e 6420 4578 7065 7269 656e 6365  s and Experience
+000006f0: 7320 426f 6f6b 6564 206f 6620 3534 2e35  s Booked of 54.5
+00000700: 206d 696c 6c69 6f6e 2063 6f6d 6269 6e65   million combine
+00000710: 6420 7769 7468 2068 6967 6865 7220 6176  d with higher av
+00000720: 6572 6167 6520 6461 696c 7920 7261 7465  erage daily rate
+00000730: 7320 6472 6976 696e 6720 6120 3136 2520  s driving a 16% 
+00000740: 696e 6372 6561 7365 2069 6e20 4772 6f73  increase in Gros
+00000750: 7320 426f 6f6b 696e 6720 5661 6c75 6520  s Booking Value 
+00000760: 6f66 2024 3130 2e30 2062 696c 6c69 6f6e  of $10.0 billion
+00000770: 2e22 0a20 207d 2c0a 2020 7b0a 2020 2020  .".  },.  {.    
+00000780: 2271 7565 7374 696f 6e22 3a20 2242 7920  "question": "By 
+00000790: 7768 6174 2070 6572 6365 6e74 6167 6520  what percentage 
+000007a0: 6469 6420 4169 7262 6e62 2773 206e 6574  did Airbnb's net
+000007b0: 2069 6e63 6f6d 6520 696e 6372 6561 7365   income increase
+000007c0: 2069 6e20 3230 3233 2063 6f6d 7061 7265   in 2023 compare
+000007d0: 6420 746f 2074 6865 2070 7269 6f72 2079  d to the prior y
+000007e0: 6561 723f 222c 0a20 2020 2022 616e 7377  ear?",.    "answ
+000007f0: 6572 223a 2022 3135 3325 222c 0a20 2020  er": "153%",.   
+00000800: 2022 636f 6e74 6578 7422 3a20 224e 6574   "context": "Net
+00000810: 2069 6e63 6f6d 6520 696e 2032 3032 3320   income in 2023 
+00000820: 696e 6372 6561 7365 6420 6279 2031 3533  increased by 153
+00000830: 2520 746f 2024 342e 3820 6269 6c6c 696f  % to $4.8 billio
+00000840: 6e2c 2063 6f6d 7061 7265 6420 746f 2074  n, compared to t
+00000850: 6865 2070 7269 6f72 2079 6561 722c 2064  he prior year, d
+00000860: 7269 7665 6e20 6279 206f 7572 2072 6576  riven by our rev
+00000870: 656e 7565 2067 726f 7774 682c 2069 6e63  enue growth, inc
+00000880: 7265 6173 6564 2069 6e74 6572 6573 7420  reased interest 
+00000890: 696e 636f 6d65 2c20 6469 7363 6970 6c69  income, discipli
+000008a0: 6e65 2069 6e20 6d61 6e61 6769 6e67 206f  ne in managing o
+000008b0: 7572 2063 6f73 7420 7374 7275 6374 7572  ur cost structur
+000008c0: 652c 2061 6e64 2074 6865 2072 656c 6561  e, and the relea
+000008d0: 7365 206f 6620 6120 706f 7274 696f 6e20  se of a portion 
+000008e0: 6f66 206f 7572 2076 616c 7561 7469 6f6e  of our valuation
+000008f0: 2061 6c6c 6f77 616e 6365 206f 6e20 6465   allowance on de
+00000900: 6665 7272 6564 2074 6178 2061 7373 6574  ferred tax asset
+00000910: 7320 6f66 2024 322e 3920 6269 6c6c 696f  s of $2.9 billio
+00000920: 6e2e 220a 2020 7d0a 5d0a 6060 600a 0a2a  n.".  }.].```..*
+00000930: 2a45 7861 6d70 6c65 2023 3120 2d20 6765  *Example #1 - ge
+00000940: 6e65 7261 7465 2066 726f 6d20 616e 7920  nerate from any 
+00000950: 7465 7874 733a 2a2a 0a0a 4d6f 7374 2066  texts:**..Most f
+00000960: 6c65 7869 626c 6520 6f70 7469 6f6e 2e20  lexible option. 
+00000970: 2047 656e 6572 6174 6573 2064 6174 6173   Generates datas
+00000980: 6574 2075 7369 6e67 2061 206c 6973 7420  et using a list 
+00000990: 6f66 2073 7472 696e 6720 6074 6578 7473  of string `texts
+000009a0: 602e 2043 6f6c 6162 2063 6f64 6520 6578  `. Colab code ex
+000009b0: 616d 706c 6520 5b68 6572 655d 2868 7474  ample [here](htt
+000009c0: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
+000009d0: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f67  rch.google.com/g
+000009e0: 6973 742f 7669 7261 7474 742f 6639 6235  ist/virattt/f9b5
+000009f0: 6130 6165 3832 6363 3063 6161 6235 3764  a0ae82cc0caab57d
+00000a00: 6635 6465 6463 3239 3237 6339 2f69 6e74  f5dedc2927c9/int
+00000a10: 726f 2d66 696e 616e 6369 616c 2d64 6174  ro-financial-dat
+00000a20: 6173 6574 732e 6970 796e 6229 2e0a 0a60  asets.ipynb)...`
+00000a30: 6060 7079 7468 6f6e 0a66 726f 6d20 6669  ``python.from fi
+00000a40: 6e61 6e63 6961 6c5f 6461 7461 7365 7473  nancial_datasets
+00000a50: 2e67 656e 6572 6174 6f72 2069 6d70 6f72  .generator impor
+00000a60: 7420 4461 7461 7365 7447 656e 6572 6174  t DatasetGenerat
+00000a70: 6f72 0a0a 7465 7874 7320 3d20 2e2e 2e20  or..texts = ... 
+00000a80: 2023 204c 6973 7420 6f66 2074 6578 7473   # List of texts
+00000a90: 2066 726f 6d20 5345 4320 6669 6c69 6e67   from SEC filing
+00000aa0: 0a67 656e 6572 6174 6f72 203d 2044 6174  .generator = Dat
+00000ab0: 6173 6574 4765 6e65 7261 746f 7228 6d6f  asetGenerator(mo
+00000ac0: 6465 6c3d 2267 7074 2d34 2d30 3132 352d  del="gpt-4-0125-
+00000ad0: 7072 6576 6965 7722 2c20 6170 695f 6b65  preview", api_ke
+00000ae0: 793d 2279 6f75 722d 6f70 656e 6169 2d6b  y="your-openai-k
+00000af0: 6579 2229 0a0a 2320 4765 6e65 7261 7465  ey")..# Generate
+00000b00: 2064 6174 6173 6574 2066 726f 6d20 7465   dataset from te
+00000b10: 7874 730a 6461 7461 7365 7420 3d20 6765  xts.dataset = ge
+00000b20: 6e65 7261 746f 722e 6765 6e65 7261 7465  nerator.generate
+00000b30: 5f66 726f 6d5f 7465 7874 7328 0a20 2020  _from_texts(.   
+00000b40: 7465 7874 733d 7465 7874 732c 200a 2020  texts=texts, .  
+00000b50: 206d 6178 5f71 7565 7374 696f 6e73 3d31   max_questions=1
+00000b60: 3030 2c0a 290a 6060 600a 0a2a 2a45 7861  00,.).```..**Exa
+00000b70: 6d70 6c65 2023 3220 2d20 6765 6e65 7261  mple #2 - genera
+00000b80: 7465 2066 726f 6d20 3130 2d4b 3a2a 2a0a  te from 10-K:**.
+00000b90: 0a47 656e 6572 6174 6520 6120 6461 7461  .Generate a data
+00000ba0: 7365 7420 7573 696e 6720 6120 6074 6963  set using a `tic
+00000bb0: 6b65 7260 2061 6e64 2060 7965 6172 602e  ker` and `year`.
+00000bc0: 2020 436f 6c61 6220 636f 6465 2065 7861    Colab code exa
+00000bd0: 6d70 6c65 205b 6865 7265 5d28 6874 7470  mple [here](http
+00000be0: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
+00000bf0: 6368 2e67 6f6f 676c 652e 636f 6d2f 6769  ch.google.com/gi
+00000c00: 7374 2f76 6972 6174 7474 2f37 3433 3837  st/virattt/74387
+00000c10: 3265 3134 3330 3334 3938 3764 3230 6536  2e143034987d20e6
+00000c20: 6136 6337 6262 3964 3061 312f 696e 7472  a6c7bb9d0a1/intr
+00000c30: 6f2d 6669 6e61 6e63 6961 6c2d 6461 7461  o-financial-data
+00000c40: 7365 7473 2e69 7079 6e62 292e 0a0a 6060  sets.ipynb)...``
+00000c50: 6070 7974 686f 6e0a 6672 6f6d 2066 696e  `python.from fin
+00000c60: 616e 6369 616c 5f64 6174 6173 6574 732e  ancial_datasets.
+00000c70: 6765 6e65 7261 746f 7220 696d 706f 7274  generator import
+00000c80: 2044 6174 6173 6574 4765 6e65 7261 746f   DatasetGenerato
+00000c90: 720a 0a74 6578 7473 203d 202e 2e2e 2020  r..texts = ...  
+00000ca0: 2320 4c69 7374 206f 6620 7465 7874 7320  # List of texts 
+00000cb0: 6672 6f6d 2053 4543 2066 696c 696e 670a  from SEC filing.
+00000cc0: 6765 6e65 7261 746f 7220 3d20 4461 7461  generator = Data
+00000cd0: 7365 7447 656e 6572 6174 6f72 286d 6f64  setGenerator(mod
+00000ce0: 656c 3d22 6770 742d 342d 3031 3235 2d70  el="gpt-4-0125-p
+00000cf0: 7265 7669 6577 222c 2061 7069 5f6b 6579  review", api_key
+00000d00: 3d22 796f 7572 2d6f 7065 6e61 692d 6b65  ="your-openai-ke
+00000d10: 7922 290a 0a23 2047 656e 6572 6174 6520  y")..# Generate 
+00000d20: 6461 7461 7365 7420 6672 6f6d 2031 302d  dataset from 10-
+00000d30: 4b0a 6461 7461 7365 7420 3d20 6765 6e65  K.dataset = gene
+00000d40: 7261 746f 722e 6765 6e65 7261 7465 5f66  rator.generate_f
+00000d50: 726f 6d5f 3130 4b28 0a20 2020 7469 636b  rom_10K(.   tick
+00000d60: 6572 3d22 4141 504c 222c 0a20 2020 7965  er="AAPL",.   ye
+00000d70: 6172 3d32 3032 332c 0a20 2020 6d61 785f  ar=2023,.   max_
+00000d80: 7175 6573 7469 6f6e 733d 3130 302c 0a29  questions=100,.)
+00000d90: 0a60 6060 0a0a 2a2a 4578 616d 706c 6520  .```..**Example 
+00000da0: 2333 202d 2067 656e 6572 6174 6520 6672  #3 - generate fr
+00000db0: 6f6d 2050 4446 3a2a 2a0a 0a47 656e 6572  om PDF:**..Gener
+00000dc0: 6174 6520 6120 6461 7461 7365 7420 7573  ate a dataset us
+00000dd0: 696e 6720 6120 5044 4620 6075 726c 6020  ing a PDF `url` 
+00000de0: 6f6e 6c79 2e20 2043 6f6c 6162 2063 6f64  only.  Colab cod
+00000df0: 6520 6578 616d 706c 6520 5b68 6572 655d  e example [here]
+00000e00: 2868 7474 7073 3a2f 2f63 6f6c 6162 2e72  (https://colab.r
+00000e10: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
+00000e20: 6f6d 2f67 6973 742f 7669 7261 7474 742f  om/gist/virattt/
+00000e30: 6230 3434 3432 6565 3763 3663 3064 3062  b04442ee7c6c0d0b
+00000e40: 6233 6339 3337 3161 6632 3238 3361 3230  b3c9371af2283a20
+00000e50: 2f69 6e74 726f 2d66 696e 616e 6369 616c  /intro-financial
+00000e60: 2d64 6174 6173 6574 732e 6970 796e 6229  -datasets.ipynb)
+00000e70: 2e0a 0a60 6060 7079 7468 6f6e 0a66 726f  ...```python.fro
+00000e80: 6d20 6669 6e61 6e63 6961 6c5f 6461 7461  m financial_data
+00000e90: 7365 7473 2e67 656e 6572 6174 6f72 2069  sets.generator i
+00000ea0: 6d70 6f72 7420 4461 7461 7365 7447 656e  mport DatasetGen
+00000eb0: 6572 6174 6f72 0a0a 7465 7874 7320 3d20  erator..texts = 
+00000ec0: 2e2e 2e20 2023 204c 6973 7420 6f66 2074  ...  # List of t
+00000ed0: 6578 7473 2066 726f 6d20 5345 4320 6669  exts from SEC fi
+00000ee0: 6c69 6e67 0a67 656e 6572 6174 6f72 203d  ling.generator =
+00000ef0: 2044 6174 6173 6574 4765 6e65 7261 746f   DatasetGenerato
+00000f00: 7228 6d6f 6465 6c3d 2267 7074 2d34 2d30  r(model="gpt-4-0
+00000f10: 3132 352d 7072 6576 6965 7722 2c20 6170  125-preview", ap
+00000f20: 695f 6b65 793d 2279 6f75 722d 6f70 656e  i_key="your-open
+00000f30: 6169 2d6b 6579 2229 0a0a 2320 4765 6e65  ai-key")..# Gene
+00000f40: 7261 7465 2064 6174 6173 6574 2066 726f  rate dataset fro
+00000f50: 6d20 5044 4620 7572 6c0a 6461 7461 7365  m PDF url.datase
+00000f60: 7420 3d20 6765 6e65 7261 746f 722e 6765  t = generator.ge
+00000f70: 6e65 7261 7465 5f66 726f 6d5f 7064 6628  nerate_from_pdf(
+00000f80: 0a20 2020 7572 6c3d 2268 7474 7073 3a2f  .   url="https:/
+00000f90: 2f77 7777 2e62 6572 6b73 6869 7265 6861  /www.berkshireha
+00000fa0: 7468 6177 6179 2e63 6f6d 2f6c 6574 7465  thaway.com/lette
+00000fb0: 7273 2f32 3032 336c 7472 2e70 6466 222c  rs/2023ltr.pdf",
+00000fc0: 0a20 2020 6d61 785f 7175 6573 7469 6f6e  .   max_question
+00000fd0: 733d 3130 302c 0a29 0a60 6060 0a0a 2323  s=100,.).```..##
+00000fe0: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a23   Installation..#
+00000ff0: 2323 2055 7369 6e67 2070 6970 0a0a 596f  ## Using pip..Yo
+00001000: 7520 6361 6e20 696e 7374 616c 6c20 7468  u can install th
+00001010: 6520 4669 6e61 6e63 6961 6c20 4461 7461  e Financial Data
+00001020: 7365 7473 206c 6962 7261 7279 2075 7369  sets library usi
+00001030: 6e67 2070 6970 3a0a 0a60 6060 0a70 6970  ng pip:..```.pip
+00001040: 2069 6e73 7461 6c6c 2066 696e 616e 6369   install financi
+00001050: 616c 2d64 6174 6173 6574 730a 6060 600a  al-datasets.```.
+00001060: 0a23 2323 2055 7369 6e67 2050 6f65 7472  .### Using Poetr
+00001070: 790a 0a49 6620 796f 7520 7072 6566 6572  y..If you prefer
+00001080: 2074 6f20 7573 6520 506f 6574 7279 2066   to use Poetry f
+00001090: 6f72 2064 6570 656e 6465 6e63 7920 6d61  or dependency ma
+000010a0: 6e61 6765 6d65 6e74 2c20 796f 7520 6361  nagement, you ca
+000010b0: 6e20 6164 6420 4669 6e61 6e63 6961 6c20  n add Financial 
+000010c0: 4461 7461 7365 7473 2074 6f20 796f 7572  Datasets to your
+000010d0: 2070 726f 6a65 6374 3a0a 0a60 6060 0a70   project:..```.p
+000010e0: 6f65 7472 7920 6164 6420 6669 6e61 6e63  oetry add financ
+000010f0: 6961 6c2d 6461 7461 7365 7473 0a60 6060  ial-datasets.```
+00001100: 0a0a 2323 2320 4672 6f6d 2074 6865 2052  ..### From the R
+00001110: 6570 6f73 6974 6f72 790a 0a49 6620 796f  epository..If yo
+00001120: 7520 7761 6e74 2074 6f20 696e 7374 616c  u want to instal
+00001130: 6c20 7468 6520 6c69 6272 6172 7920 6469  l the library di
+00001140: 7265 6374 6c79 2066 726f 6d20 7468 6520  rectly from the 
+00001150: 7265 706f 7369 746f 7279 2c20 666f 6c6c  repository, foll
+00001160: 6f77 2074 6865 7365 2073 7465 7073 3a0a  ow these steps:.
+00001170: 0a31 2e20 436c 6f6e 6520 7468 6520 7265  .1. Clone the re
+00001180: 706f 7369 746f 7279 3a0a 2020 2060 6060  pository:.   ```
+00001190: 0a20 2020 6769 7420 636c 6f6e 6520 6874  .   git clone ht
+000011a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000011b0: 2f79 6f75 7275 7365 726e 616d 652f 6669  /yourusername/fi
+000011c0: 6e61 6e63 6961 6c2d 6461 7461 7365 7473  nancial-datasets
+000011d0: 2e67 6974 0a20 2020 6060 600a 0a32 2e20  .git.   ```..2. 
+000011e0: 4e61 7669 6761 7465 2074 6f20 7468 6520  Navigate to the 
+000011f0: 7072 6f6a 6563 7420 6469 7265 6374 6f72  project director
+00001200: 793a 0a20 2020 6060 600a 2020 2063 6420  y:.   ```.   cd 
+00001210: 6669 6e61 6e63 6961 6c2d 6461 7461 7365  financial-datase
+00001220: 7473 0a20 2020 6060 600a 2020 200a 332e  ts.   ```.   .3.
+00001230: 2049 6e73 7461 6c6c 2074 6865 2064 6570   Install the dep
+00001240: 656e 6465 6e63 6965 7320 7573 696e 6720  endencies using 
+00001250: 506f 6574 7279 3a0a 2020 2060 6060 0a20  Poetry:.   ```. 
+00001260: 2020 706f 6574 7279 2069 6e73 7461 6c6c    poetry install
+00001270: 0a20 2020 6060 600a 0a34 2e20 596f 7520  .   ```..4. You 
+00001280: 6361 6e20 6e6f 7720 7573 6520 7468 6520  can now use the 
+00001290: 6c69 6272 6172 7920 696e 2079 6f75 7220  library in your 
+000012a0: 5079 7468 6f6e 2070 726f 6a65 6374 732e  Python projects.
+000012b0: 0a0a 2323 2043 6f6e 7472 6962 7574 696e  ..## Contributin
+000012c0: 670a 0a43 6f6e 7472 6962 7574 696f 6e73  g..Contributions
+000012d0: 2061 7265 2077 656c 636f 6d65 2120 4966   are welcome! If
+000012e0: 2079 6f75 2066 696e 6420 616e 7920 6973   you find any is
+000012f0: 7375 6573 206f 7220 6861 7665 2073 7567  sues or have sug
+00001300: 6765 7374 696f 6e73 2066 6f72 2069 6d70  gestions for imp
+00001310: 726f 7665 6d65 6e74 732c 200a 706c 6561  rovements, .plea
+00001320: 7365 206f 7065 6e20 616e 2069 7373 7565  se open an issue
+00001330: 206f 7220 7375 626d 6974 2061 2070 756c   or submit a pul
+00001340: 6c20 7265 7175 6573 742e 0a0a 2323 204c  l request...## L
+00001350: 6963 656e 7365 0a0a 5468 6973 2070 726f  icense..This pro
+00001360: 6a65 6374 2069 7320 6c69 6365 6e73 6564  ject is licensed
+00001370: 2075 6e64 6572 2074 6865 205b 4d49 5420   under the [MIT 
+00001380: 4c69 6365 6e73 655d 286c 696e 6b2d 746f  License](link-to
+00001390: 2d6c 6963 656e 7365 2d66 696c 6529 2e0a  -license-file)..
+000013a0: 0a23 2320 436f 6e74 7269 6275 746f 7273  .## Contributors
+000013b0: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
+000013c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7669  ://github.com/vi
+000013d0: 7261 7474 742f 6669 6e61 6e63 6961 6c2d  rattt/financial-
+000013e0: 6461 7461 7365 7473 2f67 7261 7068 732f  datasets/graphs/
+000013f0: 636f 6e74 7269 6275 746f 7273 223e 0a20  contributors">. 
+00001400: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00001410: 3a2f 2f63 6f6e 7472 6962 2e72 6f63 6b73  ://contrib.rocks
+00001420: 2f69 6d61 6765 3f72 6570 6f3d 7669 7261  /image?repo=vira
+00001430: 7474 742f 6669 6e61 6e63 6961 6c2d 6461  ttt/financial-da
+00001440: 7461 7365 7473 2220 2f3e 0a3c 2f61 3e0a  tasets" />.</a>.
```

