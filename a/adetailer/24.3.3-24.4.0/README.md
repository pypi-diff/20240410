# Comparing `tmp/adetailer-24.3.3.tar.gz` & `tmp/adetailer-24.4.0.tar.gz`

## Comparing `adetailer-24.3.3.tar` & `adetailer-24.4.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 adetailer-24.3.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    14784 2020-02-02 00:00:00.000000 adetailer-24.3.3/CHANGELOG.md
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 adetailer-24.3.3/Taskfile.yml
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 adetailer-24.3.3/install.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 adetailer-24.3.3/preload.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 adetailer-24.3.3/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 adetailer-24.3.3/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 adetailer-24.3.3/.github/ISSUE_TEMPLATE/question.yaml
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 adetailer-24.3.3/.github/workflows/lint.yml
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 adetailer-24.3.3/.github/workflows/stale.yml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 adetailer-24.3.3/.vscode/extensions.json
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 adetailer-24.3.3/.vscode/settings.json
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 adetailer-24.3.3/adetailer/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 adetailer-24.3.3/adetailer/__version__.py
--rw-r--r--   0        0        0     8701 2020-02-02 00:00:00.000000 adetailer-24.3.3/adetailer/args.py
--rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 adetailer-24.3.3/adetailer/common.py
--rw-r--r--   0        0        0     6995 2020-02-02 00:00:00.000000 adetailer-24.3.3/adetailer/mask.py
--rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 adetailer-24.3.3/adetailer/mediapipe.py
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 adetailer-24.3.3/adetailer/traceback.py
--rw-r--r--   0        0        0    23157 2020-02-02 00:00:00.000000 adetailer-24.3.3/adetailer/ui.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 adetailer-24.3.3/adetailer/ultralytics.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 adetailer-24.3.3/controlnet_ext/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 adetailer-24.3.3/controlnet_ext/common.py
--rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 adetailer-24.3.3/controlnet_ext/controlnet_ext.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 adetailer-24.3.3/controlnet_ext/controlnet_ext_forge.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 adetailer-24.3.3/controlnet_ext/restore.py
--rw-r--r--   0        0        0    34407 2020-02-02 00:00:00.000000 adetailer-24.3.3/scripts/!adetailer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adetailer-24.3.3/tests/__init__.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 adetailer-24.3.3/tests/conftest.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 adetailer-24.3.3/tests/test_common.py
--rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 adetailer-24.3.3/tests/test_mask.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 adetailer-24.3.3/tests/test_mediapipe.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 adetailer-24.3.3/tests/test_ultralytics.py
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 adetailer-24.3.3/.gitignore
--rw-r--r--   0        0        0    34521 2020-02-02 00:00:00.000000 adetailer-24.3.3/LICENSE.md
--rw-r--r--   0        0        0     8450 2020-02-02 00:00:00.000000 adetailer-24.3.3/README.md
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 adetailer-24.3.3/pyproject.toml
--rw-r--r--   0        0        0     9044 2020-02-02 00:00:00.000000 adetailer-24.3.3/PKG-INFO
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 adetailer-24.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    15469 2020-02-02 00:00:00.000000 adetailer-24.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 adetailer-24.4.0/Taskfile.yml
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 adetailer-24.4.0/install.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 adetailer-24.4.0/preload.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 adetailer-24.4.0/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 adetailer-24.4.0/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 adetailer-24.4.0/.github/ISSUE_TEMPLATE/question.yaml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 adetailer-24.4.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 adetailer-24.4.0/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 adetailer-24.4.0/.github/workflows/stale.yml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 adetailer-24.4.0/.vscode/extensions.json
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 adetailer-24.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 adetailer-24.4.0/adetailer/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 adetailer-24.4.0/adetailer/__version__.py
+-rw-r--r--   0        0        0     8701 2020-02-02 00:00:00.000000 adetailer-24.4.0/adetailer/args.py
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 adetailer-24.4.0/adetailer/common.py
+-rw-r--r--   0        0        0     6995 2020-02-02 00:00:00.000000 adetailer-24.4.0/adetailer/mask.py
+-rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 adetailer-24.4.0/adetailer/mediapipe.py
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 adetailer-24.4.0/adetailer/traceback.py
+-rw-r--r--   0        0        0    23157 2020-02-02 00:00:00.000000 adetailer-24.4.0/adetailer/ui.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 adetailer-24.4.0/adetailer/ultralytics.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 adetailer-24.4.0/controlnet_ext/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 adetailer-24.4.0/controlnet_ext/common.py
+-rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 adetailer-24.4.0/controlnet_ext/controlnet_ext.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 adetailer-24.4.0/controlnet_ext/controlnet_ext_forge.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 adetailer-24.4.0/controlnet_ext/restore.py
+-rw-r--r--   0        0        0    35424 2020-02-02 00:00:00.000000 adetailer-24.4.0/scripts/!adetailer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adetailer-24.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 adetailer-24.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 adetailer-24.4.0/tests/test_common.py
+-rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 adetailer-24.4.0/tests/test_mask.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 adetailer-24.4.0/tests/test_mediapipe.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 adetailer-24.4.0/tests/test_ultralytics.py
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 adetailer-24.4.0/.gitignore
+-rw-r--r--   0        0        0    34931 2020-02-02 00:00:00.000000 adetailer-24.4.0/LICENSE.md
+-rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 adetailer-24.4.0/README.md
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 adetailer-24.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9009 2020-02-02 00:00:00.000000 adetailer-24.4.0/PKG-INFO
```

### Comparing `adetailer-24.3.3/CHANGELOG.md` & `adetailer-24.4.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,25 @@
 # Changelog
 
+## 2024-04-10
+
+- v24.4.0
+- txt2img에서 hires를 설정했을 때, 이미지의 exif에서 Denoising Strength가 adetailer의 denoisiog stregnth로 덮어 쓰이는 문제 수정
+- ad prompt, ad negative prompt에 프롬프트를 변경하는 기능을 적용했을 때(와일드카드 등), 적용된 프롬프트가 이미지의 exif에 제대로 표시됨
+
+## 2024-03-29
+
+- v24.3.5
+- 알 수 없는 이유로 인페인팅을 확인하는 과정에서 Txt2Img 인스턴스가 들어오는 문제에 대한 임시 해결
+
+## 2024-03-28
+
+- v24.3.4
+- 인페인트에서, 이미지 해상도가 16의 배수가 아닐 때 사이즈 불일치로 인한 opencv 에러 방지
+
 ## 2024-03-25
 
 - v24.3.3
 - webui 1.6.0 미만 버전에서 create_binary_mask 함수에 대해 ImportError가 발생하는 것 수정
 
 ## 2024-03-21
 
@@ -21,14 +37,15 @@
 
 ## 2024-03-01
 
 - v24.3.0
 - YOLO World 모델 추가: 가장 큰 yolov8x-world.pt 모델만 기본적으로 선택할 수 있게 함.
 - lllyasviel/stable-diffusion-webui-forge에서 컨트롤넷을 사용가능하게 함 (PR #517)
 - 기본 스크립트 목록에 soft_inpainting 추가 (https://github.com/AUTOMATIC1111/stable-diffusion-webui/pull/14208)
+
   - 기존에 설치한 사람에게 소급적용되지는 않음
 
 - 감지모델에 대한 간단한 pytest 추가함
 - xyz grid 컨트롤넷 모델 옵션에 `Passthrough` 추가함
 
 ## 2024-01-23
 
@@ -112,45 +129,42 @@
 
 - v23.9.0
 - (실험적) 체크포인트 선택기능
   - 버그가 있어 리프레시 버튼은 구현에서 빠짐
 - 1.6.0 업데이트에 따라 img2img에서 사용불가능한 샘플러를 선택했을 때 더이상 Euler로 변경하지 않음
 - 유효하지 않은 인자가 전달되었을 때, 에러를 일으키지 않고 대신 adetailer를 비활성화함
 
-
 ## 2023-08-25
 
 - v23.8.1
 - xyz grid에서 model을 `None`으로 설정한 이후에 adetailer가 비활성화 되는 문제 수정
 - skip을 눌렀을 때 진행을 멈춤
 - `--medvram-sdxl`을 설정했을 때에도 cpu를 사용하게 함
 
 ## 2023-08-14
 
 - v23.8.0
 - `[PROMPT]` 키워드 추가. `ad_prompt` 또는 `ad_negative_prompt`에 사용하면 입력 프롬프트로 대체됨 (PR #243)
 - Only top k largest 옵션 추가 (PR #264)
 - ultralytics 버전 업데이트
 
-
 ## 2023-07-31
 
 - v23.7.11
 - separate clip skip 옵션 추가
 - install requirements 정리 (ultralytics 새 버전, mediapipe~=3.20)
 
 ## 2023-07-28
 
 - v23.7.10
 - ultralytics, mediapipe import문 정리
 - traceback에서 컬러를 없앰 (api 때문), 라이브러리 버전도 보여주게 설정.
 - huggingface_hub, pydantic을 install.py에서 없앰
 - 안쓰는 컨트롤넷 관련 코드 삭제
 
-
 ## 2023-07-23
 
 - v23.7.9
 - `ultralytics.utils` ModuleNotFoundError 해결 (https://github.com/ultralytics/ultralytics/issues/3856)
 - `pydantic` 2.0 이상 버전 설치안되도록 함
 - `controlnet_dir` cmd args 문제 수정 (PR #107)
 
@@ -250,14 +264,15 @@
 - 스크립트의 이름을 `After Detailer`에서 `ADetailer`로 변경
   - API 사용자는 변경 필요함
 - 몇몇 설정 변경
   - `ad_conf` → `ad_confidence`. 0~100 사이의 int → 0.0~1.0 사이의 float
   - `ad_inpaint_full_res` → `ad_inpaint_only_masked`
   - `ad_inpaint_full_res_padding` → `ad_inpaint_only_masked_padding`
 - mediapipe face mesh 모델 추가
+
   - mediapipe 최소 버전 `0.10.0`
 
 - rich traceback 제거함
 - huggingface 다운로드 실패할 때 에러가 나지 않게 하고 해당 모델을 제거함
 
 ## 2023-05-26
 
@@ -280,15 +295,14 @@
 ### 2023-05-22
 
 - v23.5.17
 - 컨트롤넷 확장이 있으면 컨트롤넷 스크립트를 활성화함. (컨트롤넷 관련 문제 해결)
 - 모든 컴포넌트에 elem_id 설정
 - ui에 버전을 표시함
 
-
 ### 2023-05-19
 
 - v23.5.16
 - 추가한 옵션
   - Mask min/max ratio
   - Mask merge mode
   - Restore faces after ADetailer
```

### Comparing `adetailer-24.3.3/install.py` & `adetailer-24.4.0/install.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.3.3/.github/ISSUE_TEMPLATE/bug_report.yaml` & `adetailer-24.4.0/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,63 @@
-name: Bug report
-description: Create a report
-title: "[Bug]: "
-labels:
-  - bug
-
-body:
-  - type: textarea
-    attributes:
-      label: Describe the bug
-      description: A clear and concise description of what the bug is.
-      placeholder: |
-        Any language accepted
-        아무 언어 사용가능
-        すべての言語に対応
-        接受所有语言
-        Se aceptan todos los idiomas
-        Alle Sprachen werden akzeptiert
-        Toutes les langues sont acceptées
-        Принимаются все языки
-
-  - type: textarea
-    attributes:
-      label: Screenshots
-      description: Screenshots related to the issue.
-
-  - type: textarea
-    attributes:
-      label: Console logs, from start to end.
-      description: |
-        The full console log of your terminal.
-      placeholder: |
-        Python ...
-        Version: ...
-        Commit hash: ...
-        Installing requirements
-        ...
-
-        Launching Web UI with arguments: ...
-        [-] ADetailer initialized. version: ...
-        ...
-        ...
-
-        Traceback (most recent call last):
-        ...
-        ...
-      render: Shell
-    validations:
-      required: true
-
-  - type: textarea
-    attributes:
-      label: List of installed extensions
+name: Bug report
+description: Create a report
+title: "[Bug]: "
+labels:
+  - bug
+
+body:
+  - type: textarea
+    attributes:
+      label: Describe the bug
+      description: A clear and concise description of what the bug is.
+      placeholder: |
+        Any language accepted
+        아무 언어 사용가능
+        すべての言語に対応
+        接受所有语言
+        Se aceptan todos los idiomas
+        Alle Sprachen werden akzeptiert
+        Toutes les langues sont acceptées
+        Принимаются все языки
+    validations:
+      required: true
+
+  - type: textarea
+    attributes:
+      label: Steps to reproduce
+      description: |
+        Description of how we can reproduce this issue.
+    validations:
+      required: true
+
+  - type: textarea
+    attributes:
+      label: Screenshots
+      description: Screenshots related to the issue.
+
+  - type: textarea
+    attributes:
+      label: Console logs, from start to end.
+      description: |
+        The full console log of your terminal.
+      placeholder: |
+        Python ...
+        Version: ...
+        Commit hash: ...
+        Installing requirements
+        ...
+
+        Launching Web UI with arguments: ...
+        [-] ADetailer initialized. version: ...
+        ...
+        ...
+
+        Traceback (most recent call last):
+        ...
+        ...
+      render: Shell
+    validations:
+      required: true
+
+  - type: textarea
+    attributes:
+      label: List of installed extensions
```

### Comparing `adetailer-24.3.3/.github/ISSUE_TEMPLATE/feature_request.yaml` & `adetailer-24.4.0/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-name: Feature request
-description: Suggest an idea for this project
-title: "[Feature Request]: "
-
-body:
-  - type: textarea
-    attributes:
-      label: Is your feature request related to a problem? Please describe.
-      description: A clear and concise description of what the problem is. Ex. I'm always frustrated when [...]
-
-  - type: textarea
-    attributes:
-      label: Describe the solution you'd like
-      description: A clear and concise description of what you want to happen.
-
-  - type: textarea
-    attributes:
-      label: Describe alternatives you've considered
-      description: A clear and concise description of any alternative solutions or features you've considered.
-
-  - type: textarea
-    attributes:
-      label: Additional context
-      description: Add any other context or screenshots about the feature request here.
+name: Feature request
+description: Suggest an idea for this project
+title: "[Feature Request]: "
+labels:
+  - enhancement
+
+body:
+  - type: textarea
+    attributes:
+      label: Is your feature request related to a problem? Please describe.
+      description: A clear and concise description of what the problem is. Ex. I'm always frustrated when [...]
+
+  - type: textarea
+    attributes:
+      label: Describe the solution you'd like
+      description: A clear and concise description of what you want to happen.
+
+  - type: textarea
+    attributes:
+      label: Describe alternatives you've considered
+      description: A clear and concise description of any alternative solutions or features you've considered.
+
+  - type: textarea
+    attributes:
+      label: Additional context
+      description: Add any other context or screenshots about the feature request here.
```

### Comparing `adetailer-24.3.3/.github/workflows/lint.yml` & `adetailer-24.4.0/.github/workflows/lint.yml`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-name: Lint
-
-on:
-  pull_request:
-    paths:
-      - "**.py"
-
-jobs:
-  lint:
-    runs-on: ubuntu-latest
-
-    steps:
-      - uses: actions/checkout@v4
-
-      - name: Setup python
-        uses: actions/setup-python@v5
-        with:
-          python-version: "3.10"
-
-      - name: Install python packages
-        run: pip install black ruff pre-commit-hooks
-
-      - name: Run pre-commit-hooks
-        run: |
-          check-ast
-          trailing-whitespace-fixer --markdown-linebreak-ext=md
-          end-of-file-fixer
-          mixed-line-ending
-
-      - name: Run black
-        run: black --check .
-
-      - name: Run ruff
-        run: ruff check .
+name: Lint
+
+on:
+  pull_request:
+    paths:
+      - "**.py"
+
+jobs:
+  lint:
+    runs-on: ubuntu-latest
+
+    steps:
+      - uses: actions/checkout@v4
+
+      - name: Setup python
+        uses: actions/setup-python@v5
+        with:
+          python-version: "3.10"
+
+      - name: Install python packages
+        run: pip install black ruff pre-commit-hooks
+
+      - name: Run pre-commit-hooks
+        run: |
+          check-ast
+          trailing-whitespace-fixer --markdown-linebreak-ext=md
+          end-of-file-fixer
+          mixed-line-ending
+
+      - name: Run black
+        run: black --check .
+
+      - name: Run ruff
+        run: ruff check .
```

### Comparing `adetailer-24.3.3/adetailer/args.py` & `adetailer-24.4.0/adetailer/args.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.3.3/adetailer/common.py` & `adetailer-24.4.0/adetailer/common.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.3.3/adetailer/mask.py` & `adetailer-24.4.0/adetailer/mask.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.3.3/adetailer/mediapipe.py` & `adetailer-24.4.0/adetailer/mediapipe.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.3.3/adetailer/traceback.py` & `adetailer-24.4.0/adetailer/traceback.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.3.3/adetailer/ui.py` & `adetailer-24.4.0/adetailer/ui.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.3.3/adetailer/ultralytics.py` & `adetailer-24.4.0/adetailer/ultralytics.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.3.3/controlnet_ext/__init__.py` & `adetailer-24.4.0/controlnet_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.3.3/controlnet_ext/controlnet_ext.py` & `adetailer-24.4.0/controlnet_ext/controlnet_ext.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.3.3/controlnet_ext/controlnet_ext_forge.py` & `adetailer-24.4.0/controlnet_ext/controlnet_ext_forge.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.3.3/controlnet_ext/restore.py` & `adetailer-24.4.0/controlnet_ext/restore.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.3.3/scripts/!adetailer.py` & `adetailer-24.4.0/scripts/!adetailer.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from adetailer import (
     AFTER_DETAILER,
     __version__,
     get_models,
     mediapipe_predict,
     ultralytics_predict,
 )
-from adetailer.args import ALL_ARGS, BBOX_SORTBY, ADetailerArgs, SkipImg2ImgOrig
+from adetailer.args import BBOX_SORTBY, ADetailerArgs, SkipImg2ImgOrig
 from adetailer.common import PredictOutput, ensure_pil_image
 from adetailer.mask import (
     filter_by_ratio,
     filter_k_largest,
     has_intersection,
     is_all_black,
     mask_preprocess,
@@ -263,23 +263,20 @@
 
         all_inputs = []
 
         for n, arg_dict in enumerate(args, 1):
             try:
                 inp = ADetailerArgs(**arg_dict)
             except ValueError as e:
-                msgs = [
-                    f"[-] ADetailer: ValidationError when validating {ordinal(n)} arguments: {e}\n"
-                ]
-                for attr in ALL_ARGS.attrs:
-                    arg = arg_dict.get(attr)
-                    dtype = type(arg)
-                    arg = "DEFAULT" if arg is None else repr(arg)
-                    msgs.append(f"    {attr}: {arg} ({dtype})")
-                raise ValueError("\n".join(msgs)) from e
+                msg = f"[-] ADetailer: ValidationError when validating {ordinal(n)} arguments"
+                if hasattr(e, "add_note"):
+                    e.add_note(msg)
+                else:
+                    print(msg, file=sys.stderr)
+                raise
 
             all_inputs.append(inp)
 
         return all_inputs
 
     def extra_params(self, arg_list: list[ADetailerArgs]) -> dict:
         params = {}
@@ -332,21 +329,27 @@
                 prompts[n] = prompts[n].replace(pair.s, pair.r)
         return prompts
 
     def get_prompt(self, p, args: ADetailerArgs) -> tuple[list[str], list[str]]:
         i = self.get_i(p)
         prompt_sr = p._ad_xyz_prompt_sr if hasattr(p, "_ad_xyz_prompt_sr") else []
 
-        prompt = self._get_prompt(args.ad_prompt, p.all_prompts, i, p.prompt, prompt_sr)
+        prompt = self._get_prompt(
+            ad_prompt=args.ad_prompt,
+            all_prompts=p.all_prompts,
+            i=i,
+            default=p.prompt,
+            replacements=prompt_sr,
+        )
         negative_prompt = self._get_prompt(
-            args.ad_negative_prompt,
-            p.all_negative_prompts,
-            i,
-            p.negative_prompt,
-            prompt_sr,
+            ad_prompt=args.ad_negative_prompt,
+            all_prompts=p.all_negative_prompts,
+            i=i,
+            default=p.negative_prompt,
+            replacements=prompt_sr,
         )
 
         return prompt, negative_prompt
 
     def get_seed(self, p) -> tuple[int, int]:
         i = self.get_i(p)
 
@@ -522,15 +525,15 @@
             n_iter=1,
             steps=steps,
             cfg_scale=cfg_scale,
             width=width,
             height=height,
             restore_faces=args.ad_restore_face,
             tiling=p.tiling,
-            extra_generation_params=p.extra_generation_params,
+            extra_generation_params=p.extra_generation_params.copy(),
             do_not_save_samples=True,
             do_not_save_grid=True,
             override_settings=override_settings,
         )
 
         i2i.cached_c = [None, None]
         i2i.cached_uc = [None, None]
@@ -608,24 +611,31 @@
         i2 = min(j, len(negative_prompts) - 1)
         prompt = prompts[i1]
         negative_prompt = negative_prompts[i2]
         i2i.prompt = prompt
         i2i.negative_prompt = negative_prompt
 
     @staticmethod
-    def compare_prompt(p, processed, n: int = 0):
-        if p.prompt != processed.all_prompts[0]:
+    def compare_prompt(p, extra_params: dict[str, Any], processed, n: int = 0):
+        if not hasattr(p, "_ad_extra_params_result"):
+            p._ad_extra_params_result = {}
+
+        pt = "ADetailer prompt" + suffix(n)
+        if pt in extra_params and extra_params[pt] != processed.all_prompts[0]:
             print(
                 f"[-] ADetailer: applied {ordinal(n + 1)} ad_prompt: {processed.all_prompts[0]!r}"
             )
+            p._ad_extra_params_result[pt] = processed.all_prompts[0]
 
-        if p.negative_prompt != processed.all_negative_prompts[0]:
+        ng = "ADetailer negative prompt" + suffix(n)
+        if ng in extra_params and extra_params[ng] != processed.all_negative_prompts[0]:
             print(
                 f"[-] ADetailer: applied {ordinal(n + 1)} ad_negative_prompt: {processed.all_negative_prompts[0]!r}"
             )
+            p._ad_extra_params_result[ng] = processed.all_negative_prompts[0]
 
     @staticmethod
     def need_call_process(p) -> bool:
         if p.scripts is None:
             return False
         i = p.batch_index
         bs = p.batch_size
@@ -656,25 +666,31 @@
     def is_inpaint_only_masked(p) -> bool:
         return hasattr(p, "inpaint_full_res") and p.inpaint_full_res
 
     @staticmethod
     def inpaint_mask_filter(
         img2img_mask: Image.Image, ad_mask: list[Image.Image]
     ) -> list[Image.Image]:
+        if ad_mask and img2img_mask.size != ad_mask[0].size:
+            img2img_mask = img2img_mask.resize(ad_mask[0].size, resample=images.LANCZOS)
         return [mask for mask in ad_mask if has_intersection(img2img_mask, mask)]
 
     @staticmethod
     def get_image_mask(p) -> Image.Image:
         mask = p.image_mask
-        if p.inpainting_mask_invert:
+        if getattr(p, "inpainting_mask_invert", False):
             mask = ImageChops.invert(mask)
         mask = create_binary_mask(mask)
 
         if getattr(p, "_ad_skip_img2img", False):
-            width, height = p.init_images[0].size
+            if hasattr(p, "init_images") and p.init_images:
+                width, height = p.init_images[0].size
+            else:
+                msg = "[-] ADetailer: no init_images."
+                raise RuntimeError(msg)
         else:
             width, height = p.width, p.height
         return images.resize_image(p.resize_mode, mask, width, height)
 
     @rich_traceback
     def process(self, p, *args_):
         if getattr(p, "_ad_disabled", False):
@@ -783,15 +799,15 @@
             except NansException as e:
                 msg = f"[-] ADetailer: 'NansException' occurred with {ordinal(n + 1)} settings.\n{e}"
                 print(msg, file=sys.stderr)
                 continue
             finally:
                 p2.close()
 
-            self.compare_prompt(p2, processed, n=n)
+            self.compare_prompt(p, p.extra_generation_params, processed, n=n)
             p2 = copy(i2i)
             p2.init_images = [processed.images[0]]
 
         if processed is not None:
             pp.image = processed.images[0]
             return True
 
@@ -830,14 +846,17 @@
                 copy_p = copy(p)
                 if hasattr(p.scripts, "before_process"):
                     p.scripts.before_process(copy_p)
                 p.scripts.process(copy_p)
 
         self.write_params_txt(params_txt_content)
 
+        if hasattr(p, "_ad_extra_params_result"):
+            p.extra_generation_params.update(p._ad_extra_params_result)
+
 
 def on_after_component(component, **_kwargs):
     global txt2img_submit_button, img2img_submit_button
     if getattr(component, "elem_id", None) == "txt2img_generate":
         txt2img_submit_button = component
         return
 
@@ -1040,14 +1059,16 @@
 def add_api_endpoints(_: gr.Blocks, app: FastAPI):
     @app.get("/adetailer/v1/version")
     async def version():
         return {"version": __version__}
 
     @app.get("/adetailer/v1/schema")
     async def schema():
+        if hasattr(ADetailerArgs, "model_json_schema"):
+            return ADetailerArgs.model_json_schema()
         return ADetailerArgs.schema()
 
     @app.get("/adetailer/v1/ad_model")
     async def ad_model():
         return {"ad_model": list(model_mapping)}
```

### Comparing `adetailer-24.3.3/tests/test_common.py` & `adetailer-24.4.0/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.3.3/tests/test_mask.py` & `adetailer-24.4.0/tests/test_mask.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 import cv2
 import numpy as np
 import pytest
 from PIL import Image, ImageDraw
 
-from adetailer.mask import dilate_erode, has_intersection, is_all_black, offset
+from adetailer.mask import (
+    bbox_area,
+    dilate_erode,
+    has_intersection,
+    is_all_black,
+    mask_invert,
+    mask_merge,
+    offset,
+)
 
 
 def test_dilate_positive_value():
     img = Image.new("L", (10, 10), color="black")
     draw = ImageDraw.Draw(img)
     draw.rectangle((3, 3, 5, 5), fill="white")
     value = 3
@@ -59,116 +67,170 @@
             [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
         ],
         dtype=np.uint8,
     )
     assert np.array_equal(np.array(result), expect)
 
 
-def test_is_all_black_1():
-    img = Image.new("L", (10, 10), color="black")
-    assert is_all_black(img)
-
-    draw = ImageDraw.Draw(img)
-    draw.rectangle((4, 4, 5, 5), fill="white")
-    assert not is_all_black(img)
-
-
-def test_is_all_black_2():
-    img = np.zeros((10, 10), dtype=np.uint8)
-    assert is_all_black(img)
-
-    img[4:6, 4:6] = 255
-    assert not is_all_black(img)
-
-
-def test_is_all_black_rgb_image_pil():
-    img = Image.new("RGB", (10, 10), color="red")
-    assert not is_all_black(img)
-
-    img = Image.new("RGBA", (10, 10), color="red")
-    assert not is_all_black(img)
-
-
-def test_is_all_black_rgb_image_numpy():
-    img = np.full((10, 10, 4), 127, dtype=np.uint8)
-    with pytest.raises(cv2.error):
-        is_all_black(img)
-
-    img = np.full((4, 10, 10), 0.5, dtype=np.float32)
-    with pytest.raises(cv2.error):
-        is_all_black(img)
+class TestIsAllBlack:
+    def test_is_all_black_1(self):
+        img = Image.new("L", (10, 10), color="black")
+        assert is_all_black(img)
+
+        draw = ImageDraw.Draw(img)
+        draw.rectangle((4, 4, 5, 5), fill="white")
+        assert not is_all_black(img)
+
+    def test_is_all_black_2(self):
+        img = np.zeros((10, 10), dtype=np.uint8)
+        assert is_all_black(img)
+
+        img[4:6, 4:6] = 255
+        assert not is_all_black(img)
+
+    def test_is_all_black_rgb_image_pil(self):
+        img = Image.new("RGB", (10, 10), color="red")
+        assert not is_all_black(img)
+
+        img = Image.new("RGBA", (10, 10), color="red")
+        assert not is_all_black(img)
+
+    def test_is_all_black_rgb_image_numpy(self):
+        img = np.full((10, 10, 4), 127, dtype=np.uint8)
+        with pytest.raises(cv2.error):
+            is_all_black(img)
+
+        img = np.full((4, 10, 10), 0.5, dtype=np.float32)
+        with pytest.raises(cv2.error):
+            is_all_black(img)
+
+
+class TestHasIntersection:
+    def test_has_intersection_1(self):
+        arr1 = np.array(
+            [
+                [0, 0, 0, 0],
+                [0, 0, 0, 0],
+                [0, 0, 0, 0],
+                [0, 0, 0, 0],
+            ],
+            dtype=np.uint8,
+        )
+        arr2 = arr1.copy()
+        assert not has_intersection(arr1, arr2)
+
+    def test_has_intersection_2(self):
+        arr1 = np.array(
+            [
+                [0, 0, 0, 0],
+                [0, 255, 255, 0],
+                [0, 255, 255, 0],
+                [0, 0, 0, 0],
+            ],
+            dtype=np.uint8,
+        )
+        arr2 = np.array(
+            [
+                [0, 0, 0, 0],
+                [0, 0, 0, 0],
+                [0, 0, 255, 255],
+                [0, 0, 255, 255],
+            ],
+            dtype=np.uint8,
+        )
+        assert has_intersection(arr1, arr2)
+
+        arr3 = np.array(
+            [
+                [255, 0, 0, 0],
+                [0, 0, 0, 0],
+                [0, 0, 0, 255],
+                [0, 0, 255, 255],
+            ],
+            dtype=np.uint8,
+        )
+        assert not has_intersection(arr1, arr3)
+
+    def test_has_intersection_3(self):
+        img1 = Image.new("L", (10, 10), color="black")
+        draw1 = ImageDraw.Draw(img1)
+        draw1.rectangle((3, 3, 5, 5), fill="white")
+        img2 = Image.new("L", (10, 10), color="black")
+        draw2 = ImageDraw.Draw(img2)
+        draw2.rectangle((6, 6, 8, 8), fill="white")
+        assert not has_intersection(img1, img2)
+
+        img3 = Image.new("L", (10, 10), color="black")
+        draw3 = ImageDraw.Draw(img3)
+        draw3.rectangle((2, 2, 8, 8), fill="white")
+        assert has_intersection(img1, img3)
+
+    def test_has_intersection_4(self):
+        img1 = Image.new("RGB", (10, 10), color="black")
+        draw1 = ImageDraw.Draw(img1)
+        draw1.rectangle((3, 3, 5, 5), fill="white")
+        img2 = Image.new("RGBA", (10, 10), color="black")
+        draw2 = ImageDraw.Draw(img2)
+        draw2.rectangle((2, 2, 8, 8), fill="white")
+        assert has_intersection(img1, img2)
+
+    def test_has_intersection_5(self):
+        img1 = Image.new("RGB", (10, 10), color="black")
+        draw1 = ImageDraw.Draw(img1)
+        draw1.rectangle((4, 4, 5, 5), fill="white")
+        img2 = np.full((10, 10, 4), 255, dtype=np.uint8)
+        assert has_intersection(img1, img2)
+
+
+def test_bbox_area():
+    bbox = [0.0, 0.0, 10.0, 10.0]
+    assert bbox_area(bbox) == 100
+
+
+class TestMaskMerge:
+    def test_mask_merge(self):
+        img1 = Image.new("L", (10, 10), color="black")
+        draw1 = ImageDraw.Draw(img1)
+        draw1.rectangle((3, 3, 5, 5), fill="white")
+
+        img2 = Image.new("L", (10, 10), color="black")
+        draw2 = ImageDraw.Draw(img2)
+        draw2.rectangle((6, 6, 8, 8), fill="white")
+
+        merged = mask_merge([img1, img2])
+        assert len(merged) == 1
+
+        expect = Image.new("L", (10, 10), color="black")
+        draw3 = ImageDraw.Draw(expect)
+        draw3.rectangle((3, 3, 5, 5), fill="white")
+        draw3.rectangle((6, 6, 8, 8), fill="white")
+
+        assert np.array_equal(np.array(merged[0]), np.array(expect))
+
+    def test_merge_mask_different_size(self):
+        img1 = Image.new("L", (10, 10), color="black")
+        draw1 = ImageDraw.Draw(img1)
+        draw1.rectangle((3, 3, 5, 5), fill="white")
+
+        img2 = Image.new("L", (20, 20), color="black")
+        draw2 = ImageDraw.Draw(img2)
+        draw2.rectangle((6, 6, 8, 8), fill="white")
+
+        with pytest.raises(
+            cv2.error, match="-209:Sizes of input arguments do not match"
+        ):
+            mask_merge([img1, img2])
 
 
-def test_has_intersection_1():
-    arr1 = np.array(
-        [
-            [0, 0, 0, 0],
-            [0, 0, 0, 0],
-            [0, 0, 0, 0],
-            [0, 0, 0, 0],
-        ]
-    )
-    arr2 = arr1.copy()
-    assert not has_intersection(arr1, arr2)
-
-
-def test_has_intersection_2():
-    arr1 = np.array(
-        [
-            [0, 0, 0, 0],
-            [0, 255, 255, 0],
-            [0, 255, 255, 0],
-            [0, 0, 0, 0],
-        ]
-    )
-    arr2 = np.array(
-        [
-            [0, 0, 0, 0],
-            [0, 0, 0, 0],
-            [0, 0, 255, 255],
-            [0, 0, 255, 255],
-        ]
-    )
-    assert has_intersection(arr1, arr2)
+def test_mask_invert():
+    img = Image.new("L", (10, 10), color="black")
+    draw = ImageDraw.Draw(img)
+    draw.rectangle((3, 3, 5, 5), fill="white")
 
-    arr3 = np.array(
-        [
-            [255, 0, 0, 0],
-            [0, 0, 0, 0],
-            [0, 0, 0, 255],
-            [0, 0, 255, 255],
-        ]
-    )
-    assert not has_intersection(arr1, arr3)
+    inverted = mask_invert([img])
+    assert len(inverted) == 1
 
+    expect = Image.new("L", (10, 10), color="white")
+    draw = ImageDraw.Draw(expect)
+    draw.rectangle((3, 3, 5, 5), fill="black")
 
-def test_has_intersection_3():
-    img1 = Image.new("L", (10, 10), color="black")
-    draw1 = ImageDraw.Draw(img1)
-    draw1.rectangle((3, 3, 5, 5), fill="white")
-    img2 = Image.new("L", (10, 10), color="black")
-    draw2 = ImageDraw.Draw(img2)
-    draw2.rectangle((6, 6, 8, 8), fill="white")
-    assert not has_intersection(img1, img2)
-
-    img3 = Image.new("L", (10, 10), color="black")
-    draw3 = ImageDraw.Draw(img3)
-    draw3.rectangle((2, 2, 8, 8), fill="white")
-    assert has_intersection(img1, img3)
-
-
-def test_has_intersection_4():
-    img1 = Image.new("RGB", (10, 10), color="black")
-    draw1 = ImageDraw.Draw(img1)
-    draw1.rectangle((3, 3, 5, 5), fill="white")
-    img2 = Image.new("RGBA", (10, 10), color="black")
-    draw2 = ImageDraw.Draw(img2)
-    draw2.rectangle((2, 2, 8, 8), fill="white")
-    assert has_intersection(img1, img2)
-
-
-def test_has_intersection_5():
-    img1 = Image.new("RGB", (10, 10), color="black")
-    draw1 = ImageDraw.Draw(img1)
-    draw1.rectangle((4, 4, 5, 5), fill="white")
-    img2 = np.full((10, 10, 4), 255, dtype=np.uint8)
-    assert has_intersection(img1, img2)
+    assert np.array_equal(np.array(inverted[0]), np.array(expect))
```

### Comparing `adetailer-24.3.3/tests/test_ultralytics.py` & `adetailer-24.4.0/tests/test_ultralytics.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.3.3/.gitignore` & `adetailer-24.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adetailer-24.3.3/LICENSE.md` & `adetailer-24.4.0/LICENSE.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,662 +1,661 @@
-
-                    GNU AFFERO GENERAL PUBLIC LICENSE
-                       Version 3, 19 November 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU Affero General Public License is a free, copyleft license for
-software and other kinds of works, specifically designed to ensure
-cooperation with the community in the case of network server software.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-our General Public Licenses are intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  Developers that use our General Public Licenses protect your rights
-with two steps: (1) assert copyright on the software, and (2) offer
-you this License which gives you legal permission to copy, distribute
-and/or modify the software.
-
-  A secondary benefit of defending all users' freedom is that
-improvements made in alternate versions of the program, if they
-receive widespread use, become available for other developers to
-incorporate.  Many developers of free software are heartened and
-encouraged by the resulting cooperation.  However, in the case of
-software used on network servers, this result may fail to come about.
-The GNU General Public License permits making a modified version and
-letting the public access it on a server without ever releasing its
-source code to the public.
-
-  The GNU Affero General Public License is designed specifically to
-ensure that, in such cases, the modified source code becomes available
-to the community.  It requires the operator of a network server to
-provide the source code of the modified version running there to the
-users of that server.  Therefore, public use of a modified version, on
-a publicly accessible server, gives the public access to the source
-code of the modified version.
-
-  An older license, called the Affero General Public License and
-published by Affero, was designed to accomplish similar goals.  This is
-a different license, not a version of the Affero GPL, but Affero has
-released a new version of the Affero GPL which permits relicensing under
-this license.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU Affero General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Remote Network Interaction; Use with the GNU General Public License.
-
-  Notwithstanding any other provision of this License, if you modify the
-Program, your modified version must prominently offer all users
-interacting with it remotely through a computer network (if your version
-supports such interaction) an opportunity to receive the Corresponding
-Source of your version by providing access to the Corresponding Source
-from a network server at no charge, through some standard or customary
-means of facilitating copying of software.  This Corresponding Source
-shall include the Corresponding Source for any work covered by version 3
-of the GNU General Public License that is incorporated pursuant to the
-following paragraph.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the work with which it is combined will remain governed by version
-3 of the GNU General Public License.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU Affero General Public License from time to time.  Such new versions
-will be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU Affero General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU Affero General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU Affero General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU Affero General Public License as published
-    by the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU Affero General Public License for more details.
-
-    You should have received a copy of the GNU Affero General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If your software can interact with users remotely through a computer
-network, you should also make sure that it provides a way for users to
-get its source.  For example, if your program is a web application, its
-interface could display a "Source" link that leads users to an archive
-of the code.  There are many ways you could offer source, and different
-solutions will be better for different programs; see section 13 for the
-specific requirements.
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU AGPL, see
-<http://www.gnu.org/licenses/>.
+                    GNU AFFERO GENERAL PUBLIC LICENSE
+                       Version 3, 19 November 2007
+
+Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+Everyone is permitted to copy and distribute verbatim copies
+of this license document, but changing it is not allowed.
+
+                            Preamble
+
+The GNU Affero General Public License is a free, copyleft license for
+software and other kinds of works, specifically designed to ensure
+cooperation with the community in the case of network server software.
+
+The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works. By contrast,
+our General Public Licenses are intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.
+
+When we speak of free software, we are referring to freedom, not
+price. Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+Developers that use our General Public Licenses protect your rights
+with two steps: (1) assert copyright on the software, and (2) offer
+you this License which gives you legal permission to copy, distribute
+and/or modify the software.
+
+A secondary benefit of defending all users' freedom is that
+improvements made in alternate versions of the program, if they
+receive widespread use, become available for other developers to
+incorporate. Many developers of free software are heartened and
+encouraged by the resulting cooperation. However, in the case of
+software used on network servers, this result may fail to come about.
+The GNU General Public License permits making a modified version and
+letting the public access it on a server without ever releasing its
+source code to the public.
+
+The GNU Affero General Public License is designed specifically to
+ensure that, in such cases, the modified source code becomes available
+to the community. It requires the operator of a network server to
+provide the source code of the modified version running there to the
+users of that server. Therefore, public use of a modified version, on
+a publicly accessible server, gives the public access to the source
+code of the modified version.
+
+An older license, called the Affero General Public License and
+published by Affero, was designed to accomplish similar goals. This is
+a different license, not a version of the Affero GPL, but Affero has
+released a new version of the Affero GPL which permits relicensing under
+this license.
+
+The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+0. Definitions.
+
+"This License" refers to version 3 of the GNU Affero General Public License.
+
+"Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+"The Program" refers to any copyrightable work licensed under this
+License. Each licensee is addressed as "you". "Licensees" and
+"recipients" may be individuals or organizations.
+
+To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy. The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy. Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies. Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License. If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+1. Source Code.
+
+The "source code" for a work means the preferred form of the work
+for making modifications to it. "Object code" means any non-source
+form of a work.
+
+A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form. A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities. However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work. For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+The Corresponding Source for a work in source code form is that
+same work.
+
+2. Basic Permissions.
+
+All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met. This License explicitly affirms your unlimited
+permission to run the unmodified Program. The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work. This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force. You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright. Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+Conveying under any other circumstances is permitted solely under
+the conditions stated below. Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+4. Conveying Verbatim Copies.
+
+You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+5. Conveying Modified Source Versions.
+
+You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit. Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+6. Conveying Non-Source Forms.
+
+You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling. In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage. For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product. A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+"Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source. The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information. But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed. Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+7. Additional Terms.
+
+"Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law. If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it. (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.) You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10. If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term. If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+8. Termination.
+
+You may not propagate or modify a covered work except as expressly
+provided under this License. Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License. If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+9. Acceptance Not Required for Having Copies.
+
+You are not required to accept this License in order to receive or
+run a copy of the Program. Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance. However,
+nothing other than this License grants you permission to propagate or
+modify any covered work. These actions infringe copyright if you do
+not accept this License. Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+10. Automatic Licensing of Downstream Recipients.
+
+Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License. You are not responsible
+for enforcing compliance by third parties with this License.
+
+An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations. If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License. For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+11. Patents.
+
+A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based. The
+work thus licensed is called the contributor's "contributor version".
+
+A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version. For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement). To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients. "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License. You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+12. No Surrender of Others' Freedom.
+
+If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License. If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all. For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+13. Remote Network Interaction; Use with the GNU General Public License.
+
+Notwithstanding any other provision of this License, if you modify the
+Program, your modified version must prominently offer all users
+interacting with it remotely through a computer network (if your version
+supports such interaction) an opportunity to receive the Corresponding
+Source of your version by providing access to the Corresponding Source
+from a network server at no charge, through some standard or customary
+means of facilitating copying of software. This Corresponding Source
+shall include the Corresponding Source for any work covered by version 3
+of the GNU General Public License that is incorporated pursuant to the
+following paragraph.
+
+Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU General Public License into a single
+combined work, and to convey the resulting work. The terms of this
+License will continue to apply to the part which is the covered work,
+but the work with which it is combined will remain governed by version
+3 of the GNU General Public License.
+
+14. Revised Versions of this License.
+
+The Free Software Foundation may publish revised and/or new versions of
+the GNU Affero General Public License from time to time. Such new versions
+will be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+Each version is given a distinguishing version number. If the
+Program specifies that a certain numbered version of the GNU Affero General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation. If the Program does not specify a version number of the
+GNU Affero General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+If the Program specifies that a proxy can decide which future
+versions of the GNU Affero General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+Later license versions may give you additional or different
+permissions. However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+15. Disclaimer of Warranty.
+
+THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+16. Limitation of Liability.
+
+IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+17. Interpretation of Sections 15 and 16.
+
+If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+To do so, attach the following notices to the program. It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Affero General Public License as published
+    by the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Affero General Public License for more details.
+
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+If your software can interact with users remotely through a computer
+network, you should also make sure that it provides a way for users to
+get its source. For example, if your program is a web application, its
+interface could display a "Source" link that leads users to an archive
+of the code. There are many ways you could offer source, and different
+solutions will be better for different programs; see section 13 for the
+specific requirements.
+
+You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU AGPL, see
+<http://www.gnu.org/licenses/>.
```

### Comparing `adetailer-24.3.3/README.md` & `adetailer-24.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,112 +1,129 @@
-# ADetailer
-
-ADetailer is a extension for stable diffusion webui, similar to Detection Detailer, except it uses ultralytics instead of the mmdet.
-
-## Install
-
-(from Mikubill/sd-webui-controlnet)
-
-1. Open "Extensions" tab.
-2. Open "Install from URL" tab in the tab.
-3. Enter `https://github.com/Bing-su/adetailer.git` to "URL for extension's git repository".
-4. Press "Install" button.
-5. Wait 5 seconds, and you will see the message "Installed into stable-diffusion-webui\extensions\adetailer. Use Installed tab to restart".
-6. Go to "Installed" tab, click "Check for updates", and then click "Apply and restart UI". (The next time you can also use this method to update extensions.)
-7. Completely restart A1111 webui including your terminal. (If you do not know what is a "terminal", you can reboot your computer: turn your computer off and turn it on again.)
-
-You can now install it directly from the Extensions tab.
-
-![image](https://i.imgur.com/g6GdRBT.png)
-
-You **DON'T** need to download any base model from huggingface.
-
-## Options
-
-| Model, Prompts                    |                                                                                    |                                                                                                                                                        |
-| --------------------------------- | ---------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
-| ADetailer model                   | Determine what to detect.                                                          | `None` = disable                                                                                                                                       |
-| ADetailer model classes           | Comma separated class names to detect. only available when using YOLO World models | If blank, use default values.<br/>default = [COCO 80 classes](https://github.com/ultralytics/ultralytics/blob/main/ultralytics/cfg/datasets/coco.yaml) |
-| ADetailer prompt, negative prompt | Prompts and negative prompts to apply                                              | If left blank, it will use the same as the input.                                                                                                      |
-| Skip img2img                      | Skip img2img. In practice, this works by changing the step count of img2img to 1.  | img2img only                                                                                                                                           |
-
-| Detection                            |                                                                                              |              |
-| ------------------------------------ | -------------------------------------------------------------------------------------------- | ------------ |
-| Detection model confidence threshold | Only objects with a detection model confidence above this threshold are used for inpainting. |              |
-| Mask min/max ratio                   | Only use masks whose area is between those ratios for the area of the entire image.          |              |
-| Mask only the top k largest          | Only use the k objects with the largest area of the bbox.                                    | 0 to disable |
-
-If you want to exclude objects in the background, try setting the min ratio to around `0.01`.
-
-| Mask Preprocessing              |                                                                                                                                     |                                                                                         |
-| ------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
-| Mask x, y offset                | Moves the mask horizontally and vertically by                                                                                       |                                                                                         |
-| Mask erosion (-) / dilation (+) | Enlarge or reduce the detected mask.                                                                                                | [opencv example](https://docs.opencv.org/4.7.0/db/df6/tutorial_erosion_dilatation.html) |
-| Mask merge mode                 | `None`: Inpaint each mask<br/>`Merge`: Merge all masks and inpaint<br/>`Merge and Invert`: Merge all masks and Invert, then inpaint |                                                                                         |
-
-Applied in this order: x, y offset → erosion/dilation → merge/invert.
-
-#### Inpainting
-
-Each option corresponds to a corresponding option on the inpaint tab. Therefore, please refer to the inpaint tab for usage details on how to use each option.
-
-## ControlNet Inpainting
-
-You can use the ControlNet extension if you have ControlNet installed and ControlNet models.
-
-Support `inpaint, scribble, lineart, openpose, tile, depth` controlnet models. Once you choose a model, the preprocessor is set automatically. It works separately from the model set by the Controlnet extension.
-
-If you select `Passthrough`, the controlnet settings you set outside of ADetailer will be used.
-
-## Advanced Options
-
-API request example: [wiki/API](https://github.com/Bing-su/adetailer/wiki/API)
-
-`ui-config.json` entries: [wiki/ui-config.json](https://github.com/Bing-su/adetailer/wiki/ui-config.json)
-
-`[SEP], [SKIP]` tokens: [wiki/Advanced](https://github.com/Bing-su/adetailer/wiki/Advanced)
-
-## Media
-
-- 🎥 [どこよりも詳しいAfter Detailer (adetailer)の使い方① 【Stable Diffusion】](https://youtu.be/sF3POwPUWCE)
-- 🎥 [どこよりも詳しいAfter Detailer (adetailer)の使い方② 【Stable Diffusion】](https://youtu.be/urNISRdbIEg)
-
-## Model
-
-| Model                 | Target                | mAP 50                        | mAP 50-95                     |
-| --------------------- | --------------------- | ----------------------------- | ----------------------------- |
-| face_yolov8n.pt       | 2D / realistic face   | 0.660                         | 0.366                         |
-| face_yolov8s.pt       | 2D / realistic face   | 0.713                         | 0.404                         |
-| hand_yolov8n.pt       | 2D / realistic hand   | 0.767                         | 0.505                         |
-| person_yolov8n-seg.pt | 2D / realistic person | 0.782 (bbox)<br/>0.761 (mask) | 0.555 (bbox)<br/>0.460 (mask) |
-| person_yolov8s-seg.pt | 2D / realistic person | 0.824 (bbox)<br/>0.809 (mask) | 0.605 (bbox)<br/>0.508 (mask) |
-| mediapipe_face_full   | realistic face        | -                             | -                             |
-| mediapipe_face_short  | realistic face        | -                             | -                             |
-| mediapipe_face_mesh   | realistic face        | -                             | -                             |
-
-The YOLO models can be found on huggingface [Bingsu/adetailer](https://huggingface.co/Bingsu/adetailer).
-
-For a detailed description of the YOLO8 model, see: https://docs.ultralytics.com/models/yolov8/#overview
-
-YOLO World model: https://docs.ultralytics.com/models/yolo-world/
-
-### Additional Model
-
-Put your [ultralytics](https://github.com/ultralytics/ultralytics) yolo model in `webui/models/adetailer`. The model name should end with `.pt`.
-
-It must be a bbox detection or segment model and use all label.
-
-## How it works
-
-ADetailer works in three simple steps.
-
-1. Create an image.
-2. Detect object with a detection model and create a mask image.
-3. Inpaint using the image from 1 and the mask from 2.
-
-## Development
-
-ADetailer is developed and tested using the stable-diffusion 1.5 model, for the [AUTOMATIC1111/stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) repository only.
-
-## License
-
-ADetailer is a derivative work that uses two AGPL-licensed works (stable-diffusion-webui, ultralytics) and is therefore distributed under the AGPL license.
+Metadata-Version: 2.3
+Name: adetailer
+Version: 24.4.0
+Summary: An object detection and auto-mask extension for stable diffusion webui.
+Project-URL: repository, https://github.com/Bing-su/adetailer
+Author-email: dowon <ks2515@naver.com>
+License: AGPL-3.0
+License-File: LICENSE.md
+Keywords: adetailer,stable-diffusion,stable-diffusion-webui,ultralytics
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Topic :: Scientific/Engineering :: Image Recognition
+Requires-Python: <3.13,>=3.8
+Requires-Dist: huggingface-hub
+Requires-Dist: mediapipe>=0.10
+Requires-Dist: pydantic<3
+Requires-Dist: rich>=13
+Requires-Dist: ultralytics>=8.1
+Description-Content-Type: text/markdown
+
+# ADetailer
+
+ADetailer is an extension for the stable diffusion webui that does automatic masking and inpainting. It is similar to the Detection Detailer.
+
+## Install
+
+(from Mikubill/sd-webui-controlnet)
+
+1. Open "Extensions" tab.
+2. Open "Install from URL" tab in the tab.
+3. Enter `https://github.com/Bing-su/adetailer.git` to "URL for extension's git repository".
+4. Press "Install" button.
+5. Wait 5 seconds, and you will see the message "Installed into stable-diffusion-webui\extensions\adetailer. Use Installed tab to restart".
+6. Go to "Installed" tab, click "Check for updates", and then click "Apply and restart UI". (The next time you can also use this method to update extensions.)
+7. Completely restart A1111 webui including your terminal. (If you do not know what is a "terminal", you can reboot your computer: turn your computer off and turn it on again.)
+
+You can now install it directly from the Extensions tab.
+
+![image](https://i.imgur.com/g6GdRBT.png)
+
+## Options
+
+| Model, Prompts                    |                                                                                    |                                                                                                                                                        |
+| --------------------------------- | ---------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
+| ADetailer model                   | Determine what to detect.                                                          | `None` = disable                                                                                                                                       |
+| ADetailer model classes           | Comma separated class names to detect. only available when using YOLO World models | If blank, use default values.<br/>default = [COCO 80 classes](https://github.com/ultralytics/ultralytics/blob/main/ultralytics/cfg/datasets/coco.yaml) |
+| ADetailer prompt, negative prompt | Prompts and negative prompts to apply                                              | If left blank, it will use the same as the input.                                                                                                      |
+| Skip img2img                      | Skip img2img. In practice, this works by changing the step count of img2img to 1.  | img2img only                                                                                                                                           |
+
+| Detection                            |                                                                                              |              |
+| ------------------------------------ | -------------------------------------------------------------------------------------------- | ------------ |
+| Detection model confidence threshold | Only objects with a detection model confidence above this threshold are used for inpainting. |              |
+| Mask min/max ratio                   | Only use masks whose area is between those ratios for the area of the entire image.          |              |
+| Mask only the top k largest          | Only use the k objects with the largest area of the bbox.                                    | 0 to disable |
+
+If you want to exclude objects in the background, try setting the min ratio to around `0.01`.
+
+| Mask Preprocessing              |                                                                                                                                     |                                                                                         |
+| ------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
+| Mask x, y offset                | Moves the mask horizontally and vertically by                                                                                       |                                                                                         |
+| Mask erosion (-) / dilation (+) | Enlarge or reduce the detected mask.                                                                                                | [opencv example](https://docs.opencv.org/4.7.0/db/df6/tutorial_erosion_dilatation.html) |
+| Mask merge mode                 | `None`: Inpaint each mask<br/>`Merge`: Merge all masks and inpaint<br/>`Merge and Invert`: Merge all masks and Invert, then inpaint |                                                                                         |
+
+Applied in this order: x, y offset → erosion/dilation → merge/invert.
+
+#### Inpainting
+
+Each option corresponds to a corresponding option on the inpaint tab. Therefore, please refer to the inpaint tab for usage details on how to use each option.
+
+## ControlNet Inpainting
+
+You can use the ControlNet extension if you have ControlNet installed and ControlNet models.
+
+Support `inpaint, scribble, lineart, openpose, tile, depth` controlnet models. Once you choose a model, the preprocessor is set automatically. It works separately from the model set by the Controlnet extension.
+
+If you select `Passthrough`, the controlnet settings you set outside of ADetailer will be used.
+
+## Advanced Options
+
+API request example: [wiki/REST-API](https://github.com/Bing-su/adetailer/wiki/REST-API)
+
+`[SEP], [SKIP], [PROMPT]` tokens: [wiki/Advanced](https://github.com/Bing-su/adetailer/wiki/Advanced)
+
+## Media
+
+- 🎥 [どこよりも詳しいAfter Detailer (adetailer)の使い方① 【Stable Diffusion】](https://youtu.be/sF3POwPUWCE)
+- 🎥 [どこよりも詳しいAfter Detailer (adetailer)の使い方② 【Stable Diffusion】](https://youtu.be/urNISRdbIEg)
+
+- 📜 [ADetailer Installation and 5 Usage Methods](https://kindanai.com/en/manual-adetailer/)
+
+## Model
+
+| Model                 | Target                | mAP 50                        | mAP 50-95                     |
+| --------------------- | --------------------- | ----------------------------- | ----------------------------- |
+| face_yolov8n.pt       | 2D / realistic face   | 0.660                         | 0.366                         |
+| face_yolov8s.pt       | 2D / realistic face   | 0.713                         | 0.404                         |
+| hand_yolov8n.pt       | 2D / realistic hand   | 0.767                         | 0.505                         |
+| person_yolov8n-seg.pt | 2D / realistic person | 0.782 (bbox)<br/>0.761 (mask) | 0.555 (bbox)<br/>0.460 (mask) |
+| person_yolov8s-seg.pt | 2D / realistic person | 0.824 (bbox)<br/>0.809 (mask) | 0.605 (bbox)<br/>0.508 (mask) |
+| mediapipe_face_full   | realistic face        | -                             | -                             |
+| mediapipe_face_short  | realistic face        | -                             | -                             |
+| mediapipe_face_mesh   | realistic face        | -                             | -                             |
+
+The YOLO models can be found on huggingface [Bingsu/adetailer](https://huggingface.co/Bingsu/adetailer).
+
+For a detailed description of the YOLO8 model, see: https://docs.ultralytics.com/models/yolov8/#overview
+
+YOLO World model: https://docs.ultralytics.com/models/yolo-world/
+
+### Additional Model
+
+Put your [ultralytics](https://github.com/ultralytics/ultralytics) yolo model in `models/adetailer`. The model name should end with `.pt`.
+
+It must be a bbox detection or segment model and use all label.
+
+## How it works
+
+ADetailer works in three simple steps.
+
+1. Create an image.
+2. Detect object with a detection model and create a mask image.
+3. Inpaint using the image from 1 and the mask from 2.
+
+## Development
+
+ADetailer is developed and tested using the stable-diffusion 1.5 model, for the latest version of [AUTOMATIC1111/stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) repository only.
+
+## License
+
+ADetailer is a derivative work that uses two AGPL-licensed works (stable-diffusion-webui, ultralytics) and is therefore distributed under the AGPL license.
```

### Comparing `adetailer-24.3.3/pyproject.toml` & `adetailer-24.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -50,24 +50,28 @@
     "E",
     "EM",
     "F",
     "FA",
     "I001",
     "ISC",
     "N",
+    "PD",
     "PERF",
     "PIE",
     "PT",
     "PTH",
     "RET",
     "RUF",
     "SIM",
+    "T20",
+    "TRY",
     "UP",
     "W",
 ]
-ignore = ["B008", "B905", "E501", "F401"]
+ignore = ["B905", "E501"]
+unfixable = ["F401"]
 
 [tool.ruff.lint.isort]
 known-first-party = ["launch", "modules"]
 
 [tool.ruff.lint.pyupgrade]
 keep-runtime-typing = true
```

### Comparing `adetailer-24.3.3/PKG-INFO` & `adetailer-24.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,10 @@
-Metadata-Version: 2.1
-Name: adetailer
-Version: 24.3.3
-Summary: An object detection and auto-mask extension for stable diffusion webui.
-Project-URL: repository, https://github.com/Bing-su/adetailer
-Author-email: dowon <ks2515@naver.com>
-License: AGPL-3.0
-License-File: LICENSE.md
-Keywords: adetailer,stable-diffusion,stable-diffusion-webui,ultralytics
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Requires-Python: <3.13,>=3.8
-Requires-Dist: huggingface-hub
-Requires-Dist: mediapipe>=0.10
-Requires-Dist: pydantic<3
-Requires-Dist: rich>=13
-Requires-Dist: ultralytics>=8.1
-Description-Content-Type: text/markdown
-
 # ADetailer
 
-ADetailer is a extension for stable diffusion webui, similar to Detection Detailer, except it uses ultralytics instead of the mmdet.
+ADetailer is an extension for the stable diffusion webui that does automatic masking and inpainting. It is similar to the Detection Detailer.
 
 ## Install
 
 (from Mikubill/sd-webui-controlnet)
 
 1. Open "Extensions" tab.
 2. Open "Install from URL" tab in the tab.
@@ -33,16 +14,14 @@
 6. Go to "Installed" tab, click "Check for updates", and then click "Apply and restart UI". (The next time you can also use this method to update extensions.)
 7. Completely restart A1111 webui including your terminal. (If you do not know what is a "terminal", you can reboot your computer: turn your computer off and turn it on again.)
 
 You can now install it directly from the Extensions tab.
 
 ![image](https://i.imgur.com/g6GdRBT.png)
 
-You **DON'T** need to download any base model from huggingface.
-
 ## Options
 
 | Model, Prompts                    |                                                                                    |                                                                                                                                                        |
 | --------------------------------- | ---------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
 | ADetailer model                   | Determine what to detect.                                                          | `None` = disable                                                                                                                                       |
 | ADetailer model classes           | Comma separated class names to detect. only available when using YOLO World models | If blank, use default values.<br/>default = [COCO 80 classes](https://github.com/ultralytics/ultralytics/blob/main/ultralytics/cfg/datasets/coco.yaml) |
 | ADetailer prompt, negative prompt | Prompts and negative prompts to apply                                              | If left blank, it will use the same as the input.                                                                                                      |
@@ -74,25 +53,25 @@
 
 Support `inpaint, scribble, lineart, openpose, tile, depth` controlnet models. Once you choose a model, the preprocessor is set automatically. It works separately from the model set by the Controlnet extension.
 
 If you select `Passthrough`, the controlnet settings you set outside of ADetailer will be used.
 
 ## Advanced Options
 
-API request example: [wiki/API](https://github.com/Bing-su/adetailer/wiki/API)
+API request example: [wiki/REST-API](https://github.com/Bing-su/adetailer/wiki/REST-API)
 
-`ui-config.json` entries: [wiki/ui-config.json](https://github.com/Bing-su/adetailer/wiki/ui-config.json)
-
-`[SEP], [SKIP]` tokens: [wiki/Advanced](https://github.com/Bing-su/adetailer/wiki/Advanced)
+`[SEP], [SKIP], [PROMPT]` tokens: [wiki/Advanced](https://github.com/Bing-su/adetailer/wiki/Advanced)
 
 ## Media
 
 - 🎥 [どこよりも詳しいAfter Detailer (adetailer)の使い方① 【Stable Diffusion】](https://youtu.be/sF3POwPUWCE)
 - 🎥 [どこよりも詳しいAfter Detailer (adetailer)の使い方② 【Stable Diffusion】](https://youtu.be/urNISRdbIEg)
 
+- 📜 [ADetailer Installation and 5 Usage Methods](https://kindanai.com/en/manual-adetailer/)
+
 ## Model
 
 | Model                 | Target                | mAP 50                        | mAP 50-95                     |
 | --------------------- | --------------------- | ----------------------------- | ----------------------------- |
 | face_yolov8n.pt       | 2D / realistic face   | 0.660                         | 0.366                         |
 | face_yolov8s.pt       | 2D / realistic face   | 0.713                         | 0.404                         |
 | hand_yolov8n.pt       | 2D / realistic hand   | 0.767                         | 0.505                         |
@@ -106,26 +85,26 @@
 
 For a detailed description of the YOLO8 model, see: https://docs.ultralytics.com/models/yolov8/#overview
 
 YOLO World model: https://docs.ultralytics.com/models/yolo-world/
 
 ### Additional Model
 
-Put your [ultralytics](https://github.com/ultralytics/ultralytics) yolo model in `webui/models/adetailer`. The model name should end with `.pt`.
+Put your [ultralytics](https://github.com/ultralytics/ultralytics) yolo model in `models/adetailer`. The model name should end with `.pt`.
 
 It must be a bbox detection or segment model and use all label.
 
 ## How it works
 
 ADetailer works in three simple steps.
 
 1. Create an image.
 2. Detect object with a detection model and create a mask image.
 3. Inpaint using the image from 1 and the mask from 2.
 
 ## Development
 
-ADetailer is developed and tested using the stable-diffusion 1.5 model, for the [AUTOMATIC1111/stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) repository only.
+ADetailer is developed and tested using the stable-diffusion 1.5 model, for the latest version of [AUTOMATIC1111/stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) repository only.
 
 ## License
 
 ADetailer is a derivative work that uses two AGPL-licensed works (stable-diffusion-webui, ultralytics) and is therefore distributed under the AGPL license.
```

