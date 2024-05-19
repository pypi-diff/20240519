# Comparing `tmp/adetailer-24.4.1.tar.gz` & `tmp/adetailer-24.4.2.tar.gz`

## Comparing `adetailer-24.4.1.tar` & `adetailer-24.4.2.tar`

### file list

```diff
@@ -1,44 +1,43 @@
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 adetailer-24.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    15889 2020-02-02 00:00:00.000000 adetailer-24.4.1/CHANGELOG.md
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 adetailer-24.4.1/Taskfile.yml
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 adetailer-24.4.1/install.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 adetailer-24.4.1/preload.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 adetailer-24.4.1/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 adetailer-24.4.1/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 adetailer-24.4.1/.github/ISSUE_TEMPLATE/question.yaml
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 adetailer-24.4.1/.github/workflows/notlint.yml
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 adetailer-24.4.1/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 adetailer-24.4.1/.github/workflows/stale.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 adetailer-24.4.1/.vscode/extensions.json
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 adetailer-24.4.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adetailer-24.4.1/aaaaaa/__init__.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 adetailer-24.4.1/aaaaaa/conditional.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 adetailer-24.4.1/aaaaaa/helper.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 adetailer-24.4.1/aaaaaa/p_method.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 adetailer-24.4.1/adetailer/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 adetailer-24.4.1/adetailer/__version__.py
--rw-r--r--   0        0        0     9190 2020-02-02 00:00:00.000000 adetailer-24.4.1/adetailer/args.py
--rw-r--r--   0        0        0     4346 2020-02-02 00:00:00.000000 adetailer-24.4.1/adetailer/common.py
--rw-r--r--   0        0        0     6995 2020-02-02 00:00:00.000000 adetailer-24.4.1/adetailer/mask.py
--rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 adetailer-24.4.1/adetailer/mediapipe.py
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 adetailer-24.4.1/adetailer/traceback.py
--rw-r--r--   0        0        0    23810 2020-02-02 00:00:00.000000 adetailer-24.4.1/adetailer/ui.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 adetailer-24.4.1/adetailer/ultralytics.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 adetailer-24.4.1/controlnet_ext/__init__.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 adetailer-24.4.1/controlnet_ext/common.py
--rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 adetailer-24.4.1/controlnet_ext/controlnet_ext.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 adetailer-24.4.1/controlnet_ext/controlnet_ext_forge.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 adetailer-24.4.1/controlnet_ext/restore.py
--rw-r--r--   0        0        0    34616 2020-02-02 00:00:00.000000 adetailer-24.4.1/scripts/!adetailer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adetailer-24.4.1/tests/__init__.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 adetailer-24.4.1/tests/conftest.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 adetailer-24.4.1/tests/test_args.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 adetailer-24.4.1/tests/test_common.py
--rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 adetailer-24.4.1/tests/test_mask.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 adetailer-24.4.1/tests/test_mediapipe.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 adetailer-24.4.1/tests/test_ultralytics.py
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 adetailer-24.4.1/.gitignore
--rw-r--r--   0        0        0    34270 2020-02-02 00:00:00.000000 adetailer-24.4.1/LICENSE.md
--rw-r--r--   0        0        0     8597 2020-02-02 00:00:00.000000 adetailer-24.4.1/README.md
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 adetailer-24.4.1/pyproject.toml
--rw-r--r--   0        0        0     9185 2020-02-02 00:00:00.000000 adetailer-24.4.1/PKG-INFO
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 adetailer-24.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    15620 2020-02-02 00:00:00.000000 adetailer-24.4.2/CHANGELOG.md
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 adetailer-24.4.2/Taskfile.yml
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 adetailer-24.4.2/install.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 adetailer-24.4.2/preload.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 adetailer-24.4.2/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 adetailer-24.4.2/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 adetailer-24.4.2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 adetailer-24.4.2/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 adetailer-24.4.2/.github/workflows/stale.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 adetailer-24.4.2/.vscode/extensions.json
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 adetailer-24.4.2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adetailer-24.4.2/aaaaaa/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 adetailer-24.4.2/aaaaaa/conditional.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 adetailer-24.4.2/aaaaaa/helper.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 adetailer-24.4.2/aaaaaa/p_method.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 adetailer-24.4.2/adetailer/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 adetailer-24.4.2/adetailer/__version__.py
+-rw-r--r--   0        0        0     8923 2020-02-02 00:00:00.000000 adetailer-24.4.2/adetailer/args.py
+-rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 adetailer-24.4.2/adetailer/common.py
+-rw-r--r--   0        0        0     6731 2020-02-02 00:00:00.000000 adetailer-24.4.2/adetailer/mask.py
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 adetailer-24.4.2/adetailer/mediapipe.py
+-rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 adetailer-24.4.2/adetailer/traceback.py
+-rw-r--r--   0        0        0    23117 2020-02-02 00:00:00.000000 adetailer-24.4.2/adetailer/ui.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 adetailer-24.4.2/adetailer/ultralytics.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 adetailer-24.4.2/controlnet_ext/__init__.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 adetailer-24.4.2/controlnet_ext/common.py
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 adetailer-24.4.2/controlnet_ext/controlnet_ext.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 adetailer-24.4.2/controlnet_ext/controlnet_ext_forge.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 adetailer-24.4.2/controlnet_ext/restore.py
+-rw-r--r--   0        0        0    33750 2020-02-02 00:00:00.000000 adetailer-24.4.2/scripts/!adetailer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adetailer-24.4.2/tests/__init__.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 adetailer-24.4.2/tests/conftest.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 adetailer-24.4.2/tests/test_args.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 adetailer-24.4.2/tests/test_common.py
+-rw-r--r--   0        0        0     7035 2020-02-02 00:00:00.000000 adetailer-24.4.2/tests/test_mask.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 adetailer-24.4.2/tests/test_mediapipe.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 adetailer-24.4.2/tests/test_ultralytics.py
+-rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 adetailer-24.4.2/.gitignore
+-rw-r--r--   0        0        0    34270 2020-02-02 00:00:00.000000 adetailer-24.4.2/LICENSE.md
+-rw-r--r--   0        0        0     8479 2020-02-02 00:00:00.000000 adetailer-24.4.2/README.md
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 adetailer-24.4.2/pyproject.toml
+-rw-r--r--   0        0        0     9185 2020-02-02 00:00:00.000000 adetailer-24.4.2/PKG-INFO
```

### Comparing `adetailer-24.4.1/.pre-commit-config.yaml` & `adetailer-24.4.2/.pre-commit-config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-ci:
-  autoupdate_branch: "dev"
-
-repos:
-  - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.6.0
-    hooks:
-      - id: check-added-large-files
-        args: [--maxkb=100]
-      - id: check-merge-conflict
-      - id: check-case-conflict
-      - id: check-ast
-      - id: trailing-whitespace
-        args: [--markdown-linebreak-ext=md]
-      - id: end-of-file-fixer
-      - id: mixed-line-ending
-
-  - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v4.0.0-alpha.8"
-    hooks:
-      - id: prettier
-
-  - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.7
-    hooks:
-      - id: ruff
-        args: [--fix, --exit-non-zero-on-fix]
-      - id: ruff-format
+ci:
+  autoupdate_branch: "dev"
+
+repos:
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.6.0
+    hooks:
+      - id: check-added-large-files
+        args: [--maxkb=100]
+      - id: check-merge-conflict
+      - id: check-case-conflict
+      - id: check-ast
+      - id: check-yaml
+      - id: trailing-whitespace
+        args: [--markdown-linebreak-ext=md]
+      - id: end-of-file-fixer
+      - id: mixed-line-ending
+
+  - repo: https://github.com/pre-commit/mirrors-prettier
+    rev: "v4.0.0-alpha.8"
+    hooks:
+      - id: prettier
+
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.3.7
+    hooks:
+      - id: ruff
+        args: [--fix, --exit-non-zero-on-fix]
+      - id: ruff-format
```

### Comparing `adetailer-24.4.1/CHANGELOG.md` & `adetailer-24.4.2/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,431 +1,437 @@
-# Changelog
-
-## 2024-04-14
-
-- v24.4.1
-- webui 1.9.0에서 발생한 에러 수정
-  - extra generation params에 callable이 들어와서 생긴 문제
-  - assign_current_image에 None이 들어갈 수 있던 문제
-- webui 1.9.0에서 변경된 scheduler 지원
-- 컨트롤넷 모델을 찾을 때, 대소문자 구분을 하지 않음 (PR #577)
-- 몇몇 기능을 스크립트에서 분리하여 별도 파일로 빼냄
-
-## 2024-04-10
-
-- v24.4.0
-- txt2img에서 hires를 설정했을 때, 이미지의 exif에서 Denoising Strength가 adetailer의 denoisiog stregnth로 덮어 쓰이는 문제 수정
-- ad prompt, ad negative prompt에 프롬프트를 변경하는 기능을 적용했을 때(와일드카드 등), 적용된 프롬프트가 이미지의 exif에 제대로 표시됨
-
-## 2024-03-29
-
-- v24.3.5
-- 알 수 없는 이유로 인페인팅을 확인하는 과정에서 Txt2Img 인스턴스가 들어오는 문제에 대한 임시 해결
-
-## 2024-03-28
-
-- v24.3.4
-- 인페인트에서, 이미지 해상도가 16의 배수가 아닐 때 사이즈 불일치로 인한 opencv 에러 방지
-
-## 2024-03-25
-
-- v24.3.3
-- webui 1.6.0 미만 버전에서 create_binary_mask 함수에 대해 ImportError가 발생하는 것 수정
-
-## 2024-03-21
-
-- v24.3.2
-- UI를 거치지 않은 입력에 대해, image_mask를 입력했을 때 opencv 에러가 발생하는 것 수정
-- img2img inpaint에서 skip img2img 옵션을 활성화할 경우, adetailer를 비활성화함
-  - 마스크 크기에 대해 해결하기 힘든 문제가 있음
-
-## 2024-03-16
-
-- v24.3.1
-- YOLO World v2, YOLO9 지원가능한 버전으로 ultralytics 업데이트
-- inpaint full res인 경우 인페인트 모드에서 동작하게 변경
-- inpaint full res가 아닌 경우, 사용자가 입력한 마스크와 교차점이 있는 마스크만 선택하여 사용함
-
-## 2024-03-01
-
-- v24.3.0
-- YOLO World 모델 추가: 가장 큰 yolov8x-world.pt 모델만 기본적으로 선택할 수 있게 함.
-- lllyasviel/stable-diffusion-webui-forge에서 컨트롤넷을 사용가능하게 함 (PR #517)
-- 기본 스크립트 목록에 soft_inpainting 추가 (https://github.com/AUTOMATIC1111/stable-diffusion-webui/pull/14208)
-
-  - 기존에 설치한 사람에게 소급적용되지는 않음
-
-- 감지모델에 대한 간단한 pytest 추가함
-- xyz grid 컨트롤넷 모델 옵션에 `Passthrough` 추가함
-
-## 2024-01-23
-
-- v24.1.2
-- controlnet 모델에 `Passthrough` 옵션 추가. 입력으로 들어온 컨트롤넷 옵션을 그대로 사용
-- fastapi 엔드포인트 추가
-
-## 2024-01-10
-
-- v24.1.1
-- SDNext 호환 업데이트 (issue #466)
-  - 설정 값 state에 초기값 추가
-  - 위젯 값을 변경할 때마다 state도 변경되게 함 (기존에는 생성 버튼을 누를 때 적용되었음)
-- `inpaint_depth_hand` 컨트롤넷 모델이 depth 모델로 인식되게 함 (issue #463)
-
-## 2024-01-04
-
-- v24.1.0
-- `depth_hand_refiner` ControlNet 추가 (PR #460)
-
-## 2023-12-30
-
-- v23.12.0
-- 파일을 인자로 추가하는 몇몇 스크립트에 대해 deepcopy의 에러를 피하기 위해 script_args 복사 방법을 변경함
-- skip img2img 기능을 사용할 때 너비, 높이를 128로 고정하여 스킵 과정이 조금 더 나아짐
-- img2img inpainting 모드에서 adetailer 자동 비활성화
-- 처음 생성된 params.txt 파일을 항상 유지하도록 변경함
-
-## 2023-11-19
-
-- v23.11.1
-- 기본 스크립트 목록에 negpip 추가
-  - 기존에 설치한 사람에게 소급적용되지는 않음
-- skip img2img 옵션이 2스텝 이상일 때, 제대로 적용되지 않는 문제 수정
-- SD.Next에서 이미지가 np.ndarray로 입력되는 경우 수정
-- 컨트롤넷 경로를 sys.path에 추가하여 --data-dir등을 지정한 경우에도 임포트 에러가 일어나지 않게 함.
-
-## 2023-10-30
-
-- v23.11.0
-- 이미지의 인덱스 계산방법 변경
-  - webui 1.1.0 미만에서 adetailer 실행 불가능하게 함
-- 컨트롤넷 preprocessor 선택지 늘림
-- 추가 yolo 모델 디렉터리를 설정할 수 있는 옵션 추가
-- infotext에 `/`가 있는 항목이 exif에서 복원되지 않는 문제 수정
-  - 이전 버전에 생성된 이미지는 여전히 복원안됨
-- 같은 탭에서 항상 같은 시드를 적용하게 하는 옵션 추가
-- 컨트롤넷 1.1.411 (f2aafcf2beb99a03cbdf7db73852228ccd6bd1d6) 버전을 사용중일 경우,
-  webui 버전 1.6.0 미만에서 사용할 수 없다는 메세지 출력
-
-## 2023-10-15
-
-- v23.10.1
-- xyz grid에 prompt S/R 추가
-- img2img에서 steps가 1일때 에러가 발생하는 샘플러의 처리를 위해 샘플러 이름도 변경하게 수정
-
-## 2023-10-07
-
-- v23.10.0
-- 허깅페이스 모델을 다운로드 실패했을 때, 계속 다운로드를 시도하지 않음
-- img2img에서 img2img단계를 건너뛰는 기능 추가
-- live preview에서 감지 단계를 보여줌 (PR #352)
-
-## 2023-09-20
-
-- v23.9.3
-- ultralytics 버전 8.0.181로 업데이트 (https://github.com/ultralytics/ultralytics/pull/4891)
-- mediapipe와 ultralytics의 lazy import
-
-## 2023-09-10
-
-- v23.9.2
-- (실험적) VAE 선택 기능
-
-## 2023-09-01
-
-- v23.9.1
-- webui 1.6.0에 추가된 인자를 사용해서 생긴 하위 호환 문제 수정
-
-## 2023-08-31
-
-- v23.9.0
-- (실험적) 체크포인트 선택기능
-  - 버그가 있어 리프레시 버튼은 구현에서 빠짐
-- 1.6.0 업데이트에 따라 img2img에서 사용불가능한 샘플러를 선택했을 때 더이상 Euler로 변경하지 않음
-- 유효하지 않은 인자가 전달되었을 때, 에러를 일으키지 않고 대신 adetailer를 비활성화함
-
-## 2023-08-25
-
-- v23.8.1
-- xyz grid에서 model을 `None`으로 설정한 이후에 adetailer가 비활성화 되는 문제 수정
-- skip을 눌렀을 때 진행을 멈춤
-- `--medvram-sdxl`을 설정했을 때에도 cpu를 사용하게 함
-
-## 2023-08-14
-
-- v23.8.0
-- `[PROMPT]` 키워드 추가. `ad_prompt` 또는 `ad_negative_prompt`에 사용하면 입력 프롬프트로 대체됨 (PR #243)
-- Only top k largest 옵션 추가 (PR #264)
-- ultralytics 버전 업데이트
-
-## 2023-07-31
-
-- v23.7.11
-- separate clip skip 옵션 추가
-- install requirements 정리 (ultralytics 새 버전, mediapipe~=3.20)
-
-## 2023-07-28
-
-- v23.7.10
-- ultralytics, mediapipe import문 정리
-- traceback에서 컬러를 없앰 (api 때문), 라이브러리 버전도 보여주게 설정.
-- huggingface_hub, pydantic을 install.py에서 없앰
-- 안쓰는 컨트롤넷 관련 코드 삭제
-
-## 2023-07-23
-
-- v23.7.9
-- `ultralytics.utils` ModuleNotFoundError 해결 (https://github.com/ultralytics/ultralytics/issues/3856)
-- `pydantic` 2.0 이상 버전 설치안되도록 함
-- `controlnet_dir` cmd args 문제 수정 (PR #107)
-
-## 2023-07-20
-
-- v23.7.8
-- `paste_field_names` 추가했던 것을 되돌림
-
-## 2023-07-19
-
-- v23.7.7
-- 인페인팅 단계에서 별도의 샘플러를 선택할 수 있게 옵션을 추가함 (xyz그리드에도 추가)
-- webui 1.0.0-pre 이하 버전에서 batch index 문제 수정
-- 스크립트에 `paste_field_names`을 추가함. 사용되는지는 모르겠음
-
-## 2023-07-16
-
-- v23.7.6
-- `ultralytics 8.0.135`에 추가된 cpuinfo 기능을 위해 `py-cpuinfo`를 미리 설치하게 함. (미리 설치 안하면 cpu나 mps사용할 때 재시작해야함)
-- init_image가 RGB 모드가 아닐 때 RGB로 변경.
-
-## 2023-07-07
-
-- v23.7.4
-- batch count > 1일때 프롬프트의 인덱스 문제 수정
-
-- v23.7.5
-- i2i의 `cached_uc`와 `cached_c`가 p의 `cached_uc`와 `cached_c`가 다른 인스턴스가 되도록 수정
-
-## 2023-07-05
-
-- v23.7.3
-- 버그 수정
-  - `object()`가 json 직렬화 안되는 문제
-  - `process`를 호출함에 따라 배치 카운트가 2이상일 때, all_prompts가 고정되는 문제
-  - `ad-before`와 `ad-preview` 이미지 파일명이 실제 파일명과 다른 문제
-  - pydantic 2.0 호환성 문제
-
-## 2023-07-04
-
-- v23.7.2
-- `mediapipe_face_mesh_eyes_only` 모델 추가: `mediapipe_face_mesh`로 감지한 뒤 눈만 사용함.
-- 매 배치 시작 전에 `scripts.postprocess`를, 후에 `scripts.process`를 호출함.
-  - 컨트롤넷을 사용하면 소요 시간이 조금 늘어나지만 몇몇 문제 해결에 도움이 됨.
-- `lora_block_weight`를 스크립트 화이트리스트에 추가함.
-  - 한번이라도 ADetailer를 사용한 사람은 수동으로 추가해야함.
-
-## 2023-07-03
-
-- v23.7.1
-- `process_images`를 진행한 뒤 `StableDiffusionProcessing` 오브젝트의 close를 호출함
-- api 호출로 사용했는지 확인하는 속성 추가
-- `NansException`이 발생했을 때 중지하지 않고 남은 과정 계속 진행함
-
-## 2023-07-02
-
-- v23.7.0
-- `NansException`이 발생하면 로그에 표시하고 원본 이미지를 반환하게 설정
-- `rich`를 사용한 에러 트레이싱
-  - install.py에 `rich` 추가
-- 생성 중에 컴포넌트의 값을 변경하면 args의 값도 함께 변경되는 문제 수정 (issue #180)
-- 터미널 로그로 ad_prompt와 ad_negative_prompt에 적용된 실제 프롬프트 확인할 수 있음 (입력과 다를 경우에만)
-
-## 2023-06-28
-
-- v23.6.4
-- 최대 모델 수 5 -> 10개
-- ad_prompt와 ad_negative_prompt에 빈칸으로 놔두면 입력 프롬프트가 사용된다는 문구 추가
-- huggingface 모델 다운로드 실패시 로깅
-- 1st 모델이 `None`일 경우 나머지 입력을 무시하던 문제 수정
-- `--use-cpu` 에 `adetailer` 입력 시 cpu로 yolo모델을 사용함
-
-## 2023-06-20
-
-- v23.6.3
-- 컨트롤넷 inpaint 모델에 대해, 3가지 모듈을 사용할 수 있도록 함
-- Noise Multiplier 옵션 추가 (PR #149)
-- pydantic 최소 버전 1.10.8로 설정 (Issue #146)
-
-## 2023-06-05
-
-- v23.6.2
-- xyz_grid에서 ADetailer를 사용할 수 있게함.
-  - 8가지 옵션만 1st 탭에 적용되도록 함.
-
-## 2023-06-01
-
-- v23.6.1
-- `inpaint, scribble, lineart, openpose, tile` 5가지 컨트롤넷 모델 지원 (PR #107)
-- controlnet guidance start, end 인자 추가 (PR #107)
-- `modules.extensions`를 사용하여 컨트롤넷 확장을 불러오고 경로를 알아내로록 변경
-- ui에서 컨트롤넷을 별도 함수로 분리
-
-## 2023-05-30
-
-- v23.6.0
-- 스크립트의 이름을 `After Detailer`에서 `ADetailer`로 변경
-  - API 사용자는 변경 필요함
-- 몇몇 설정 변경
-  - `ad_conf` → `ad_confidence`. 0~100 사이의 int → 0.0~1.0 사이의 float
-  - `ad_inpaint_full_res` → `ad_inpaint_only_masked`
-  - `ad_inpaint_full_res_padding` → `ad_inpaint_only_masked_padding`
-- mediapipe face mesh 모델 추가
-
-  - mediapipe 최소 버전 `0.10.0`
-
-- rich traceback 제거함
-- huggingface 다운로드 실패할 때 에러가 나지 않게 하고 해당 모델을 제거함
-
-## 2023-05-26
-
-- v23.5.19
-- 1번째 탭에도 `None` 옵션을 추가함
-- api로 ad controlnet model에 inpaint가 아닌 다른 컨트롤넷 모델을 사용하지 못하도록 막음
-- adetailer 진행중에 total tqdm 진행바 업데이트를 멈춤
-- state.inturrupted 상태에서 adetailer 과정을 중지함
-- 컨트롤넷 process를 각 batch가 끝난 순간에만 호출하도록 변경
-
-### 2023-05-25
-
-- v23.5.18
-- 컨트롤넷 관련 수정
-  - unit의 `input_mode`를 `SIMPLE`로 모두 변경
-  - 컨트롤넷 유넷 훅과 하이잭 함수들을 adetailer를 실행할 때에만 되돌리는 기능 추가
-  - adetailer 처리가 끝난 뒤 컨트롤넷 스크립트의 process를 다시 진행함. (batch count 2 이상일때의 문제 해결)
-- 기본 활성 스크립트 목록에서 컨트롤넷을 뺌
-
-### 2023-05-22
-
-- v23.5.17
-- 컨트롤넷 확장이 있으면 컨트롤넷 스크립트를 활성화함. (컨트롤넷 관련 문제 해결)
-- 모든 컴포넌트에 elem_id 설정
-- ui에 버전을 표시함
-
-### 2023-05-19
-
-- v23.5.16
-- 추가한 옵션
-  - Mask min/max ratio
-  - Mask merge mode
-  - Restore faces after ADetailer
-- 옵션들을 Accordion으로 묶음
-
-### 2023-05-18
-
-- v23.5.15
-- 필요한 것만 임포트하도록 변경 (vae 로딩 오류 없어짐. 로딩 속도 빨라짐)
-
-### 2023-05-17
-
-- v23.5.14
-- `[SKIP]`으로 ad prompt 일부를 건너뛰는 기능 추가
-- bbox 정렬 옵션 추가
-- sd_webui 타입힌트를 만들어냄
-- enable checker와 관련된 api 오류 수정?
-
-### 2023-05-15
-
-- v23.5.13
-- `[SEP]`으로 ad prompt를 분리하여 적용하는 기능 추가
-- enable checker를 다시 pydantic으로 변경함
-- ui 관련 함수를 adetailer.ui 폴더로 분리함
-- controlnet을 사용할 때 모든 controlnet unit 비활성화
-- adetailer 폴더가 없으면 만들게 함
-
-### 2023-05-13
-
-- v23.5.12
-- `ad_enable`을 제외한 입력이 dict타입으로 들어오도록 변경
-  - web api로 사용할 때에 특히 사용하기 쉬움
-  - web api breaking change
-- `mask_preprocess` 인자를 넣지 않았던 오류 수정 (PR #47)
-- huggingface에서 모델을 다운로드하지 않는 옵션 추가 `--ad-no-huggingface`
-
-### 2023-05-12
-
-- v23.5.11
-- `ultralytics` 알람 제거
-- 필요없는 exif 인자 더 제거함
-- `use separate steps` 옵션 추가
-- ui 배치를 조정함
-
-### 2023-05-09
-
-- v23.5.10
-- 선택한 스크립트만 ADetailer에 적용하는 옵션 추가, 기본값 `True`. 설정 탭에서 지정가능.
-  - 기본값: `dynamic_prompting,dynamic_thresholding,wildcards,wildcard_recursive`
-- `person_yolov8s-seg.pt` 모델 추가
-- `ultralytics`의 최소 버전을 `8.0.97`로 설정 (C:\\ 문제 해결된 버전)
-
-### 2023-05-08
-
-- v23.5.9
-- 2가지 이상의 모델을 사용할 수 있음. 기본값: 2, 최대: 5
-- segment 모델을 사용할 수 있게 함. `person_yolov8n-seg.pt` 추가
-
-### 2023-05-07
-
-- v23.5.8
-- 프롬프트와 네거티브 프롬프트에 방향키 지원 (PR #24)
-- `mask_preprocess`를 추가함. 이전 버전과 시드값이 달라질 가능성 있음!
-- 이미지 처리가 일어났을 때에만 before이미지를 저장함
-- 설정창의 레이블을 ADetailer 대신 더 적절하게 수정함
-
-### 2023-05-06
-
-- v23.5.7
-- `ad_use_cfg_scale` 옵션 추가. cfg 스케일을 따로 사용할지 말지 결정함.
-- `ad_enable` 기본값을 `True`에서 `False`로 변경
-- `ad_model`의 기본값을 `None`에서 첫번째 모델로 변경
-- 최소 2개의 입력(ad_enable, ad_model)만 들어오면 작동하게 변경.
-
-- v23.5.7.post0
-- `init_controlnet_ext`을 controlnet_exists == True일때에만 실행
-- webui를 C드라이브 바로 밑에 설치한 사람들에게 `ultralytics` 경고 표시
-
-### 2023-05-05 (어린이날)
-
-- v23.5.5
-- `Save images before ADetailer` 옵션 추가
-- 입력으로 들어온 인자와 ALL_ARGS의 길이가 다르면 에러메세지
-- README.md에 설치방법 추가
-
-- v23.5.6
-- get_args에서 IndexError가 발생하면 자세한 에러메세지를 볼 수 있음
-- AdetailerArgs에 extra_params 내장
-- scripts_args를 딥카피함
-- postprocess_image를 약간 분리함
-
-- v23.5.6.post0
-- `init_controlnet_ext`에서 에러메세지를 자세히 볼 수 있음
-
-### 2023-05-04
-
-- v23.5.4
-- use pydantic for arguments validation
-- revert: ad_model to `None` as default
-- revert: `__future__` imports
-- lazily import yolo and mediapipe
-
-### 2023-05-03
-
-- v23.5.3.post0
-- remove `__future__` imports
-- change to copy scripts and scripts args
-
-- v23.5.3.post1
-- change default ad_model from `None`
-
-### 2023-05-02
-
-- v23.5.3
-- Remove `None` from model list and add `Enable ADetailer` checkbox.
-- install.py `skip_install` fix.
+# Changelog
+
+## 2024-04-17
+
+- v24.4.2
+- `params.txt` 파일이 없을 때 에러가 발생하지 않도록 수정
+- 파이썬 3.9 이하에서 유니온 타입 에러 방지
+
+## 2024-04-14
+
+- v24.4.1
+- webui 1.9.0에서 발생한 에러 수정
+  - extra generation params에 callable이 들어와서 생긴 문제
+  - assign_current_image에 None이 들어갈 수 있던 문제
+- webui 1.9.0에서 변경된 scheduler 지원
+- 컨트롤넷 모델을 찾을 때, 대소문자 구분을 하지 않음 (PR #577)
+- 몇몇 기능을 스크립트에서 분리하여 별도 파일로 빼냄
+
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
+## 2024-03-25
+
+- v24.3.3
+- webui 1.6.0 미만 버전에서 create_binary_mask 함수에 대해 ImportError가 발생하는 것 수정
+
+## 2024-03-21
+
+- v24.3.2
+- UI를 거치지 않은 입력에 대해, image_mask를 입력했을 때 opencv 에러가 발생하는 것 수정
+- img2img inpaint에서 skip img2img 옵션을 활성화할 경우, adetailer를 비활성화함
+  - 마스크 크기에 대해 해결하기 힘든 문제가 있음
+
+## 2024-03-16
+
+- v24.3.1
+- YOLO World v2, YOLO9 지원가능한 버전으로 ultralytics 업데이트
+- inpaint full res인 경우 인페인트 모드에서 동작하게 변경
+- inpaint full res가 아닌 경우, 사용자가 입력한 마스크와 교차점이 있는 마스크만 선택하여 사용함
+
+## 2024-03-01
+
+- v24.3.0
+- YOLO World 모델 추가: 가장 큰 yolov8x-world.pt 모델만 기본적으로 선택할 수 있게 함.
+- lllyasviel/stable-diffusion-webui-forge에서 컨트롤넷을 사용가능하게 함 (PR #517)
+- 기본 스크립트 목록에 soft_inpainting 추가 (https://github.com/AUTOMATIC1111/stable-diffusion-webui/pull/14208)
+
+  - 기존에 설치한 사람에게 소급적용되지는 않음
+
+- 감지모델에 대한 간단한 pytest 추가함
+- xyz grid 컨트롤넷 모델 옵션에 `Passthrough` 추가함
+
+## 2024-01-23
+
+- v24.1.2
+- controlnet 모델에 `Passthrough` 옵션 추가. 입력으로 들어온 컨트롤넷 옵션을 그대로 사용
+- fastapi 엔드포인트 추가
+
+## 2024-01-10
+
+- v24.1.1
+- SDNext 호환 업데이트 (issue #466)
+  - 설정 값 state에 초기값 추가
+  - 위젯 값을 변경할 때마다 state도 변경되게 함 (기존에는 생성 버튼을 누를 때 적용되었음)
+- `inpaint_depth_hand` 컨트롤넷 모델이 depth 모델로 인식되게 함 (issue #463)
+
+## 2024-01-04
+
+- v24.1.0
+- `depth_hand_refiner` ControlNet 추가 (PR #460)
+
+## 2023-12-30
+
+- v23.12.0
+- 파일을 인자로 추가하는 몇몇 스크립트에 대해 deepcopy의 에러를 피하기 위해 script_args 복사 방법을 변경함
+- skip img2img 기능을 사용할 때 너비, 높이를 128로 고정하여 스킵 과정이 조금 더 나아짐
+- img2img inpainting 모드에서 adetailer 자동 비활성화
+- 처음 생성된 params.txt 파일을 항상 유지하도록 변경함
+
+## 2023-11-19
+
+- v23.11.1
+- 기본 스크립트 목록에 negpip 추가
+  - 기존에 설치한 사람에게 소급적용되지는 않음
+- skip img2img 옵션이 2스텝 이상일 때, 제대로 적용되지 않는 문제 수정
+- SD.Next에서 이미지가 np.ndarray로 입력되는 경우 수정
+- 컨트롤넷 경로를 sys.path에 추가하여 --data-dir등을 지정한 경우에도 임포트 에러가 일어나지 않게 함.
+
+## 2023-10-30
+
+- v23.11.0
+- 이미지의 인덱스 계산방법 변경
+  - webui 1.1.0 미만에서 adetailer 실행 불가능하게 함
+- 컨트롤넷 preprocessor 선택지 늘림
+- 추가 yolo 모델 디렉터리를 설정할 수 있는 옵션 추가
+- infotext에 `/`가 있는 항목이 exif에서 복원되지 않는 문제 수정
+  - 이전 버전에 생성된 이미지는 여전히 복원안됨
+- 같은 탭에서 항상 같은 시드를 적용하게 하는 옵션 추가
+- 컨트롤넷 1.1.411 (f2aafcf2beb99a03cbdf7db73852228ccd6bd1d6) 버전을 사용중일 경우,
+  webui 버전 1.6.0 미만에서 사용할 수 없다는 메세지 출력
+
+## 2023-10-15
+
+- v23.10.1
+- xyz grid에 prompt S/R 추가
+- img2img에서 steps가 1일때 에러가 발생하는 샘플러의 처리를 위해 샘플러 이름도 변경하게 수정
+
+## 2023-10-07
+
+- v23.10.0
+- 허깅페이스 모델을 다운로드 실패했을 때, 계속 다운로드를 시도하지 않음
+- img2img에서 img2img단계를 건너뛰는 기능 추가
+- live preview에서 감지 단계를 보여줌 (PR #352)
+
+## 2023-09-20
+
+- v23.9.3
+- ultralytics 버전 8.0.181로 업데이트 (https://github.com/ultralytics/ultralytics/pull/4891)
+- mediapipe와 ultralytics의 lazy import
+
+## 2023-09-10
+
+- v23.9.2
+- (실험적) VAE 선택 기능
+
+## 2023-09-01
+
+- v23.9.1
+- webui 1.6.0에 추가된 인자를 사용해서 생긴 하위 호환 문제 수정
+
+## 2023-08-31
+
+- v23.9.0
+- (실험적) 체크포인트 선택기능
+  - 버그가 있어 리프레시 버튼은 구현에서 빠짐
+- 1.6.0 업데이트에 따라 img2img에서 사용불가능한 샘플러를 선택했을 때 더이상 Euler로 변경하지 않음
+- 유효하지 않은 인자가 전달되었을 때, 에러를 일으키지 않고 대신 adetailer를 비활성화함
+
+## 2023-08-25
+
+- v23.8.1
+- xyz grid에서 model을 `None`으로 설정한 이후에 adetailer가 비활성화 되는 문제 수정
+- skip을 눌렀을 때 진행을 멈춤
+- `--medvram-sdxl`을 설정했을 때에도 cpu를 사용하게 함
+
+## 2023-08-14
+
+- v23.8.0
+- `[PROMPT]` 키워드 추가. `ad_prompt` 또는 `ad_negative_prompt`에 사용하면 입력 프롬프트로 대체됨 (PR #243)
+- Only top k largest 옵션 추가 (PR #264)
+- ultralytics 버전 업데이트
+
+## 2023-07-31
+
+- v23.7.11
+- separate clip skip 옵션 추가
+- install requirements 정리 (ultralytics 새 버전, mediapipe~=3.20)
+
+## 2023-07-28
+
+- v23.7.10
+- ultralytics, mediapipe import문 정리
+- traceback에서 컬러를 없앰 (api 때문), 라이브러리 버전도 보여주게 설정.
+- huggingface_hub, pydantic을 install.py에서 없앰
+- 안쓰는 컨트롤넷 관련 코드 삭제
+
+## 2023-07-23
+
+- v23.7.9
+- `ultralytics.utils` ModuleNotFoundError 해결 (https://github.com/ultralytics/ultralytics/issues/3856)
+- `pydantic` 2.0 이상 버전 설치안되도록 함
+- `controlnet_dir` cmd args 문제 수정 (PR #107)
+
+## 2023-07-20
+
+- v23.7.8
+- `paste_field_names` 추가했던 것을 되돌림
+
+## 2023-07-19
+
+- v23.7.7
+- 인페인팅 단계에서 별도의 샘플러를 선택할 수 있게 옵션을 추가함 (xyz그리드에도 추가)
+- webui 1.0.0-pre 이하 버전에서 batch index 문제 수정
+- 스크립트에 `paste_field_names`을 추가함. 사용되는지는 모르겠음
+
+## 2023-07-16
+
+- v23.7.6
+- `ultralytics 8.0.135`에 추가된 cpuinfo 기능을 위해 `py-cpuinfo`를 미리 설치하게 함. (미리 설치 안하면 cpu나 mps사용할 때 재시작해야함)
+- init_image가 RGB 모드가 아닐 때 RGB로 변경.
+
+## 2023-07-07
+
+- v23.7.4
+- batch count > 1일때 프롬프트의 인덱스 문제 수정
+
+- v23.7.5
+- i2i의 `cached_uc`와 `cached_c`가 p의 `cached_uc`와 `cached_c`가 다른 인스턴스가 되도록 수정
+
+## 2023-07-05
+
+- v23.7.3
+- 버그 수정
+  - `object()`가 json 직렬화 안되는 문제
+  - `process`를 호출함에 따라 배치 카운트가 2이상일 때, all_prompts가 고정되는 문제
+  - `ad-before`와 `ad-preview` 이미지 파일명이 실제 파일명과 다른 문제
+  - pydantic 2.0 호환성 문제
+
+## 2023-07-04
+
+- v23.7.2
+- `mediapipe_face_mesh_eyes_only` 모델 추가: `mediapipe_face_mesh`로 감지한 뒤 눈만 사용함.
+- 매 배치 시작 전에 `scripts.postprocess`를, 후에 `scripts.process`를 호출함.
+  - 컨트롤넷을 사용하면 소요 시간이 조금 늘어나지만 몇몇 문제 해결에 도움이 됨.
+- `lora_block_weight`를 스크립트 화이트리스트에 추가함.
+  - 한번이라도 ADetailer를 사용한 사람은 수동으로 추가해야함.
+
+## 2023-07-03
+
+- v23.7.1
+- `process_images`를 진행한 뒤 `StableDiffusionProcessing` 오브젝트의 close를 호출함
+- api 호출로 사용했는지 확인하는 속성 추가
+- `NansException`이 발생했을 때 중지하지 않고 남은 과정 계속 진행함
+
+## 2023-07-02
+
+- v23.7.0
+- `NansException`이 발생하면 로그에 표시하고 원본 이미지를 반환하게 설정
+- `rich`를 사용한 에러 트레이싱
+  - install.py에 `rich` 추가
+- 생성 중에 컴포넌트의 값을 변경하면 args의 값도 함께 변경되는 문제 수정 (issue #180)
+- 터미널 로그로 ad_prompt와 ad_negative_prompt에 적용된 실제 프롬프트 확인할 수 있음 (입력과 다를 경우에만)
+
+## 2023-06-28
+
+- v23.6.4
+- 최대 모델 수 5 -> 10개
+- ad_prompt와 ad_negative_prompt에 빈칸으로 놔두면 입력 프롬프트가 사용된다는 문구 추가
+- huggingface 모델 다운로드 실패시 로깅
+- 1st 모델이 `None`일 경우 나머지 입력을 무시하던 문제 수정
+- `--use-cpu` 에 `adetailer` 입력 시 cpu로 yolo모델을 사용함
+
+## 2023-06-20
+
+- v23.6.3
+- 컨트롤넷 inpaint 모델에 대해, 3가지 모듈을 사용할 수 있도록 함
+- Noise Multiplier 옵션 추가 (PR #149)
+- pydantic 최소 버전 1.10.8로 설정 (Issue #146)
+
+## 2023-06-05
+
+- v23.6.2
+- xyz_grid에서 ADetailer를 사용할 수 있게함.
+  - 8가지 옵션만 1st 탭에 적용되도록 함.
+
+## 2023-06-01
+
+- v23.6.1
+- `inpaint, scribble, lineart, openpose, tile` 5가지 컨트롤넷 모델 지원 (PR #107)
+- controlnet guidance start, end 인자 추가 (PR #107)
+- `modules.extensions`를 사용하여 컨트롤넷 확장을 불러오고 경로를 알아내로록 변경
+- ui에서 컨트롤넷을 별도 함수로 분리
+
+## 2023-05-30
+
+- v23.6.0
+- 스크립트의 이름을 `After Detailer`에서 `ADetailer`로 변경
+  - API 사용자는 변경 필요함
+- 몇몇 설정 변경
+  - `ad_conf` → `ad_confidence`. 0~100 사이의 int → 0.0~1.0 사이의 float
+  - `ad_inpaint_full_res` → `ad_inpaint_only_masked`
+  - `ad_inpaint_full_res_padding` → `ad_inpaint_only_masked_padding`
+- mediapipe face mesh 모델 추가
+
+  - mediapipe 최소 버전 `0.10.0`
+
+- rich traceback 제거함
+- huggingface 다운로드 실패할 때 에러가 나지 않게 하고 해당 모델을 제거함
+
+## 2023-05-26
+
+- v23.5.19
+- 1번째 탭에도 `None` 옵션을 추가함
+- api로 ad controlnet model에 inpaint가 아닌 다른 컨트롤넷 모델을 사용하지 못하도록 막음
+- adetailer 진행중에 total tqdm 진행바 업데이트를 멈춤
+- state.inturrupted 상태에서 adetailer 과정을 중지함
+- 컨트롤넷 process를 각 batch가 끝난 순간에만 호출하도록 변경
+
+### 2023-05-25
+
+- v23.5.18
+- 컨트롤넷 관련 수정
+  - unit의 `input_mode`를 `SIMPLE`로 모두 변경
+  - 컨트롤넷 유넷 훅과 하이잭 함수들을 adetailer를 실행할 때에만 되돌리는 기능 추가
+  - adetailer 처리가 끝난 뒤 컨트롤넷 스크립트의 process를 다시 진행함. (batch count 2 이상일때의 문제 해결)
+- 기본 활성 스크립트 목록에서 컨트롤넷을 뺌
+
+### 2023-05-22
+
+- v23.5.17
+- 컨트롤넷 확장이 있으면 컨트롤넷 스크립트를 활성화함. (컨트롤넷 관련 문제 해결)
+- 모든 컴포넌트에 elem_id 설정
+- ui에 버전을 표시함
+
+### 2023-05-19
+
+- v23.5.16
+- 추가한 옵션
+  - Mask min/max ratio
+  - Mask merge mode
+  - Restore faces after ADetailer
+- 옵션들을 Accordion으로 묶음
+
+### 2023-05-18
+
+- v23.5.15
+- 필요한 것만 임포트하도록 변경 (vae 로딩 오류 없어짐. 로딩 속도 빨라짐)
+
+### 2023-05-17
+
+- v23.5.14
+- `[SKIP]`으로 ad prompt 일부를 건너뛰는 기능 추가
+- bbox 정렬 옵션 추가
+- sd_webui 타입힌트를 만들어냄
+- enable checker와 관련된 api 오류 수정?
+
+### 2023-05-15
+
+- v23.5.13
+- `[SEP]`으로 ad prompt를 분리하여 적용하는 기능 추가
+- enable checker를 다시 pydantic으로 변경함
+- ui 관련 함수를 adetailer.ui 폴더로 분리함
+- controlnet을 사용할 때 모든 controlnet unit 비활성화
+- adetailer 폴더가 없으면 만들게 함
+
+### 2023-05-13
+
+- v23.5.12
+- `ad_enable`을 제외한 입력이 dict타입으로 들어오도록 변경
+  - web api로 사용할 때에 특히 사용하기 쉬움
+  - web api breaking change
+- `mask_preprocess` 인자를 넣지 않았던 오류 수정 (PR #47)
+- huggingface에서 모델을 다운로드하지 않는 옵션 추가 `--ad-no-huggingface`
+
+### 2023-05-12
+
+- v23.5.11
+- `ultralytics` 알람 제거
+- 필요없는 exif 인자 더 제거함
+- `use separate steps` 옵션 추가
+- ui 배치를 조정함
+
+### 2023-05-09
+
+- v23.5.10
+- 선택한 스크립트만 ADetailer에 적용하는 옵션 추가, 기본값 `True`. 설정 탭에서 지정가능.
+  - 기본값: `dynamic_prompting,dynamic_thresholding,wildcards,wildcard_recursive`
+- `person_yolov8s-seg.pt` 모델 추가
+- `ultralytics`의 최소 버전을 `8.0.97`로 설정 (C:\\ 문제 해결된 버전)
+
+### 2023-05-08
+
+- v23.5.9
+- 2가지 이상의 모델을 사용할 수 있음. 기본값: 2, 최대: 5
+- segment 모델을 사용할 수 있게 함. `person_yolov8n-seg.pt` 추가
+
+### 2023-05-07
+
+- v23.5.8
+- 프롬프트와 네거티브 프롬프트에 방향키 지원 (PR #24)
+- `mask_preprocess`를 추가함. 이전 버전과 시드값이 달라질 가능성 있음!
+- 이미지 처리가 일어났을 때에만 before이미지를 저장함
+- 설정창의 레이블을 ADetailer 대신 더 적절하게 수정함
+
+### 2023-05-06
+
+- v23.5.7
+- `ad_use_cfg_scale` 옵션 추가. cfg 스케일을 따로 사용할지 말지 결정함.
+- `ad_enable` 기본값을 `True`에서 `False`로 변경
+- `ad_model`의 기본값을 `None`에서 첫번째 모델로 변경
+- 최소 2개의 입력(ad_enable, ad_model)만 들어오면 작동하게 변경.
+
+- v23.5.7.post0
+- `init_controlnet_ext`을 controlnet_exists == True일때에만 실행
+- webui를 C드라이브 바로 밑에 설치한 사람들에게 `ultralytics` 경고 표시
+
+### 2023-05-05 (어린이날)
+
+- v23.5.5
+- `Save images before ADetailer` 옵션 추가
+- 입력으로 들어온 인자와 ALL_ARGS의 길이가 다르면 에러메세지
+- README.md에 설치방법 추가
+
+- v23.5.6
+- get_args에서 IndexError가 발생하면 자세한 에러메세지를 볼 수 있음
+- AdetailerArgs에 extra_params 내장
+- scripts_args를 딥카피함
+- postprocess_image를 약간 분리함
+
+- v23.5.6.post0
+- `init_controlnet_ext`에서 에러메세지를 자세히 볼 수 있음
+
+### 2023-05-04
+
+- v23.5.4
+- use pydantic for arguments validation
+- revert: ad_model to `None` as default
+- revert: `__future__` imports
+- lazily import yolo and mediapipe
+
+### 2023-05-03
+
+- v23.5.3.post0
+- remove `__future__` imports
+- change to copy scripts and scripts args
+
+- v23.5.3.post1
+- change default ad_model from `None`
+
+### 2023-05-02
+
+- v23.5.3
+- Remove `None` from model list and add `Enable ADetailer` checkbox.
+- install.py `skip_install` fix.
```

### Comparing `adetailer-24.4.1/Taskfile.yml` & `adetailer-24.4.2/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.1/install.py` & `adetailer-24.4.2/install.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-from __future__ import annotations
-
-import importlib.util
-import subprocess
-import sys
-from importlib.metadata import version  # python >= 3.8
-
-from packaging.version import parse
-
-import_name = {"py-cpuinfo": "cpuinfo", "protobuf": "google.protobuf"}
-
-
-def is_installed(
-    package: str, min_version: str | None = None, max_version: str | None = None
-):
-    name = import_name.get(package, package)
-    try:
-        spec = importlib.util.find_spec(name)
-    except ModuleNotFoundError:
-        return False
-
-    if spec is None:
-        return False
-
-    if not min_version and not max_version:
-        return True
-
-    if not min_version:
-        min_version = "0.0.0"
-    if not max_version:
-        max_version = "99999999.99999999.99999999"
-
-    try:
-        pkg_version = version(package)
-        return parse(min_version) <= parse(pkg_version) <= parse(max_version)
-    except Exception:
-        return False
-
-
-def run_pip(*args):
-    subprocess.run([sys.executable, "-m", "pip", "install", *args])
-
-
-def install():
-    deps = [
-        # requirements
-        ("ultralytics", "8.1.29", None),
-        ("mediapipe", "0.10.9", None),
-        ("rich", "13.0.0", None),
-        # mediapipe
-        ("protobuf", "3.20", "3.9999"),
-    ]
-
-    for pkg, low, high in deps:
-        if not is_installed(pkg, low, high):
-            if low and high:
-                cmd = f"{pkg}>={low},<={high}"
-            elif low:
-                cmd = f"{pkg}>={low}"
-            elif high:
-                cmd = f"{pkg}<={high}"
-            else:
-                cmd = pkg
-
-            run_pip("-U", cmd)
-
-
-try:
-    import launch
-
-    skip_install = launch.args.skip_install
-except Exception:
-    skip_install = False
-
-if not skip_install:
-    install()
+from __future__ import annotations
+
+import importlib.util
+import subprocess
+import sys
+from importlib.metadata import version  # python >= 3.8
+
+from packaging.version import parse
+
+import_name = {"py-cpuinfo": "cpuinfo", "protobuf": "google.protobuf"}
+
+
+def is_installed(
+    package: str, min_version: str | None = None, max_version: str | None = None
+):
+    name = import_name.get(package, package)
+    try:
+        spec = importlib.util.find_spec(name)
+    except ModuleNotFoundError:
+        return False
+
+    if spec is None:
+        return False
+
+    if not min_version and not max_version:
+        return True
+
+    if not min_version:
+        min_version = "0.0.0"
+    if not max_version:
+        max_version = "99999999.99999999.99999999"
+
+    try:
+        pkg_version = version(package)
+        return parse(min_version) <= parse(pkg_version) <= parse(max_version)
+    except Exception:
+        return False
+
+
+def run_pip(*args):
+    subprocess.run([sys.executable, "-m", "pip", "install", *args])
+
+
+def install():
+    deps = [
+        # requirements
+        ("ultralytics", "8.1.29", None),
+        ("mediapipe", "0.10.9", None),
+        ("rich", "13.0.0", None),
+        # mediapipe
+        ("protobuf", "3.20", "3.9999"),
+    ]
+
+    for pkg, low, high in deps:
+        if not is_installed(pkg, low, high):
+            if low and high:
+                cmd = f"{pkg}>={low},<={high}"
+            elif low:
+                cmd = f"{pkg}>={low}"
+            elif high:
+                cmd = f"{pkg}<={high}"
+            else:
+                cmd = pkg
+
+            run_pip("-U", cmd)
+
+
+try:
+    import launch
+
+    skip_install = launch.args.skip_install
+except Exception:
+    skip_install = False
+
+if not skip_install:
+    install()
```

### Comparing `adetailer-24.4.1/.github/ISSUE_TEMPLATE/bug_report.yaml` & `adetailer-24.4.2/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.1/.github/ISSUE_TEMPLATE/feature_request.yaml` & `adetailer-24.4.2/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.1/.github/workflows/pypi.yml` & `adetailer-24.4.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.1/aaaaaa/helper.py` & `adetailer-24.4.2/aaaaaa/helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from __future__ import annotations
-
-from contextlib import contextmanager
-from copy import copy
-from typing import TYPE_CHECKING, Any
-
-import torch
-
-from modules import safe
-from modules.shared import opts
-
-if TYPE_CHECKING:
-    # 타입 체커가 빨간 줄을 긋지 않게 하는 편법
-    from types import SimpleNamespace
-
-    StableDiffusionProcessingTxt2Img = SimpleNamespace
-    StableDiffusionProcessingImg2Img = SimpleNamespace
-else:
-    from modules.processing import (
-        StableDiffusionProcessingImg2Img,
-        StableDiffusionProcessingTxt2Img,
-    )
-
-PT = StableDiffusionProcessingTxt2Img | StableDiffusionProcessingImg2Img
-
-
-@contextmanager
-def change_torch_load():
-    orig = torch.load
-    try:
-        torch.load = safe.unsafe_torch_load
-        yield
-    finally:
-        torch.load = orig
-
-
-@contextmanager
-def pause_total_tqdm():
-    orig = opts.data.get("multiple_tqdm", True)
-    try:
-        opts.data["multiple_tqdm"] = False
-        yield
-    finally:
-        opts.data["multiple_tqdm"] = orig
-
-
-@contextmanager
-def preseve_prompts(p: PT):
-    all_pt = copy(p.all_prompts)
-    all_ng = copy(p.all_negative_prompts)
-    try:
-        yield
-    finally:
-        p.all_prompts = all_pt
-        p.all_negative_prompts = all_ng
-
-
-def copy_extra_params(extra_params: dict[str, Any]) -> dict[str, Any]:
-    return {k: v for k, v in extra_params.items() if not callable(v)}
+from __future__ import annotations
+
+from contextlib import contextmanager
+from copy import copy
+from typing import TYPE_CHECKING, Any, Union
+
+import torch
+
+from modules import safe
+from modules.shared import opts
+
+if TYPE_CHECKING:
+    # 타입 체커가 빨간 줄을 긋지 않게 하는 편법
+    from types import SimpleNamespace
+
+    StableDiffusionProcessingTxt2Img = SimpleNamespace
+    StableDiffusionProcessingImg2Img = SimpleNamespace
+else:
+    from modules.processing import (
+        StableDiffusionProcessingImg2Img,
+        StableDiffusionProcessingTxt2Img,
+    )
+
+PT = Union[StableDiffusionProcessingTxt2Img, StableDiffusionProcessingImg2Img]
+
+
+@contextmanager
+def change_torch_load():
+    orig = torch.load
+    try:
+        torch.load = safe.unsafe_torch_load
+        yield
+    finally:
+        torch.load = orig
+
+
+@contextmanager
+def pause_total_tqdm():
+    orig = opts.data.get("multiple_tqdm", True)
+    try:
+        opts.data["multiple_tqdm"] = False
+        yield
+    finally:
+        opts.data["multiple_tqdm"] = orig
+
+
+@contextmanager
+def preseve_prompts(p: PT):
+    all_pt = copy(p.all_prompts)
+    all_ng = copy(p.all_negative_prompts)
+    try:
+        yield
+    finally:
+        p.all_prompts = all_pt
+        p.all_negative_prompts = all_ng
+
+
+def copy_extra_params(extra_params: dict[str, Any]) -> dict[str, Any]:
+    return {k: v for k, v in extra_params.items() if not callable(v)}
```

### Comparing `adetailer-24.4.1/adetailer/args.py` & `adetailer-24.4.2/adetailer/args.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,267 +1,267 @@
-from __future__ import annotations
-
-from collections import UserList
-from dataclasses import dataclass
-from functools import cached_property, partial
-from typing import Any, Literal, NamedTuple, Optional
-
-try:
-    from pydantic.v1 import (
-        BaseModel,
-        Extra,
-        NonNegativeFloat,
-        NonNegativeInt,
-        PositiveInt,
-        confloat,
-        conint,
-        validator,
-    )
-except ImportError:
-    from pydantic import (
-        BaseModel,
-        Extra,
-        NonNegativeFloat,
-        NonNegativeInt,
-        PositiveInt,
-        confloat,
-        conint,
-        validator,
-    )
-
-
-@dataclass
-class SkipImg2ImgOrig:
-    steps: int
-    sampler_name: str
-    width: int
-    height: int
-
-
-class Arg(NamedTuple):
-    attr: str
-    name: str
-
-
-class ArgsList(UserList):
-    @cached_property
-    def attrs(self) -> tuple[str, ...]:
-        return tuple(attr for attr, _ in self)
-
-    @cached_property
-    def names(self) -> tuple[str, ...]:
-        return tuple(name for _, name in self)
-
-
-class ADetailerArgs(BaseModel, extra=Extra.forbid):
-    ad_model: str = "None"
-    ad_model_classes: str = ""
-    ad_prompt: str = ""
-    ad_negative_prompt: str = ""
-    ad_confidence: confloat(ge=0.0, le=1.0) = 0.3
-    ad_mask_k_largest: NonNegativeInt = 0
-    ad_mask_min_ratio: confloat(ge=0.0, le=1.0) = 0.0
-    ad_mask_max_ratio: confloat(ge=0.0, le=1.0) = 1.0
-    ad_dilate_erode: int = 4
-    ad_x_offset: int = 0
-    ad_y_offset: int = 0
-    ad_mask_merge_invert: Literal["None", "Merge", "Merge and Invert"] = "None"
-    ad_mask_blur: NonNegativeInt = 4
-    ad_denoising_strength: confloat(ge=0.0, le=1.0) = 0.4
-    ad_inpaint_only_masked: bool = True
-    ad_inpaint_only_masked_padding: NonNegativeInt = 32
-    ad_use_inpaint_width_height: bool = False
-    ad_inpaint_width: PositiveInt = 512
-    ad_inpaint_height: PositiveInt = 512
-    ad_use_steps: bool = False
-    ad_steps: PositiveInt = 28
-    ad_use_cfg_scale: bool = False
-    ad_cfg_scale: NonNegativeFloat = 7.0
-    ad_use_checkpoint: bool = False
-    ad_checkpoint: Optional[str] = None
-    ad_use_vae: bool = False
-    ad_vae: Optional[str] = None
-    ad_use_sampler: bool = False
-    ad_sampler: str = "DPM++ 2M Karras"
-    ad_scheduler: str = "Use same scheduler"
-    ad_use_noise_multiplier: bool = False
-    ad_noise_multiplier: confloat(ge=0.5, le=1.5) = 1.0
-    ad_use_clip_skip: bool = False
-    ad_clip_skip: conint(ge=1, le=12) = 1
-    ad_restore_face: bool = False
-    ad_controlnet_model: str = "None"
-    ad_controlnet_module: str = "None"
-    ad_controlnet_weight: confloat(ge=0.0, le=1.0) = 1.0
-    ad_controlnet_guidance_start: confloat(ge=0.0, le=1.0) = 0.0
-    ad_controlnet_guidance_end: confloat(ge=0.0, le=1.0) = 1.0
-    is_api: bool = True
-
-    @validator("is_api", pre=True)
-    def is_api_validator(cls, v: Any):  # noqa: N805
-        "tuple is json serializable but cannot be made with json deserialize."
-        return type(v) is not tuple
-
-    @staticmethod
-    def ppop(
-        p: dict[str, Any],
-        key: str,
-        pops: list[str] | None = None,
-        cond: Any = None,
-    ) -> None:
-        if pops is None:
-            pops = [key]
-        if key not in p:
-            return
-        value = p[key]
-        cond = (not bool(value)) if cond is None else value == cond
-
-        if cond:
-            for k in pops:
-                p.pop(k, None)
-
-    def extra_params(self, suffix: str = "") -> dict[str, Any]:
-        if self.ad_model == "None":
-            return {}
-
-        p = {name: getattr(self, attr) for attr, name in ALL_ARGS}
-        ppop = partial(self.ppop, p)
-
-        ppop("ADetailer model classes")
-        ppop("ADetailer prompt")
-        ppop("ADetailer negative prompt")
-        ppop("ADetailer mask only top k largest", cond=0)
-        ppop("ADetailer mask min ratio", cond=0.0)
-        ppop("ADetailer mask max ratio", cond=1.0)
-        ppop("ADetailer x offset", cond=0)
-        ppop("ADetailer y offset", cond=0)
-        ppop("ADetailer mask merge invert", cond="None")
-        ppop("ADetailer inpaint only masked", ["ADetailer inpaint padding"])
-        ppop(
-            "ADetailer use inpaint width height",
-            [
-                "ADetailer use inpaint width height",
-                "ADetailer inpaint width",
-                "ADetailer inpaint height",
-            ],
-        )
-        ppop(
-            "ADetailer use separate steps",
-            ["ADetailer use separate steps", "ADetailer steps"],
-        )
-        ppop(
-            "ADetailer use separate CFG scale",
-            ["ADetailer use separate CFG scale", "ADetailer CFG scale"],
-        )
-        ppop(
-            "ADetailer use separate checkpoint",
-            ["ADetailer use separate checkpoint", "ADetailer checkpoint"],
-        )
-        ppop(
-            "ADetailer use separate VAE",
-            ["ADetailer use separate VAE", "ADetailer VAE"],
-        )
-        ppop(
-            "ADetailer use separate sampler",
-            [
-                "ADetailer use separate sampler",
-                "ADetailer sampler",
-                "ADetailer scheduler",
-            ],
-        )
-        ppop("ADetailer scheduler", cond="Use same scheduler")
-        ppop(
-            "ADetailer use separate noise multiplier",
-            ["ADetailer use separate noise multiplier", "ADetailer noise multiplier"],
-        )
-
-        ppop(
-            "ADetailer use separate CLIP skip",
-            ["ADetailer use separate CLIP skip", "ADetailer CLIP skip"],
-        )
-
-        ppop("ADetailer restore face")
-        ppop(
-            "ADetailer ControlNet model",
-            [
-                "ADetailer ControlNet model",
-                "ADetailer ControlNet module",
-                "ADetailer ControlNet weight",
-                "ADetailer ControlNet guidance start",
-                "ADetailer ControlNet guidance end",
-            ],
-            cond="None",
-        )
-        ppop("ADetailer ControlNet module", cond="None")
-        ppop("ADetailer ControlNet weight", cond=1.0)
-        ppop("ADetailer ControlNet guidance start", cond=0.0)
-        ppop("ADetailer ControlNet guidance end", cond=1.0)
-
-        if suffix:
-            p = {k + suffix: v for k, v in p.items()}
-
-        return p
-
-
-_all_args = [
-    ("ad_model", "ADetailer model"),
-    ("ad_model_classes", "ADetailer model classes"),
-    ("ad_prompt", "ADetailer prompt"),
-    ("ad_negative_prompt", "ADetailer negative prompt"),
-    ("ad_confidence", "ADetailer confidence"),
-    ("ad_mask_k_largest", "ADetailer mask only top k largest"),
-    ("ad_mask_min_ratio", "ADetailer mask min ratio"),
-    ("ad_mask_max_ratio", "ADetailer mask max ratio"),
-    ("ad_x_offset", "ADetailer x offset"),
-    ("ad_y_offset", "ADetailer y offset"),
-    ("ad_dilate_erode", "ADetailer dilate erode"),
-    ("ad_mask_merge_invert", "ADetailer mask merge invert"),
-    ("ad_mask_blur", "ADetailer mask blur"),
-    ("ad_denoising_strength", "ADetailer denoising strength"),
-    ("ad_inpaint_only_masked", "ADetailer inpaint only masked"),
-    ("ad_inpaint_only_masked_padding", "ADetailer inpaint padding"),
-    ("ad_use_inpaint_width_height", "ADetailer use inpaint width height"),
-    ("ad_inpaint_width", "ADetailer inpaint width"),
-    ("ad_inpaint_height", "ADetailer inpaint height"),
-    ("ad_use_steps", "ADetailer use separate steps"),
-    ("ad_steps", "ADetailer steps"),
-    ("ad_use_cfg_scale", "ADetailer use separate CFG scale"),
-    ("ad_cfg_scale", "ADetailer CFG scale"),
-    ("ad_use_checkpoint", "ADetailer use separate checkpoint"),
-    ("ad_checkpoint", "ADetailer checkpoint"),
-    ("ad_use_vae", "ADetailer use separate VAE"),
-    ("ad_vae", "ADetailer VAE"),
-    ("ad_use_sampler", "ADetailer use separate sampler"),
-    ("ad_sampler", "ADetailer sampler"),
-    ("ad_scheduler", "ADetailer scheduler"),
-    ("ad_use_noise_multiplier", "ADetailer use separate noise multiplier"),
-    ("ad_noise_multiplier", "ADetailer noise multiplier"),
-    ("ad_use_clip_skip", "ADetailer use separate CLIP skip"),
-    ("ad_clip_skip", "ADetailer CLIP skip"),
-    ("ad_restore_face", "ADetailer restore face"),
-    ("ad_controlnet_model", "ADetailer ControlNet model"),
-    ("ad_controlnet_module", "ADetailer ControlNet module"),
-    ("ad_controlnet_weight", "ADetailer ControlNet weight"),
-    ("ad_controlnet_guidance_start", "ADetailer ControlNet guidance start"),
-    ("ad_controlnet_guidance_end", "ADetailer ControlNet guidance end"),
-]
-
-_args = [Arg(*args) for args in _all_args]
-ALL_ARGS = ArgsList(_args)
-
-BBOX_SORTBY = [
-    "None",
-    "Position (left to right)",
-    "Position (center to edge)",
-    "Area (large to small)",
-]
-MASK_MERGE_INVERT = ["None", "Merge", "Merge and Invert"]
-
-_script_default = (
-    "dynamic_prompting",
-    "dynamic_thresholding",
-    "wildcard_recursive",
-    "wildcards",
-    "lora_block_weight",
-    "negpip",
-    "soft_inpainting",
-)
-SCRIPT_DEFAULT = ",".join(sorted(_script_default))
+from __future__ import annotations
+
+from collections import UserList
+from dataclasses import dataclass
+from functools import cached_property, partial
+from typing import Any, Literal, NamedTuple, Optional
+
+try:
+    from pydantic.v1 import (
+        BaseModel,
+        Extra,
+        NonNegativeFloat,
+        NonNegativeInt,
+        PositiveInt,
+        confloat,
+        conint,
+        validator,
+    )
+except ImportError:
+    from pydantic import (
+        BaseModel,
+        Extra,
+        NonNegativeFloat,
+        NonNegativeInt,
+        PositiveInt,
+        confloat,
+        conint,
+        validator,
+    )
+
+
+@dataclass
+class SkipImg2ImgOrig:
+    steps: int
+    sampler_name: str
+    width: int
+    height: int
+
+
+class Arg(NamedTuple):
+    attr: str
+    name: str
+
+
+class ArgsList(UserList):
+    @cached_property
+    def attrs(self) -> tuple[str, ...]:
+        return tuple(attr for attr, _ in self)
+
+    @cached_property
+    def names(self) -> tuple[str, ...]:
+        return tuple(name for _, name in self)
+
+
+class ADetailerArgs(BaseModel, extra=Extra.forbid):
+    ad_model: str = "None"
+    ad_model_classes: str = ""
+    ad_prompt: str = ""
+    ad_negative_prompt: str = ""
+    ad_confidence: confloat(ge=0.0, le=1.0) = 0.3
+    ad_mask_k_largest: NonNegativeInt = 0
+    ad_mask_min_ratio: confloat(ge=0.0, le=1.0) = 0.0
+    ad_mask_max_ratio: confloat(ge=0.0, le=1.0) = 1.0
+    ad_dilate_erode: int = 4
+    ad_x_offset: int = 0
+    ad_y_offset: int = 0
+    ad_mask_merge_invert: Literal["None", "Merge", "Merge and Invert"] = "None"
+    ad_mask_blur: NonNegativeInt = 4
+    ad_denoising_strength: confloat(ge=0.0, le=1.0) = 0.4
+    ad_inpaint_only_masked: bool = True
+    ad_inpaint_only_masked_padding: NonNegativeInt = 32
+    ad_use_inpaint_width_height: bool = False
+    ad_inpaint_width: PositiveInt = 512
+    ad_inpaint_height: PositiveInt = 512
+    ad_use_steps: bool = False
+    ad_steps: PositiveInt = 28
+    ad_use_cfg_scale: bool = False
+    ad_cfg_scale: NonNegativeFloat = 7.0
+    ad_use_checkpoint: bool = False
+    ad_checkpoint: Optional[str] = None
+    ad_use_vae: bool = False
+    ad_vae: Optional[str] = None
+    ad_use_sampler: bool = False
+    ad_sampler: str = "DPM++ 2M Karras"
+    ad_scheduler: str = "Use same scheduler"
+    ad_use_noise_multiplier: bool = False
+    ad_noise_multiplier: confloat(ge=0.5, le=1.5) = 1.0
+    ad_use_clip_skip: bool = False
+    ad_clip_skip: conint(ge=1, le=12) = 1
+    ad_restore_face: bool = False
+    ad_controlnet_model: str = "None"
+    ad_controlnet_module: str = "None"
+    ad_controlnet_weight: confloat(ge=0.0, le=1.0) = 1.0
+    ad_controlnet_guidance_start: confloat(ge=0.0, le=1.0) = 0.0
+    ad_controlnet_guidance_end: confloat(ge=0.0, le=1.0) = 1.0
+    is_api: bool = True
+
+    @validator("is_api", pre=True)
+    def is_api_validator(cls, v: Any):  # noqa: N805
+        "tuple is json serializable but cannot be made with json deserialize."
+        return type(v) is not tuple
+
+    @staticmethod
+    def ppop(
+        p: dict[str, Any],
+        key: str,
+        pops: list[str] | None = None,
+        cond: Any = None,
+    ) -> None:
+        if pops is None:
+            pops = [key]
+        if key not in p:
+            return
+        value = p[key]
+        cond = (not bool(value)) if cond is None else value == cond
+
+        if cond:
+            for k in pops:
+                p.pop(k, None)
+
+    def extra_params(self, suffix: str = "") -> dict[str, Any]:
+        if self.ad_model == "None":
+            return {}
+
+        p = {name: getattr(self, attr) for attr, name in ALL_ARGS}
+        ppop = partial(self.ppop, p)
+
+        ppop("ADetailer model classes")
+        ppop("ADetailer prompt")
+        ppop("ADetailer negative prompt")
+        ppop("ADetailer mask only top k largest", cond=0)
+        ppop("ADetailer mask min ratio", cond=0.0)
+        ppop("ADetailer mask max ratio", cond=1.0)
+        ppop("ADetailer x offset", cond=0)
+        ppop("ADetailer y offset", cond=0)
+        ppop("ADetailer mask merge invert", cond="None")
+        ppop("ADetailer inpaint only masked", ["ADetailer inpaint padding"])
+        ppop(
+            "ADetailer use inpaint width height",
+            [
+                "ADetailer use inpaint width height",
+                "ADetailer inpaint width",
+                "ADetailer inpaint height",
+            ],
+        )
+        ppop(
+            "ADetailer use separate steps",
+            ["ADetailer use separate steps", "ADetailer steps"],
+        )
+        ppop(
+            "ADetailer use separate CFG scale",
+            ["ADetailer use separate CFG scale", "ADetailer CFG scale"],
+        )
+        ppop(
+            "ADetailer use separate checkpoint",
+            ["ADetailer use separate checkpoint", "ADetailer checkpoint"],
+        )
+        ppop(
+            "ADetailer use separate VAE",
+            ["ADetailer use separate VAE", "ADetailer VAE"],
+        )
+        ppop(
+            "ADetailer use separate sampler",
+            [
+                "ADetailer use separate sampler",
+                "ADetailer sampler",
+                "ADetailer scheduler",
+            ],
+        )
+        ppop("ADetailer scheduler", cond="Use same scheduler")
+        ppop(
+            "ADetailer use separate noise multiplier",
+            ["ADetailer use separate noise multiplier", "ADetailer noise multiplier"],
+        )
+
+        ppop(
+            "ADetailer use separate CLIP skip",
+            ["ADetailer use separate CLIP skip", "ADetailer CLIP skip"],
+        )
+
+        ppop("ADetailer restore face")
+        ppop(
+            "ADetailer ControlNet model",
+            [
+                "ADetailer ControlNet model",
+                "ADetailer ControlNet module",
+                "ADetailer ControlNet weight",
+                "ADetailer ControlNet guidance start",
+                "ADetailer ControlNet guidance end",
+            ],
+            cond="None",
+        )
+        ppop("ADetailer ControlNet module", cond="None")
+        ppop("ADetailer ControlNet weight", cond=1.0)
+        ppop("ADetailer ControlNet guidance start", cond=0.0)
+        ppop("ADetailer ControlNet guidance end", cond=1.0)
+
+        if suffix:
+            p = {k + suffix: v for k, v in p.items()}
+
+        return p
+
+
+_all_args = [
+    ("ad_model", "ADetailer model"),
+    ("ad_model_classes", "ADetailer model classes"),
+    ("ad_prompt", "ADetailer prompt"),
+    ("ad_negative_prompt", "ADetailer negative prompt"),
+    ("ad_confidence", "ADetailer confidence"),
+    ("ad_mask_k_largest", "ADetailer mask only top k largest"),
+    ("ad_mask_min_ratio", "ADetailer mask min ratio"),
+    ("ad_mask_max_ratio", "ADetailer mask max ratio"),
+    ("ad_x_offset", "ADetailer x offset"),
+    ("ad_y_offset", "ADetailer y offset"),
+    ("ad_dilate_erode", "ADetailer dilate erode"),
+    ("ad_mask_merge_invert", "ADetailer mask merge invert"),
+    ("ad_mask_blur", "ADetailer mask blur"),
+    ("ad_denoising_strength", "ADetailer denoising strength"),
+    ("ad_inpaint_only_masked", "ADetailer inpaint only masked"),
+    ("ad_inpaint_only_masked_padding", "ADetailer inpaint padding"),
+    ("ad_use_inpaint_width_height", "ADetailer use inpaint width height"),
+    ("ad_inpaint_width", "ADetailer inpaint width"),
+    ("ad_inpaint_height", "ADetailer inpaint height"),
+    ("ad_use_steps", "ADetailer use separate steps"),
+    ("ad_steps", "ADetailer steps"),
+    ("ad_use_cfg_scale", "ADetailer use separate CFG scale"),
+    ("ad_cfg_scale", "ADetailer CFG scale"),
+    ("ad_use_checkpoint", "ADetailer use separate checkpoint"),
+    ("ad_checkpoint", "ADetailer checkpoint"),
+    ("ad_use_vae", "ADetailer use separate VAE"),
+    ("ad_vae", "ADetailer VAE"),
+    ("ad_use_sampler", "ADetailer use separate sampler"),
+    ("ad_sampler", "ADetailer sampler"),
+    ("ad_scheduler", "ADetailer scheduler"),
+    ("ad_use_noise_multiplier", "ADetailer use separate noise multiplier"),
+    ("ad_noise_multiplier", "ADetailer noise multiplier"),
+    ("ad_use_clip_skip", "ADetailer use separate CLIP skip"),
+    ("ad_clip_skip", "ADetailer CLIP skip"),
+    ("ad_restore_face", "ADetailer restore face"),
+    ("ad_controlnet_model", "ADetailer ControlNet model"),
+    ("ad_controlnet_module", "ADetailer ControlNet module"),
+    ("ad_controlnet_weight", "ADetailer ControlNet weight"),
+    ("ad_controlnet_guidance_start", "ADetailer ControlNet guidance start"),
+    ("ad_controlnet_guidance_end", "ADetailer ControlNet guidance end"),
+]
+
+_args = [Arg(*args) for args in _all_args]
+ALL_ARGS = ArgsList(_args)
+
+BBOX_SORTBY = [
+    "None",
+    "Position (left to right)",
+    "Position (center to edge)",
+    "Area (large to small)",
+]
+MASK_MERGE_INVERT = ["None", "Merge", "Merge and Invert"]
+
+_script_default = (
+    "dynamic_prompting",
+    "dynamic_thresholding",
+    "wildcard_recursive",
+    "wildcards",
+    "lora_block_weight",
+    "negpip",
+    "soft_inpainting",
+)
+SCRIPT_DEFAULT = ",".join(sorted(_script_default))
```

### Comparing `adetailer-24.4.1/adetailer/common.py` & `adetailer-24.4.2/adetailer/common.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,156 +1,156 @@
-from __future__ import annotations
-
-import os
-from collections import OrderedDict
-from dataclasses import dataclass, field
-from pathlib import Path
-from typing import Any, Optional
-
-from huggingface_hub import hf_hub_download
-from PIL import Image, ImageDraw
-from rich import print
-from torchvision.transforms.functional import to_pil_image
-
-REPO_ID = "Bingsu/adetailer"
-_download_failed = False
-
-
-@dataclass
-class PredictOutput:
-    bboxes: list[list[int | float]] = field(default_factory=list)
-    masks: list[Image.Image] = field(default_factory=list)
-    preview: Optional[Image.Image] = None
-
-
-def hf_download(file: str, repo_id: str = REPO_ID) -> str | None:
-    global _download_failed
-
-    if _download_failed:
-        return "INVALID"
-
-    try:
-        path = hf_hub_download(repo_id, file)
-    except Exception:
-        msg = f"[-] ADetailer: Failed to load model {file!r} from huggingface"
-        print(msg)
-        path = "INVALID"
-        _download_failed = True
-    return path
-
-
-def safe_mkdir(path: str | os.PathLike[str]) -> None:
-    path = Path(path)
-    if not path.exists() and path.parent.exists() and os.access(path.parent, os.W_OK):
-        path.mkdir()
-
-
-def scan_model_dir(path: Path) -> list[Path]:
-    if not path.is_dir():
-        return []
-    return [p for p in path.rglob("*") if p.is_file() and p.suffix == ".pt"]
-
-
-def get_models(
-    *dirs: str | os.PathLike[str], huggingface: bool = True
-) -> OrderedDict[str, str]:
-    model_paths = []
-
-    for dir_ in dirs:
-        if not dir_:
-            continue
-        model_paths.extend(scan_model_dir(Path(dir_)))
-
-    models = OrderedDict()
-    if huggingface:
-        models.update(
-            {
-                "face_yolov8n.pt": hf_download("face_yolov8n.pt"),
-                "face_yolov8s.pt": hf_download("face_yolov8s.pt"),
-                "hand_yolov8n.pt": hf_download("hand_yolov8n.pt"),
-                "person_yolov8n-seg.pt": hf_download("person_yolov8n-seg.pt"),
-                "person_yolov8s-seg.pt": hf_download("person_yolov8s-seg.pt"),
-                "yolov8x-worldv2.pt": hf_download(
-                    "yolov8x-worldv2.pt", repo_id="Bingsu/yolo-world-mirror"
-                ),
-            }
-        )
-    models.update(
-        {
-            "mediapipe_face_full": "mediapipe_face_full",
-            "mediapipe_face_short": "mediapipe_face_short",
-            "mediapipe_face_mesh": "mediapipe_face_mesh",
-            "mediapipe_face_mesh_eyes_only": "mediapipe_face_mesh_eyes_only",
-        }
-    )
-
-    invalid_keys = [k for k, v in models.items() if v == "INVALID"]
-    for key in invalid_keys:
-        models.pop(key)
-
-    for path in model_paths:
-        if path.name in models:
-            continue
-        models[path.name] = str(path)
-
-    return models
-
-
-def create_mask_from_bbox(
-    bboxes: list[list[float]], shape: tuple[int, int]
-) -> list[Image.Image]:
-    """
-    Parameters
-    ----------
-        bboxes: list[list[float]]
-            list of [x1, y1, x2, y2]
-            bounding boxes
-        shape: tuple[int, int]
-            shape of the image (width, height)
-
-    Returns
-    -------
-        masks: list[Image.Image]
-        A list of masks
-
-    """
-    masks = []
-    for bbox in bboxes:
-        mask = Image.new("L", shape, 0)
-        mask_draw = ImageDraw.Draw(mask)
-        mask_draw.rectangle(bbox, fill=255)
-        masks.append(mask)
-    return masks
-
-
-def create_bbox_from_mask(
-    masks: list[Image.Image], shape: tuple[int, int]
-) -> list[list[int]]:
-    """
-    Parameters
-    ----------
-        masks: list[Image.Image]
-            A list of masks
-        shape: tuple[int, int]
-            shape of the image (width, height)
-
-    Returns
-    -------
-        bboxes: list[list[float]]
-        A list of bounding boxes
-
-    """
-    bboxes = []
-    for mask in masks:
-        mask = mask.resize(shape)
-        bbox = mask.getbbox()
-        if bbox is not None:
-            bboxes.append(list(bbox))
-    return bboxes
-
-
-def ensure_pil_image(image: Any, mode: str = "RGB") -> Image.Image:
-    if not isinstance(image, Image.Image):
-        image = to_pil_image(image)
-    if image.mode != mode:
-        image = image.convert(mode)
-    return image
+from __future__ import annotations
+
+import os
+from collections import OrderedDict
+from dataclasses import dataclass, field
+from pathlib import Path
+from typing import Any, Optional
+
+from huggingface_hub import hf_hub_download
+from PIL import Image, ImageDraw
+from rich import print
+from torchvision.transforms.functional import to_pil_image
+
+REPO_ID = "Bingsu/adetailer"
+_download_failed = False
+
+
+@dataclass
+class PredictOutput:
+    bboxes: list[list[int | float]] = field(default_factory=list)
+    masks: list[Image.Image] = field(default_factory=list)
+    preview: Optional[Image.Image] = None
+
+
+def hf_download(file: str, repo_id: str = REPO_ID) -> str | None:
+    global _download_failed
+
+    if _download_failed:
+        return "INVALID"
+
+    try:
+        path = hf_hub_download(repo_id, file)
+    except Exception:
+        msg = f"[-] ADetailer: Failed to load model {file!r} from huggingface"
+        print(msg)
+        path = "INVALID"
+        _download_failed = True
+    return path
+
+
+def safe_mkdir(path: str | os.PathLike[str]) -> None:
+    path = Path(path)
+    if not path.exists() and path.parent.exists() and os.access(path.parent, os.W_OK):
+        path.mkdir()
+
+
+def scan_model_dir(path: Path) -> list[Path]:
+    if not path.is_dir():
+        return []
+    return [p for p in path.rglob("*") if p.is_file() and p.suffix == ".pt"]
+
+
+def get_models(
+    *dirs: str | os.PathLike[str], huggingface: bool = True
+) -> OrderedDict[str, str]:
+    model_paths = []
+
+    for dir_ in dirs:
+        if not dir_:
+            continue
+        model_paths.extend(scan_model_dir(Path(dir_)))
+
+    models = OrderedDict()
+    if huggingface:
+        models.update(
+            {
+                "face_yolov8n.pt": hf_download("face_yolov8n.pt"),
+                "face_yolov8s.pt": hf_download("face_yolov8s.pt"),
+                "hand_yolov8n.pt": hf_download("hand_yolov8n.pt"),
+                "person_yolov8n-seg.pt": hf_download("person_yolov8n-seg.pt"),
+                "person_yolov8s-seg.pt": hf_download("person_yolov8s-seg.pt"),
+                "yolov8x-worldv2.pt": hf_download(
+                    "yolov8x-worldv2.pt", repo_id="Bingsu/yolo-world-mirror"
+                ),
+            }
+        )
+    models.update(
+        {
+            "mediapipe_face_full": "mediapipe_face_full",
+            "mediapipe_face_short": "mediapipe_face_short",
+            "mediapipe_face_mesh": "mediapipe_face_mesh",
+            "mediapipe_face_mesh_eyes_only": "mediapipe_face_mesh_eyes_only",
+        }
+    )
+
+    invalid_keys = [k for k, v in models.items() if v == "INVALID"]
+    for key in invalid_keys:
+        models.pop(key)
+
+    for path in model_paths:
+        if path.name in models:
+            continue
+        models[path.name] = str(path)
+
+    return models
+
+
+def create_mask_from_bbox(
+    bboxes: list[list[float]], shape: tuple[int, int]
+) -> list[Image.Image]:
+    """
+    Parameters
+    ----------
+        bboxes: list[list[float]]
+            list of [x1, y1, x2, y2]
+            bounding boxes
+        shape: tuple[int, int]
+            shape of the image (width, height)
+
+    Returns
+    -------
+        masks: list[Image.Image]
+        A list of masks
+
+    """
+    masks = []
+    for bbox in bboxes:
+        mask = Image.new("L", shape, 0)
+        mask_draw = ImageDraw.Draw(mask)
+        mask_draw.rectangle(bbox, fill=255)
+        masks.append(mask)
+    return masks
+
+
+def create_bbox_from_mask(
+    masks: list[Image.Image], shape: tuple[int, int]
+) -> list[list[int]]:
+    """
+    Parameters
+    ----------
+        masks: list[Image.Image]
+            A list of masks
+        shape: tuple[int, int]
+            shape of the image (width, height)
+
+    Returns
+    -------
+        bboxes: list[list[float]]
+        A list of bounding boxes
+
+    """
+    bboxes = []
+    for mask in masks:
+        mask = mask.resize(shape)
+        bbox = mask.getbbox()
+        if bbox is not None:
+            bboxes.append(list(bbox))
+    return bboxes
+
+
+def ensure_pil_image(image: Any, mode: str = "RGB") -> Image.Image:
+    if not isinstance(image, Image.Image):
+        image = to_pil_image(image)
+    if image.mode != mode:
+        image = image.convert(mode)
+    return image
```

### Comparing `adetailer-24.4.1/adetailer/ui.py` & `adetailer-24.4.2/adetailer/ui.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,693 +1,693 @@
-from __future__ import annotations
-
-from dataclasses import dataclass
-from functools import partial
-from types import SimpleNamespace
-from typing import Any
-
-import gradio as gr
-
-from adetailer import AFTER_DETAILER, __version__
-from adetailer.args import ALL_ARGS, MASK_MERGE_INVERT
-from controlnet_ext import controlnet_exists, controlnet_type, get_cn_models
-
-if controlnet_type == "forge":
-    from lib_controlnet import global_state
-
-    cn_module_choices = {
-        "inpaint": list(global_state.get_filtered_preprocessors("Inpaint")),
-        "lineart": list(global_state.get_filtered_preprocessors("Lineart")),
-        "openpose": list(global_state.get_filtered_preprocessors("OpenPose")),
-        "tile": list(global_state.get_filtered_preprocessors("Tile")),
-        "scribble": list(global_state.get_filtered_preprocessors("Scribble")),
-        "depth": list(global_state.get_filtered_preprocessors("Depth")),
-    }
-else:
-    cn_module_choices = {
-        "inpaint": [
-            "inpaint_global_harmonious",
-            "inpaint_only",
-            "inpaint_only+lama",
-        ],
-        "lineart": [
-            "lineart_coarse",
-            "lineart_realistic",
-            "lineart_anime",
-            "lineart_anime_denoise",
-        ],
-        "openpose": ["openpose_full", "dw_openpose_full"],
-        "tile": ["tile_resample", "tile_colorfix", "tile_colorfix+sharp"],
-        "scribble": ["t2ia_sketch_pidi"],
-        "depth": ["depth_midas", "depth_hand_refiner"],
-    }
-
-
-class Widgets(SimpleNamespace):
-    def tolist(self):
-        return [getattr(self, attr) for attr in ALL_ARGS.attrs]
-
-
-@dataclass
-class WebuiInfo:
-    ad_model_list: list[str]
-    sampler_names: list[str]
-    scheduler_names: list[str]
-    t2i_button: gr.Button
-    i2i_button: gr.Button
-    checkpoints_list: list[str]
-    vae_list: list[str]
-
-
-def gr_interactive(value: bool = True):
-    return gr.update(interactive=value)
-
-
-def ordinal(n: int) -> str:
-    d = {1: "st", 2: "nd", 3: "rd"}
-    return str(n) + ("th" if 11 <= n % 100 <= 13 else d.get(n % 10, "th"))
-
-
-def suffix(n: int, c: str = " ") -> str:
-    return "" if n == 0 else c + ordinal(n + 1)
-
-
-def on_widget_change(state: dict, value: Any, *, attr: str):
-    if "is_api" in state:
-        state = state.copy()
-        state.pop("is_api")
-    state[attr] = value
-    return state
-
-
-def on_generate_click(state: dict, *values: Any):
-    for attr, value in zip(ALL_ARGS.attrs, values):
-        state[attr] = value
-    state["is_api"] = ()
-    return state
-
-
-def on_ad_model_update(model: str):
-    if "-world" in model:
-        return gr.update(
-            visible=True,
-            placeholder="Comma separated class names to detect, ex: 'person,cat'. default: COCO 80 classes",
-        )
-    return gr.update(visible=False, placeholder="")
-
-
-def on_cn_model_update(cn_model_name: str):
-    cn_model_name = cn_model_name.replace("inpaint_depth", "depth")
-    for t in cn_module_choices:
-        if t in cn_model_name:
-            choices = cn_module_choices[t]
-            return gr.update(visible=True, choices=choices, value=choices[0])
-    return gr.update(visible=False, choices=["None"], value="None")
-
-
-def elem_id(item_id: str, n: int, is_img2img: bool) -> str:
-    tap = "img2img" if is_img2img else "txt2img"
-    suf = suffix(n, "_")
-    return f"script_{tap}_adetailer_{item_id}{suf}"
-
-
-def state_init(w: Widgets) -> dict[str, Any]:
-    return {attr: getattr(w, attr).value for attr in ALL_ARGS.attrs}
-
-
-def adui(
-    num_models: int,
-    is_img2img: bool,
-    webui_info: WebuiInfo,
-):
-    states = []
-    infotext_fields = []
-    eid = partial(elem_id, n=0, is_img2img=is_img2img)
-
-    with gr.Accordion(AFTER_DETAILER, open=False, elem_id=eid("ad_main_accordion")):
-        with gr.Row():
-            with gr.Column(scale=6):
-                ad_enable = gr.Checkbox(
-                    label="Enable ADetailer",
-                    value=False,
-                    visible=True,
-                    elem_id=eid("ad_enable"),
-                )
-
-            with gr.Column(scale=6):
-                ad_skip_img2img = gr.Checkbox(
-                    label="Skip img2img",
-                    value=False,
-                    visible=is_img2img,
-                    elem_id=eid("ad_skip_img2img"),
-                )
-
-            with gr.Column(scale=1, min_width=180):
-                gr.Markdown(
-                    f"v{__version__}",
-                    elem_id=eid("ad_version"),
-                )
-
-        infotext_fields.append((ad_enable, "ADetailer enable"))
-        infotext_fields.append((ad_skip_img2img, "ADetailer skip img2img"))
-
-        with gr.Group(), gr.Tabs():
-            for n in range(num_models):
-                with gr.Tab(ordinal(n + 1)):
-                    state, infofields = one_ui_group(
-                        n=n,
-                        is_img2img=is_img2img,
-                        webui_info=webui_info,
-                    )
-
-                states.append(state)
-                infotext_fields.extend(infofields)
-
-    # components: [bool, dict, dict, ...]
-    components = [ad_enable, ad_skip_img2img, *states]
-    return components, infotext_fields
-
-
-def one_ui_group(n: int, is_img2img: bool, webui_info: WebuiInfo):
-    w = Widgets()
-    eid = partial(elem_id, n=n, is_img2img=is_img2img)
-
-    with gr.Group():
-        with gr.Row():
-            model_choices = (
-                [*webui_info.ad_model_list, "None"]
-                if n == 0
-                else ["None", *webui_info.ad_model_list]
-            )
-
-            w.ad_model = gr.Dropdown(
-                label="ADetailer model" + suffix(n),
-                choices=model_choices,
-                value=model_choices[0],
-                visible=True,
-                type="value",
-                elem_id=eid("ad_model"),
-            )
-
-        with gr.Row():
-            w.ad_model_classes = gr.Textbox(
-                label="ADetailer model classes" + suffix(n),
-                value="",
-                visible=False,
-                elem_id=eid("ad_classes"),
-            )
-
-            w.ad_model.change(
-                on_ad_model_update,
-                inputs=w.ad_model,
-                outputs=w.ad_model_classes,
-                queue=False,
-            )
-
-    gr.HTML("<br>")
-
-    with gr.Group():
-        with gr.Row(elem_id=eid("ad_toprow_prompt")):
-            w.ad_prompt = gr.Textbox(
-                label="ad_prompt" + suffix(n),
-                show_label=False,
-                lines=3,
-                placeholder="ADetailer prompt"
-                + suffix(n)
-                + "\nIf blank, the main prompt is used.",
-                elem_id=eid("ad_prompt"),
-            )
-
-        with gr.Row(elem_id=eid("ad_toprow_negative_prompt")):
-            w.ad_negative_prompt = gr.Textbox(
-                label="ad_negative_prompt" + suffix(n),
-                show_label=False,
-                lines=2,
-                placeholder="ADetailer negative prompt"
-                + suffix(n)
-                + "\nIf blank, the main negative prompt is used.",
-                elem_id=eid("ad_negative_prompt"),
-            )
-
-    with gr.Group():
-        with gr.Accordion(
-            "Detection", open=False, elem_id=eid("ad_detection_accordion")
-        ):
-            detection(w, n, is_img2img)
-
-        with gr.Accordion(
-            "Mask Preprocessing",
-            open=False,
-            elem_id=eid("ad_mask_preprocessing_accordion"),
-        ):
-            mask_preprocessing(w, n, is_img2img)
-
-        with gr.Accordion(
-            "Inpainting", open=False, elem_id=eid("ad_inpainting_accordion")
-        ):
-            inpainting(w, n, is_img2img, webui_info)
-
-    with gr.Group():
-        controlnet(w, n, is_img2img)
-
-    state = gr.State(lambda: state_init(w))
-
-    for attr in ALL_ARGS.attrs:
-        widget = getattr(w, attr)
-        on_change = partial(on_widget_change, attr=attr)
-        widget.change(fn=on_change, inputs=[state, widget], outputs=state, queue=False)
-
-    all_inputs = [state, *w.tolist()]
-    target_button = webui_info.i2i_button if is_img2img else webui_info.t2i_button
-    target_button.click(
-        fn=on_generate_click, inputs=all_inputs, outputs=state, queue=False
-    )
-
-    infotext_fields = [(getattr(w, attr), name + suffix(n)) for attr, name in ALL_ARGS]
-
-    return state, infotext_fields
-
-
-def detection(w: Widgets, n: int, is_img2img: bool):
-    eid = partial(elem_id, n=n, is_img2img=is_img2img)
-
-    with gr.Row():
-        with gr.Column(variant="compact"):
-            w.ad_confidence = gr.Slider(
-                label="Detection model confidence threshold" + suffix(n),
-                minimum=0.0,
-                maximum=1.0,
-                step=0.01,
-                value=0.3,
-                visible=True,
-                elem_id=eid("ad_confidence"),
-            )
-            w.ad_mask_k_largest = gr.Slider(
-                label="Mask only the top k largest (0 to disable)" + suffix(n),
-                minimum=0,
-                maximum=10,
-                step=1,
-                value=0,
-                visible=True,
-                elem_id=eid("ad_mask_k_largest"),
-            )
-
-        with gr.Column(variant="compact"):
-            w.ad_mask_min_ratio = gr.Slider(
-                label="Mask min area ratio" + suffix(n),
-                minimum=0.0,
-                maximum=1.0,
-                step=0.001,
-                value=0.0,
-                visible=True,
-                elem_id=eid("ad_mask_min_ratio"),
-            )
-            w.ad_mask_max_ratio = gr.Slider(
-                label="Mask max area ratio" + suffix(n),
-                minimum=0.0,
-                maximum=1.0,
-                step=0.001,
-                value=1.0,
-                visible=True,
-                elem_id=eid("ad_mask_max_ratio"),
-            )
-
-
-def mask_preprocessing(w: Widgets, n: int, is_img2img: bool):
-    eid = partial(elem_id, n=n, is_img2img=is_img2img)
-
-    with gr.Group():
-        with gr.Row():
-            with gr.Column(variant="compact"):
-                w.ad_x_offset = gr.Slider(
-                    label="Mask x(→) offset" + suffix(n),
-                    minimum=-200,
-                    maximum=200,
-                    step=1,
-                    value=0,
-                    visible=True,
-                    elem_id=eid("ad_x_offset"),
-                )
-                w.ad_y_offset = gr.Slider(
-                    label="Mask y(↑) offset" + suffix(n),
-                    minimum=-200,
-                    maximum=200,
-                    step=1,
-                    value=0,
-                    visible=True,
-                    elem_id=eid("ad_y_offset"),
-                )
-
-            with gr.Column(variant="compact"):
-                w.ad_dilate_erode = gr.Slider(
-                    label="Mask erosion (-) / dilation (+)" + suffix(n),
-                    minimum=-128,
-                    maximum=128,
-                    step=4,
-                    value=4,
-                    visible=True,
-                    elem_id=eid("ad_dilate_erode"),
-                )
-
-        with gr.Row():
-            w.ad_mask_merge_invert = gr.Radio(
-                label="Mask merge mode" + suffix(n),
-                choices=MASK_MERGE_INVERT,
-                value="None",
-                elem_id=eid("ad_mask_merge_invert"),
-            )
-
-
-def inpainting(w: Widgets, n: int, is_img2img: bool, webui_info: WebuiInfo):
-    eid = partial(elem_id, n=n, is_img2img=is_img2img)
-
-    with gr.Group():
-        with gr.Row():
-            w.ad_mask_blur = gr.Slider(
-                label="Inpaint mask blur" + suffix(n),
-                minimum=0,
-                maximum=64,
-                step=1,
-                value=4,
-                visible=True,
-                elem_id=eid("ad_mask_blur"),
-            )
-
-            w.ad_denoising_strength = gr.Slider(
-                label="Inpaint denoising strength" + suffix(n),
-                minimum=0.0,
-                maximum=1.0,
-                step=0.01,
-                value=0.4,
-                visible=True,
-                elem_id=eid("ad_denoising_strength"),
-            )
-
-        with gr.Row():
-            with gr.Column(variant="compact"):
-                w.ad_inpaint_only_masked = gr.Checkbox(
-                    label="Inpaint only masked" + suffix(n),
-                    value=True,
-                    visible=True,
-                    elem_id=eid("ad_inpaint_only_masked"),
-                )
-                w.ad_inpaint_only_masked_padding = gr.Slider(
-                    label="Inpaint only masked padding, pixels" + suffix(n),
-                    minimum=0,
-                    maximum=256,
-                    step=4,
-                    value=32,
-                    visible=True,
-                    elem_id=eid("ad_inpaint_only_masked_padding"),
-                )
-
-                w.ad_inpaint_only_masked.change(
-                    gr_interactive,
-                    inputs=w.ad_inpaint_only_masked,
-                    outputs=w.ad_inpaint_only_masked_padding,
-                    queue=False,
-                )
-
-            with gr.Column(variant="compact"):
-                w.ad_use_inpaint_width_height = gr.Checkbox(
-                    label="Use separate width/height" + suffix(n),
-                    value=False,
-                    visible=True,
-                    elem_id=eid("ad_use_inpaint_width_height"),
-                )
-
-                w.ad_inpaint_width = gr.Slider(
-                    label="inpaint width" + suffix(n),
-                    minimum=64,
-                    maximum=2048,
-                    step=4,
-                    value=512,
-                    visible=True,
-                    elem_id=eid("ad_inpaint_width"),
-                )
-
-                w.ad_inpaint_height = gr.Slider(
-                    label="inpaint height" + suffix(n),
-                    minimum=64,
-                    maximum=2048,
-                    step=4,
-                    value=512,
-                    visible=True,
-                    elem_id=eid("ad_inpaint_height"),
-                )
-
-                w.ad_use_inpaint_width_height.change(
-                    lambda value: (gr_interactive(value), gr_interactive(value)),
-                    inputs=w.ad_use_inpaint_width_height,
-                    outputs=[w.ad_inpaint_width, w.ad_inpaint_height],
-                    queue=False,
-                )
-
-        with gr.Row():
-            with gr.Column(variant="compact"):
-                w.ad_use_steps = gr.Checkbox(
-                    label="Use separate steps" + suffix(n),
-                    value=False,
-                    visible=True,
-                    elem_id=eid("ad_use_steps"),
-                )
-
-                w.ad_steps = gr.Slider(
-                    label="ADetailer steps" + suffix(n),
-                    minimum=1,
-                    maximum=150,
-                    step=1,
-                    value=28,
-                    visible=True,
-                    elem_id=eid("ad_steps"),
-                )
-
-                w.ad_use_steps.change(
-                    gr_interactive,
-                    inputs=w.ad_use_steps,
-                    outputs=w.ad_steps,
-                    queue=False,
-                )
-
-            with gr.Column(variant="compact"):
-                w.ad_use_cfg_scale = gr.Checkbox(
-                    label="Use separate CFG scale" + suffix(n),
-                    value=False,
-                    visible=True,
-                    elem_id=eid("ad_use_cfg_scale"),
-                )
-
-                w.ad_cfg_scale = gr.Slider(
-                    label="ADetailer CFG scale" + suffix(n),
-                    minimum=0.0,
-                    maximum=30.0,
-                    step=0.5,
-                    value=7.0,
-                    visible=True,
-                    elem_id=eid("ad_cfg_scale"),
-                )
-
-                w.ad_use_cfg_scale.change(
-                    gr_interactive,
-                    inputs=w.ad_use_cfg_scale,
-                    outputs=w.ad_cfg_scale,
-                    queue=False,
-                )
-
-        with gr.Row():
-            with gr.Column(variant="compact"):
-                w.ad_use_checkpoint = gr.Checkbox(
-                    label="Use separate checkpoint" + suffix(n),
-                    value=False,
-                    visible=True,
-                    elem_id=eid("ad_use_checkpoint"),
-                )
-
-                ckpts = ["Use same checkpoint", *webui_info.checkpoints_list]
-
-                w.ad_checkpoint = gr.Dropdown(
-                    label="ADetailer checkpoint" + suffix(n),
-                    choices=ckpts,
-                    value=ckpts[0],
-                    visible=True,
-                    elem_id=eid("ad_checkpoint"),
-                )
-
-            with gr.Column(variant="compact"):
-                w.ad_use_vae = gr.Checkbox(
-                    label="Use separate VAE" + suffix(n),
-                    value=False,
-                    visible=True,
-                    elem_id=eid("ad_use_vae"),
-                )
-
-                vaes = ["Use same VAE", *webui_info.vae_list]
-
-                w.ad_vae = gr.Dropdown(
-                    label="ADetailer VAE" + suffix(n),
-                    choices=vaes,
-                    value=vaes[0],
-                    visible=True,
-                    elem_id=eid("ad_vae"),
-                )
-
-        with gr.Row(), gr.Column(variant="compact"):
-            w.ad_use_sampler = gr.Checkbox(
-                label="Use separate sampler" + suffix(n),
-                value=False,
-                visible=True,
-                elem_id=eid("ad_use_sampler"),
-            )
-
-            with gr.Row():
-                w.ad_sampler = gr.Dropdown(
-                    label="ADetailer sampler" + suffix(n),
-                    choices=webui_info.sampler_names,
-                    value=webui_info.sampler_names[0],
-                    visible=True,
-                    elem_id=eid("ad_sampler"),
-                )
-
-                scheduler_names = [
-                    "Use same scheduler",
-                    *webui_info.scheduler_names,
-                ]
-                w.ad_scheduler = gr.Dropdown(
-                    label="ADetailer scheduler" + suffix(n),
-                    choices=scheduler_names,
-                    value=scheduler_names[0],
-                    visible=len(scheduler_names) > 1,
-                    elem_id=eid("ad_scheduler"),
-                )
-
-                w.ad_use_sampler.change(
-                    lambda value: (gr_interactive(value), gr_interactive(value)),
-                    inputs=w.ad_use_sampler,
-                    outputs=[w.ad_sampler, w.ad_scheduler],
-                    queue=False,
-                )
-
-        with gr.Row():
-            with gr.Column(variant="compact"):
-                w.ad_use_noise_multiplier = gr.Checkbox(
-                    label="Use separate noise multiplier" + suffix(n),
-                    value=False,
-                    visible=True,
-                    elem_id=eid("ad_use_noise_multiplier"),
-                )
-
-                w.ad_noise_multiplier = gr.Slider(
-                    label="Noise multiplier for img2img" + suffix(n),
-                    minimum=0.5,
-                    maximum=1.5,
-                    step=0.01,
-                    value=1.0,
-                    visible=True,
-                    elem_id=eid("ad_noise_multiplier"),
-                )
-
-                w.ad_use_noise_multiplier.change(
-                    gr_interactive,
-                    inputs=w.ad_use_noise_multiplier,
-                    outputs=w.ad_noise_multiplier,
-                    queue=False,
-                )
-
-            with gr.Column(variant="compact"):
-                w.ad_use_clip_skip = gr.Checkbox(
-                    label="Use separate CLIP skip" + suffix(n),
-                    value=False,
-                    visible=True,
-                    elem_id=eid("ad_use_clip_skip"),
-                )
-
-                w.ad_clip_skip = gr.Slider(
-                    label="ADetailer CLIP skip" + suffix(n),
-                    minimum=1,
-                    maximum=12,
-                    step=1,
-                    value=1,
-                    visible=True,
-                    elem_id=eid("ad_clip_skip"),
-                )
-
-                w.ad_use_clip_skip.change(
-                    gr_interactive,
-                    inputs=w.ad_use_clip_skip,
-                    outputs=w.ad_clip_skip,
-                    queue=False,
-                )
-
-        with gr.Row(), gr.Column(variant="compact"):
-            w.ad_restore_face = gr.Checkbox(
-                label="Restore faces after ADetailer" + suffix(n),
-                value=False,
-                elem_id=eid("ad_restore_face"),
-            )
-
-
-def controlnet(w: Widgets, n: int, is_img2img: bool):
-    eid = partial(elem_id, n=n, is_img2img=is_img2img)
-    cn_models = ["None", "Passthrough", *get_cn_models()]
-
-    with gr.Row(variant="panel"):
-        with gr.Column(variant="compact"):
-            w.ad_controlnet_model = gr.Dropdown(
-                label="ControlNet model" + suffix(n),
-                choices=cn_models,
-                value="None",
-                visible=True,
-                type="value",
-                interactive=controlnet_exists,
-                elem_id=eid("ad_controlnet_model"),
-            )
-
-            w.ad_controlnet_module = gr.Dropdown(
-                label="ControlNet module" + suffix(n),
-                choices=["None"],
-                value="None",
-                visible=False,
-                type="value",
-                interactive=controlnet_exists,
-                elem_id=eid("ad_controlnet_module"),
-            )
-
-            w.ad_controlnet_weight = gr.Slider(
-                label="ControlNet weight" + suffix(n),
-                minimum=0.0,
-                maximum=1.0,
-                step=0.01,
-                value=1.0,
-                visible=True,
-                interactive=controlnet_exists,
-                elem_id=eid("ad_controlnet_weight"),
-            )
-
-            w.ad_controlnet_model.change(
-                on_cn_model_update,
-                inputs=w.ad_controlnet_model,
-                outputs=w.ad_controlnet_module,
-                queue=False,
-            )
-
-        with gr.Column(variant="compact"):
-            w.ad_controlnet_guidance_start = gr.Slider(
-                label="ControlNet guidance start" + suffix(n),
-                minimum=0.0,
-                maximum=1.0,
-                step=0.01,
-                value=0.0,
-                visible=True,
-                interactive=controlnet_exists,
-                elem_id=eid("ad_controlnet_guidance_start"),
-            )
-
-            w.ad_controlnet_guidance_end = gr.Slider(
-                label="ControlNet guidance end" + suffix(n),
-                minimum=0.0,
-                maximum=1.0,
-                step=0.01,
-                value=1.0,
-                visible=True,
-                interactive=controlnet_exists,
-                elem_id=eid("ad_controlnet_guidance_end"),
-            )
+from __future__ import annotations
+
+from dataclasses import dataclass
+from functools import partial
+from types import SimpleNamespace
+from typing import Any
+
+import gradio as gr
+
+from adetailer import AFTER_DETAILER, __version__
+from adetailer.args import ALL_ARGS, MASK_MERGE_INVERT
+from controlnet_ext import controlnet_exists, controlnet_type, get_cn_models
+
+if controlnet_type == "forge":
+    from lib_controlnet import global_state
+
+    cn_module_choices = {
+        "inpaint": list(global_state.get_filtered_preprocessors("Inpaint")),
+        "lineart": list(global_state.get_filtered_preprocessors("Lineart")),
+        "openpose": list(global_state.get_filtered_preprocessors("OpenPose")),
+        "tile": list(global_state.get_filtered_preprocessors("Tile")),
+        "scribble": list(global_state.get_filtered_preprocessors("Scribble")),
+        "depth": list(global_state.get_filtered_preprocessors("Depth")),
+    }
+else:
+    cn_module_choices = {
+        "inpaint": [
+            "inpaint_global_harmonious",
+            "inpaint_only",
+            "inpaint_only+lama",
+        ],
+        "lineart": [
+            "lineart_coarse",
+            "lineart_realistic",
+            "lineart_anime",
+            "lineart_anime_denoise",
+        ],
+        "openpose": ["openpose_full", "dw_openpose_full"],
+        "tile": ["tile_resample", "tile_colorfix", "tile_colorfix+sharp"],
+        "scribble": ["t2ia_sketch_pidi"],
+        "depth": ["depth_midas", "depth_hand_refiner"],
+    }
+
+
+class Widgets(SimpleNamespace):
+    def tolist(self):
+        return [getattr(self, attr) for attr in ALL_ARGS.attrs]
+
+
+@dataclass
+class WebuiInfo:
+    ad_model_list: list[str]
+    sampler_names: list[str]
+    scheduler_names: list[str]
+    t2i_button: gr.Button
+    i2i_button: gr.Button
+    checkpoints_list: list[str]
+    vae_list: list[str]
+
+
+def gr_interactive(value: bool = True):
+    return gr.update(interactive=value)
+
+
+def ordinal(n: int) -> str:
+    d = {1: "st", 2: "nd", 3: "rd"}
+    return str(n) + ("th" if 11 <= n % 100 <= 13 else d.get(n % 10, "th"))
+
+
+def suffix(n: int, c: str = " ") -> str:
+    return "" if n == 0 else c + ordinal(n + 1)
+
+
+def on_widget_change(state: dict, value: Any, *, attr: str):
+    if "is_api" in state:
+        state = state.copy()
+        state.pop("is_api")
+    state[attr] = value
+    return state
+
+
+def on_generate_click(state: dict, *values: Any):
+    for attr, value in zip(ALL_ARGS.attrs, values):
+        state[attr] = value
+    state["is_api"] = ()
+    return state
+
+
+def on_ad_model_update(model: str):
+    if "-world" in model:
+        return gr.update(
+            visible=True,
+            placeholder="Comma separated class names to detect, ex: 'person,cat'. default: COCO 80 classes",
+        )
+    return gr.update(visible=False, placeholder="")
+
+
+def on_cn_model_update(cn_model_name: str):
+    cn_model_name = cn_model_name.replace("inpaint_depth", "depth")
+    for t in cn_module_choices:
+        if t in cn_model_name:
+            choices = cn_module_choices[t]
+            return gr.update(visible=True, choices=choices, value=choices[0])
+    return gr.update(visible=False, choices=["None"], value="None")
+
+
+def elem_id(item_id: str, n: int, is_img2img: bool) -> str:
+    tap = "img2img" if is_img2img else "txt2img"
+    suf = suffix(n, "_")
+    return f"script_{tap}_adetailer_{item_id}{suf}"
+
+
+def state_init(w: Widgets) -> dict[str, Any]:
+    return {attr: getattr(w, attr).value for attr in ALL_ARGS.attrs}
+
+
+def adui(
+    num_models: int,
+    is_img2img: bool,
+    webui_info: WebuiInfo,
+):
+    states = []
+    infotext_fields = []
+    eid = partial(elem_id, n=0, is_img2img=is_img2img)
+
+    with gr.Accordion(AFTER_DETAILER, open=False, elem_id=eid("ad_main_accordion")):
+        with gr.Row():
+            with gr.Column(scale=6):
+                ad_enable = gr.Checkbox(
+                    label="Enable ADetailer",
+                    value=False,
+                    visible=True,
+                    elem_id=eid("ad_enable"),
+                )
+
+            with gr.Column(scale=6):
+                ad_skip_img2img = gr.Checkbox(
+                    label="Skip img2img",
+                    value=False,
+                    visible=is_img2img,
+                    elem_id=eid("ad_skip_img2img"),
+                )
+
+            with gr.Column(scale=1, min_width=180):
+                gr.Markdown(
+                    f"v{__version__}",
+                    elem_id=eid("ad_version"),
+                )
+
+        infotext_fields.append((ad_enable, "ADetailer enable"))
+        infotext_fields.append((ad_skip_img2img, "ADetailer skip img2img"))
+
+        with gr.Group(), gr.Tabs():
+            for n in range(num_models):
+                with gr.Tab(ordinal(n + 1)):
+                    state, infofields = one_ui_group(
+                        n=n,
+                        is_img2img=is_img2img,
+                        webui_info=webui_info,
+                    )
+
+                states.append(state)
+                infotext_fields.extend(infofields)
+
+    # components: [bool, dict, dict, ...]
+    components = [ad_enable, ad_skip_img2img, *states]
+    return components, infotext_fields
+
+
+def one_ui_group(n: int, is_img2img: bool, webui_info: WebuiInfo):
+    w = Widgets()
+    eid = partial(elem_id, n=n, is_img2img=is_img2img)
+
+    with gr.Group():
+        with gr.Row():
+            model_choices = (
+                [*webui_info.ad_model_list, "None"]
+                if n == 0
+                else ["None", *webui_info.ad_model_list]
+            )
+
+            w.ad_model = gr.Dropdown(
+                label="ADetailer model" + suffix(n),
+                choices=model_choices,
+                value=model_choices[0],
+                visible=True,
+                type="value",
+                elem_id=eid("ad_model"),
+            )
+
+        with gr.Row():
+            w.ad_model_classes = gr.Textbox(
+                label="ADetailer model classes" + suffix(n),
+                value="",
+                visible=False,
+                elem_id=eid("ad_classes"),
+            )
+
+            w.ad_model.change(
+                on_ad_model_update,
+                inputs=w.ad_model,
+                outputs=w.ad_model_classes,
+                queue=False,
+            )
+
+    gr.HTML("<br>")
+
+    with gr.Group():
+        with gr.Row(elem_id=eid("ad_toprow_prompt")):
+            w.ad_prompt = gr.Textbox(
+                label="ad_prompt" + suffix(n),
+                show_label=False,
+                lines=3,
+                placeholder="ADetailer prompt"
+                + suffix(n)
+                + "\nIf blank, the main prompt is used.",
+                elem_id=eid("ad_prompt"),
+            )
+
+        with gr.Row(elem_id=eid("ad_toprow_negative_prompt")):
+            w.ad_negative_prompt = gr.Textbox(
+                label="ad_negative_prompt" + suffix(n),
+                show_label=False,
+                lines=2,
+                placeholder="ADetailer negative prompt"
+                + suffix(n)
+                + "\nIf blank, the main negative prompt is used.",
+                elem_id=eid("ad_negative_prompt"),
+            )
+
+    with gr.Group():
+        with gr.Accordion(
+            "Detection", open=False, elem_id=eid("ad_detection_accordion")
+        ):
+            detection(w, n, is_img2img)
+
+        with gr.Accordion(
+            "Mask Preprocessing",
+            open=False,
+            elem_id=eid("ad_mask_preprocessing_accordion"),
+        ):
+            mask_preprocessing(w, n, is_img2img)
+
+        with gr.Accordion(
+            "Inpainting", open=False, elem_id=eid("ad_inpainting_accordion")
+        ):
+            inpainting(w, n, is_img2img, webui_info)
+
+    with gr.Group():
+        controlnet(w, n, is_img2img)
+
+    state = gr.State(lambda: state_init(w))
+
+    for attr in ALL_ARGS.attrs:
+        widget = getattr(w, attr)
+        on_change = partial(on_widget_change, attr=attr)
+        widget.change(fn=on_change, inputs=[state, widget], outputs=state, queue=False)
+
+    all_inputs = [state, *w.tolist()]
+    target_button = webui_info.i2i_button if is_img2img else webui_info.t2i_button
+    target_button.click(
+        fn=on_generate_click, inputs=all_inputs, outputs=state, queue=False
+    )
+
+    infotext_fields = [(getattr(w, attr), name + suffix(n)) for attr, name in ALL_ARGS]
+
+    return state, infotext_fields
+
+
+def detection(w: Widgets, n: int, is_img2img: bool):
+    eid = partial(elem_id, n=n, is_img2img=is_img2img)
+
+    with gr.Row():
+        with gr.Column(variant="compact"):
+            w.ad_confidence = gr.Slider(
+                label="Detection model confidence threshold" + suffix(n),
+                minimum=0.0,
+                maximum=1.0,
+                step=0.01,
+                value=0.3,
+                visible=True,
+                elem_id=eid("ad_confidence"),
+            )
+            w.ad_mask_k_largest = gr.Slider(
+                label="Mask only the top k largest (0 to disable)" + suffix(n),
+                minimum=0,
+                maximum=10,
+                step=1,
+                value=0,
+                visible=True,
+                elem_id=eid("ad_mask_k_largest"),
+            )
+
+        with gr.Column(variant="compact"):
+            w.ad_mask_min_ratio = gr.Slider(
+                label="Mask min area ratio" + suffix(n),
+                minimum=0.0,
+                maximum=1.0,
+                step=0.001,
+                value=0.0,
+                visible=True,
+                elem_id=eid("ad_mask_min_ratio"),
+            )
+            w.ad_mask_max_ratio = gr.Slider(
+                label="Mask max area ratio" + suffix(n),
+                minimum=0.0,
+                maximum=1.0,
+                step=0.001,
+                value=1.0,
+                visible=True,
+                elem_id=eid("ad_mask_max_ratio"),
+            )
+
+
+def mask_preprocessing(w: Widgets, n: int, is_img2img: bool):
+    eid = partial(elem_id, n=n, is_img2img=is_img2img)
+
+    with gr.Group():
+        with gr.Row():
+            with gr.Column(variant="compact"):
+                w.ad_x_offset = gr.Slider(
+                    label="Mask x(→) offset" + suffix(n),
+                    minimum=-200,
+                    maximum=200,
+                    step=1,
+                    value=0,
+                    visible=True,
+                    elem_id=eid("ad_x_offset"),
+                )
+                w.ad_y_offset = gr.Slider(
+                    label="Mask y(↑) offset" + suffix(n),
+                    minimum=-200,
+                    maximum=200,
+                    step=1,
+                    value=0,
+                    visible=True,
+                    elem_id=eid("ad_y_offset"),
+                )
+
+            with gr.Column(variant="compact"):
+                w.ad_dilate_erode = gr.Slider(
+                    label="Mask erosion (-) / dilation (+)" + suffix(n),
+                    minimum=-128,
+                    maximum=128,
+                    step=4,
+                    value=4,
+                    visible=True,
+                    elem_id=eid("ad_dilate_erode"),
+                )
+
+        with gr.Row():
+            w.ad_mask_merge_invert = gr.Radio(
+                label="Mask merge mode" + suffix(n),
+                choices=MASK_MERGE_INVERT,
+                value="None",
+                elem_id=eid("ad_mask_merge_invert"),
+            )
+
+
+def inpainting(w: Widgets, n: int, is_img2img: bool, webui_info: WebuiInfo):
+    eid = partial(elem_id, n=n, is_img2img=is_img2img)
+
+    with gr.Group():
+        with gr.Row():
+            w.ad_mask_blur = gr.Slider(
+                label="Inpaint mask blur" + suffix(n),
+                minimum=0,
+                maximum=64,
+                step=1,
+                value=4,
+                visible=True,
+                elem_id=eid("ad_mask_blur"),
+            )
+
+            w.ad_denoising_strength = gr.Slider(
+                label="Inpaint denoising strength" + suffix(n),
+                minimum=0.0,
+                maximum=1.0,
+                step=0.01,
+                value=0.4,
+                visible=True,
+                elem_id=eid("ad_denoising_strength"),
+            )
+
+        with gr.Row():
+            with gr.Column(variant="compact"):
+                w.ad_inpaint_only_masked = gr.Checkbox(
+                    label="Inpaint only masked" + suffix(n),
+                    value=True,
+                    visible=True,
+                    elem_id=eid("ad_inpaint_only_masked"),
+                )
+                w.ad_inpaint_only_masked_padding = gr.Slider(
+                    label="Inpaint only masked padding, pixels" + suffix(n),
+                    minimum=0,
+                    maximum=256,
+                    step=4,
+                    value=32,
+                    visible=True,
+                    elem_id=eid("ad_inpaint_only_masked_padding"),
+                )
+
+                w.ad_inpaint_only_masked.change(
+                    gr_interactive,
+                    inputs=w.ad_inpaint_only_masked,
+                    outputs=w.ad_inpaint_only_masked_padding,
+                    queue=False,
+                )
+
+            with gr.Column(variant="compact"):
+                w.ad_use_inpaint_width_height = gr.Checkbox(
+                    label="Use separate width/height" + suffix(n),
+                    value=False,
+                    visible=True,
+                    elem_id=eid("ad_use_inpaint_width_height"),
+                )
+
+                w.ad_inpaint_width = gr.Slider(
+                    label="inpaint width" + suffix(n),
+                    minimum=64,
+                    maximum=2048,
+                    step=4,
+                    value=512,
+                    visible=True,
+                    elem_id=eid("ad_inpaint_width"),
+                )
+
+                w.ad_inpaint_height = gr.Slider(
+                    label="inpaint height" + suffix(n),
+                    minimum=64,
+                    maximum=2048,
+                    step=4,
+                    value=512,
+                    visible=True,
+                    elem_id=eid("ad_inpaint_height"),
+                )
+
+                w.ad_use_inpaint_width_height.change(
+                    lambda value: (gr_interactive(value), gr_interactive(value)),
+                    inputs=w.ad_use_inpaint_width_height,
+                    outputs=[w.ad_inpaint_width, w.ad_inpaint_height],
+                    queue=False,
+                )
+
+        with gr.Row():
+            with gr.Column(variant="compact"):
+                w.ad_use_steps = gr.Checkbox(
+                    label="Use separate steps" + suffix(n),
+                    value=False,
+                    visible=True,
+                    elem_id=eid("ad_use_steps"),
+                )
+
+                w.ad_steps = gr.Slider(
+                    label="ADetailer steps" + suffix(n),
+                    minimum=1,
+                    maximum=150,
+                    step=1,
+                    value=28,
+                    visible=True,
+                    elem_id=eid("ad_steps"),
+                )
+
+                w.ad_use_steps.change(
+                    gr_interactive,
+                    inputs=w.ad_use_steps,
+                    outputs=w.ad_steps,
+                    queue=False,
+                )
+
+            with gr.Column(variant="compact"):
+                w.ad_use_cfg_scale = gr.Checkbox(
+                    label="Use separate CFG scale" + suffix(n),
+                    value=False,
+                    visible=True,
+                    elem_id=eid("ad_use_cfg_scale"),
+                )
+
+                w.ad_cfg_scale = gr.Slider(
+                    label="ADetailer CFG scale" + suffix(n),
+                    minimum=0.0,
+                    maximum=30.0,
+                    step=0.5,
+                    value=7.0,
+                    visible=True,
+                    elem_id=eid("ad_cfg_scale"),
+                )
+
+                w.ad_use_cfg_scale.change(
+                    gr_interactive,
+                    inputs=w.ad_use_cfg_scale,
+                    outputs=w.ad_cfg_scale,
+                    queue=False,
+                )
+
+        with gr.Row():
+            with gr.Column(variant="compact"):
+                w.ad_use_checkpoint = gr.Checkbox(
+                    label="Use separate checkpoint" + suffix(n),
+                    value=False,
+                    visible=True,
+                    elem_id=eid("ad_use_checkpoint"),
+                )
+
+                ckpts = ["Use same checkpoint", *webui_info.checkpoints_list]
+
+                w.ad_checkpoint = gr.Dropdown(
+                    label="ADetailer checkpoint" + suffix(n),
+                    choices=ckpts,
+                    value=ckpts[0],
+                    visible=True,
+                    elem_id=eid("ad_checkpoint"),
+                )
+
+            with gr.Column(variant="compact"):
+                w.ad_use_vae = gr.Checkbox(
+                    label="Use separate VAE" + suffix(n),
+                    value=False,
+                    visible=True,
+                    elem_id=eid("ad_use_vae"),
+                )
+
+                vaes = ["Use same VAE", *webui_info.vae_list]
+
+                w.ad_vae = gr.Dropdown(
+                    label="ADetailer VAE" + suffix(n),
+                    choices=vaes,
+                    value=vaes[0],
+                    visible=True,
+                    elem_id=eid("ad_vae"),
+                )
+
+        with gr.Row(), gr.Column(variant="compact"):
+            w.ad_use_sampler = gr.Checkbox(
+                label="Use separate sampler" + suffix(n),
+                value=False,
+                visible=True,
+                elem_id=eid("ad_use_sampler"),
+            )
+
+            with gr.Row():
+                w.ad_sampler = gr.Dropdown(
+                    label="ADetailer sampler" + suffix(n),
+                    choices=webui_info.sampler_names,
+                    value=webui_info.sampler_names[0],
+                    visible=True,
+                    elem_id=eid("ad_sampler"),
+                )
+
+                scheduler_names = [
+                    "Use same scheduler",
+                    *webui_info.scheduler_names,
+                ]
+                w.ad_scheduler = gr.Dropdown(
+                    label="ADetailer scheduler" + suffix(n),
+                    choices=scheduler_names,
+                    value=scheduler_names[0],
+                    visible=len(scheduler_names) > 1,
+                    elem_id=eid("ad_scheduler"),
+                )
+
+                w.ad_use_sampler.change(
+                    lambda value: (gr_interactive(value), gr_interactive(value)),
+                    inputs=w.ad_use_sampler,
+                    outputs=[w.ad_sampler, w.ad_scheduler],
+                    queue=False,
+                )
+
+        with gr.Row():
+            with gr.Column(variant="compact"):
+                w.ad_use_noise_multiplier = gr.Checkbox(
+                    label="Use separate noise multiplier" + suffix(n),
+                    value=False,
+                    visible=True,
+                    elem_id=eid("ad_use_noise_multiplier"),
+                )
+
+                w.ad_noise_multiplier = gr.Slider(
+                    label="Noise multiplier for img2img" + suffix(n),
+                    minimum=0.5,
+                    maximum=1.5,
+                    step=0.01,
+                    value=1.0,
+                    visible=True,
+                    elem_id=eid("ad_noise_multiplier"),
+                )
+
+                w.ad_use_noise_multiplier.change(
+                    gr_interactive,
+                    inputs=w.ad_use_noise_multiplier,
+                    outputs=w.ad_noise_multiplier,
+                    queue=False,
+                )
+
+            with gr.Column(variant="compact"):
+                w.ad_use_clip_skip = gr.Checkbox(
+                    label="Use separate CLIP skip" + suffix(n),
+                    value=False,
+                    visible=True,
+                    elem_id=eid("ad_use_clip_skip"),
+                )
+
+                w.ad_clip_skip = gr.Slider(
+                    label="ADetailer CLIP skip" + suffix(n),
+                    minimum=1,
+                    maximum=12,
+                    step=1,
+                    value=1,
+                    visible=True,
+                    elem_id=eid("ad_clip_skip"),
+                )
+
+                w.ad_use_clip_skip.change(
+                    gr_interactive,
+                    inputs=w.ad_use_clip_skip,
+                    outputs=w.ad_clip_skip,
+                    queue=False,
+                )
+
+        with gr.Row(), gr.Column(variant="compact"):
+            w.ad_restore_face = gr.Checkbox(
+                label="Restore faces after ADetailer" + suffix(n),
+                value=False,
+                elem_id=eid("ad_restore_face"),
+            )
+
+
+def controlnet(w: Widgets, n: int, is_img2img: bool):
+    eid = partial(elem_id, n=n, is_img2img=is_img2img)
+    cn_models = ["None", "Passthrough", *get_cn_models()]
+
+    with gr.Row(variant="panel"):
+        with gr.Column(variant="compact"):
+            w.ad_controlnet_model = gr.Dropdown(
+                label="ControlNet model" + suffix(n),
+                choices=cn_models,
+                value="None",
+                visible=True,
+                type="value",
+                interactive=controlnet_exists,
+                elem_id=eid("ad_controlnet_model"),
+            )
+
+            w.ad_controlnet_module = gr.Dropdown(
+                label="ControlNet module" + suffix(n),
+                choices=["None"],
+                value="None",
+                visible=False,
+                type="value",
+                interactive=controlnet_exists,
+                elem_id=eid("ad_controlnet_module"),
+            )
+
+            w.ad_controlnet_weight = gr.Slider(
+                label="ControlNet weight" + suffix(n),
+                minimum=0.0,
+                maximum=1.0,
+                step=0.01,
+                value=1.0,
+                visible=True,
+                interactive=controlnet_exists,
+                elem_id=eid("ad_controlnet_weight"),
+            )
+
+            w.ad_controlnet_model.change(
+                on_cn_model_update,
+                inputs=w.ad_controlnet_model,
+                outputs=w.ad_controlnet_module,
+                queue=False,
+            )
+
+        with gr.Column(variant="compact"):
+            w.ad_controlnet_guidance_start = gr.Slider(
+                label="ControlNet guidance start" + suffix(n),
+                minimum=0.0,
+                maximum=1.0,
+                step=0.01,
+                value=0.0,
+                visible=True,
+                interactive=controlnet_exists,
+                elem_id=eid("ad_controlnet_guidance_start"),
+            )
+
+            w.ad_controlnet_guidance_end = gr.Slider(
+                label="ControlNet guidance end" + suffix(n),
+                minimum=0.0,
+                maximum=1.0,
+                step=0.01,
+                value=1.0,
+                visible=True,
+                interactive=controlnet_exists,
+                elem_id=eid("ad_controlnet_guidance_end"),
+            )
```

### Comparing `adetailer-24.4.1/adetailer/ultralytics.py` & `adetailer-24.4.2/adetailer/ultralytics.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-from __future__ import annotations
-
-from pathlib import Path
-from typing import TYPE_CHECKING
-
-import cv2
-from PIL import Image
-from torchvision.transforms.functional import to_pil_image
-
-from adetailer import PredictOutput
-from adetailer.common import create_mask_from_bbox
-
-if TYPE_CHECKING:
-    import torch
-    from ultralytics import YOLO, YOLOWorld
-
-
-def ultralytics_predict(
-    model_path: str | Path,
-    image: Image.Image,
-    confidence: float = 0.3,
-    device: str = "",
-    classes: str = "",
-) -> PredictOutput:
-    from ultralytics import YOLO
-
-    model = YOLO(model_path)
-    apply_classes(model, model_path, classes)
-    pred = model(image, conf=confidence, device=device)
-
-    bboxes = pred[0].boxes.xyxy.cpu().numpy()
-    if bboxes.size == 0:
-        return PredictOutput()
-    bboxes = bboxes.tolist()
-
-    if pred[0].masks is None:
-        masks = create_mask_from_bbox(bboxes, image.size)
-    else:
-        masks = mask_to_pil(pred[0].masks.data, image.size)
-    preview = pred[0].plot()
-    preview = cv2.cvtColor(preview, cv2.COLOR_BGR2RGB)
-    preview = Image.fromarray(preview)
-
-    return PredictOutput(bboxes=bboxes, masks=masks, preview=preview)
-
-
-def apply_classes(model: YOLO | YOLOWorld, model_path: str | Path, classes: str):
-    if not classes or "-world" not in Path(model_path).stem:
-        return
-    parsed = [c.strip() for c in classes.split(",") if c.strip()]
-    if parsed:
-        model.set_classes(parsed)
-
-
-def mask_to_pil(masks: torch.Tensor, shape: tuple[int, int]) -> list[Image.Image]:
-    """
-    Parameters
-    ----------
-    masks: torch.Tensor, dtype=torch.float32, shape=(N, H, W).
-        The device can be CUDA, but `to_pil_image` takes care of that.
-
-    shape: tuple[int, int]
-        (W, H) of the original image
-    """
-    n = masks.shape[0]
-    return [to_pil_image(masks[i], mode="L").resize(shape) for i in range(n)]
+from __future__ import annotations
+
+from pathlib import Path
+from typing import TYPE_CHECKING
+
+import cv2
+from PIL import Image
+from torchvision.transforms.functional import to_pil_image
+
+from adetailer import PredictOutput
+from adetailer.common import create_mask_from_bbox
+
+if TYPE_CHECKING:
+    import torch
+    from ultralytics import YOLO, YOLOWorld
+
+
+def ultralytics_predict(
+    model_path: str | Path,
+    image: Image.Image,
+    confidence: float = 0.3,
+    device: str = "",
+    classes: str = "",
+) -> PredictOutput:
+    from ultralytics import YOLO
+
+    model = YOLO(model_path)
+    apply_classes(model, model_path, classes)
+    pred = model(image, conf=confidence, device=device)
+
+    bboxes = pred[0].boxes.xyxy.cpu().numpy()
+    if bboxes.size == 0:
+        return PredictOutput()
+    bboxes = bboxes.tolist()
+
+    if pred[0].masks is None:
+        masks = create_mask_from_bbox(bboxes, image.size)
+    else:
+        masks = mask_to_pil(pred[0].masks.data, image.size)
+    preview = pred[0].plot()
+    preview = cv2.cvtColor(preview, cv2.COLOR_BGR2RGB)
+    preview = Image.fromarray(preview)
+
+    return PredictOutput(bboxes=bboxes, masks=masks, preview=preview)
+
+
+def apply_classes(model: YOLO | YOLOWorld, model_path: str | Path, classes: str):
+    if not classes or "-world" not in Path(model_path).stem:
+        return
+    parsed = [c.strip() for c in classes.split(",") if c.strip()]
+    if parsed:
+        model.set_classes(parsed)
+
+
+def mask_to_pil(masks: torch.Tensor, shape: tuple[int, int]) -> list[Image.Image]:
+    """
+    Parameters
+    ----------
+    masks: torch.Tensor, dtype=torch.float32, shape=(N, H, W).
+        The device can be CUDA, but `to_pil_image` takes care of that.
+
+    shape: tuple[int, int]
+        (W, H) of the original image
+    """
+    n = masks.shape[0]
+    return [to_pil_image(masks[i], mode="L").resize(shape) for i in range(n)]
```

### Comparing `adetailer-24.4.1/controlnet_ext/controlnet_ext.py` & `adetailer-24.4.2/controlnet_ext/controlnet_ext.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-from __future__ import annotations
-
-import importlib
-import sys
-from functools import lru_cache
-from pathlib import Path
-from textwrap import dedent
-
-from modules import extensions, sd_models, shared
-
-from .common import cn_model_module, cn_model_regex
-
-try:
-    from modules.paths import extensions_builtin_dir, extensions_dir, models_path
-except ImportError as e:
-    msg = """
-    [-] ADetailer: `stable-diffusion-webui < 1.1.0` is no longer supported.
-        Please upgrade to stable-diffusion-webui >= 1.1.0.
-        or you can use ADetailer v23.10.1 (https://github.com/Bing-su/adetailer/archive/refs/tags/v23.10.1.zip)
-    """
-    raise RuntimeError(dedent(msg)) from e
-
-ext_path = Path(extensions_dir)
-ext_builtin_path = Path(extensions_builtin_dir)
-controlnet_exists = False
-controlnet_type = "standard"
-controlnet_path = None
-cn_base_path = ""
-
-for extension in extensions.active():
-    if not extension.enabled:
-        continue
-    # For cases like sd-webui-controlnet-master
-    if "sd-webui-controlnet" in extension.name:
-        controlnet_exists = True
-        controlnet_path = Path(extension.path)
-        cn_base_path = ".".join(controlnet_path.parts[-2:])
-        break
-
-if controlnet_path is not None:
-    sd_webui_controlnet_path = controlnet_path.resolve().parent
-    if sd_webui_controlnet_path.stem in ("extensions", "extensions-builtin"):
-        target_path = str(sd_webui_controlnet_path.parent)
-        if target_path not in sys.path:
-            sys.path.append(target_path)
-
-
-class ControlNetExt:
-    def __init__(self):
-        self.cn_models = ["None"]
-        self.cn_available = False
-        self.external_cn = None
-
-    def init_controlnet(self):
-        import_path = cn_base_path + ".scripts.external_code"
-
-        self.external_cn = importlib.import_module(import_path, "external_code")
-        self.cn_available = True
-        models = self.external_cn.get_models()
-        self.cn_models.extend(m for m in models if cn_model_regex.search(m))
-
-    def update_scripts_args(
-        self,
-        p,
-        model: str,
-        module: str | None,
-        weight: float,
-        guidance_start: float,
-        guidance_end: float,
-    ):
-        if (not self.cn_available) or model == "None":
-            return
-
-        if module is None or module == "None":
-            for m, v in cn_model_module.items():
-                if m in model:
-                    module = v
-                    break
-            else:
-                module = None
-
-        cn_units = [
-            self.external_cn.ControlNetUnit(
-                model=model,
-                weight=weight,
-                control_mode=self.external_cn.ControlMode.BALANCED,
-                module=module,
-                guidance_start=guidance_start,
-                guidance_end=guidance_end,
-                pixel_perfect=True,
-            )
-        ]
-
-        try:
-            self.external_cn.update_cn_script_in_processing(p, cn_units)
-        except AttributeError as e:
-            if "script_args_value" not in str(e):
-                raise
-            msg = "[-] Adetailer: ControlNet option not available in WEBUI version lower than 1.6.0 due to updates in ControlNet"
-            raise RuntimeError(msg) from e
-
-
-def get_cn_model_dirs() -> list[Path]:
-    cn_model_dir = Path(models_path, "ControlNet")
-    if controlnet_path is not None:
-        cn_model_dir_old = controlnet_path.joinpath("models")
-    else:
-        cn_model_dir_old = None
-    ext_dir1 = shared.opts.data.get("control_net_models_path", "")
-    ext_dir2 = getattr(shared.cmd_opts, "controlnet_dir", "")
-
-    dirs = [cn_model_dir]
-    dirs += [
-        Path(ext_dir) for ext_dir in [cn_model_dir_old, ext_dir1, ext_dir2] if ext_dir
-    ]
-
-    return dirs
-
-
-@lru_cache
-def _get_cn_models() -> list[str]:
-    """
-    Since we can't import ControlNet, we use a function that does something like
-    controlnet's `list(global_state.cn_models_names.values())`.
-    """
-    cn_model_exts = (".pt", ".pth", ".ckpt", ".safetensors")
-    dirs = get_cn_model_dirs()
-    name_filter = shared.opts.data.get("control_net_models_name_filter", "")
-    name_filter = name_filter.strip(" ").lower()
-
-    model_paths = []
-
-    for base in dirs:
-        if not base.exists():
-            continue
-
-        for p in base.rglob("*"):
-            if (
-                p.is_file()
-                and p.suffix in cn_model_exts
-                and cn_model_regex.search(p.name)
-            ):
-                if name_filter and name_filter not in p.name.lower():
-                    continue
-                model_paths.append(p)
-    model_paths.sort(key=lambda p: p.name)
-
-    models = []
-    for p in model_paths:
-        model_hash = sd_models.model_hash(p)
-        name = f"{p.stem} [{model_hash}]"
-        models.append(name)
-    return models
-
-
-def get_cn_models() -> list[str]:
-    if controlnet_exists:
-        return _get_cn_models()
-    return []
+from __future__ import annotations
+
+import importlib
+import sys
+from functools import lru_cache
+from pathlib import Path
+from textwrap import dedent
+
+from modules import extensions, sd_models, shared
+
+from .common import cn_model_module, cn_model_regex
+
+try:
+    from modules.paths import extensions_builtin_dir, extensions_dir, models_path
+except ImportError as e:
+    msg = """
+    [-] ADetailer: `stable-diffusion-webui < 1.1.0` is no longer supported.
+        Please upgrade to stable-diffusion-webui >= 1.1.0.
+        or you can use ADetailer v23.10.1 (https://github.com/Bing-su/adetailer/archive/refs/tags/v23.10.1.zip)
+    """
+    raise RuntimeError(dedent(msg)) from e
+
+ext_path = Path(extensions_dir)
+ext_builtin_path = Path(extensions_builtin_dir)
+controlnet_exists = False
+controlnet_type = "standard"
+controlnet_path = None
+cn_base_path = ""
+
+for extension in extensions.active():
+    if not extension.enabled:
+        continue
+    # For cases like sd-webui-controlnet-master
+    if "sd-webui-controlnet" in extension.name:
+        controlnet_exists = True
+        controlnet_path = Path(extension.path)
+        cn_base_path = ".".join(controlnet_path.parts[-2:])
+        break
+
+if controlnet_path is not None:
+    sd_webui_controlnet_path = controlnet_path.resolve().parent
+    if sd_webui_controlnet_path.stem in ("extensions", "extensions-builtin"):
+        target_path = str(sd_webui_controlnet_path.parent)
+        if target_path not in sys.path:
+            sys.path.append(target_path)
+
+
+class ControlNetExt:
+    def __init__(self):
+        self.cn_models = ["None"]
+        self.cn_available = False
+        self.external_cn = None
+
+    def init_controlnet(self):
+        import_path = cn_base_path + ".scripts.external_code"
+
+        self.external_cn = importlib.import_module(import_path, "external_code")
+        self.cn_available = True
+        models = self.external_cn.get_models()
+        self.cn_models.extend(m for m in models if cn_model_regex.search(m))
+
+    def update_scripts_args(
+        self,
+        p,
+        model: str,
+        module: str | None,
+        weight: float,
+        guidance_start: float,
+        guidance_end: float,
+    ):
+        if (not self.cn_available) or model == "None":
+            return
+
+        if module is None or module == "None":
+            for m, v in cn_model_module.items():
+                if m in model:
+                    module = v
+                    break
+            else:
+                module = None
+
+        cn_units = [
+            self.external_cn.ControlNetUnit(
+                model=model,
+                weight=weight,
+                control_mode=self.external_cn.ControlMode.BALANCED,
+                module=module,
+                guidance_start=guidance_start,
+                guidance_end=guidance_end,
+                pixel_perfect=True,
+            )
+        ]
+
+        try:
+            self.external_cn.update_cn_script_in_processing(p, cn_units)
+        except AttributeError as e:
+            if "script_args_value" not in str(e):
+                raise
+            msg = "[-] Adetailer: ControlNet option not available in WEBUI version lower than 1.6.0 due to updates in ControlNet"
+            raise RuntimeError(msg) from e
+
+
+def get_cn_model_dirs() -> list[Path]:
+    cn_model_dir = Path(models_path, "ControlNet")
+    if controlnet_path is not None:
+        cn_model_dir_old = controlnet_path.joinpath("models")
+    else:
+        cn_model_dir_old = None
+    ext_dir1 = shared.opts.data.get("control_net_models_path", "")
+    ext_dir2 = getattr(shared.cmd_opts, "controlnet_dir", "")
+
+    dirs = [cn_model_dir]
+    dirs += [
+        Path(ext_dir) for ext_dir in [cn_model_dir_old, ext_dir1, ext_dir2] if ext_dir
+    ]
+
+    return dirs
+
+
+@lru_cache
+def _get_cn_models() -> list[str]:
+    """
+    Since we can't import ControlNet, we use a function that does something like
+    controlnet's `list(global_state.cn_models_names.values())`.
+    """
+    cn_model_exts = (".pt", ".pth", ".ckpt", ".safetensors")
+    dirs = get_cn_model_dirs()
+    name_filter = shared.opts.data.get("control_net_models_name_filter", "")
+    name_filter = name_filter.strip(" ").lower()
+
+    model_paths = []
+
+    for base in dirs:
+        if not base.exists():
+            continue
+
+        for p in base.rglob("*"):
+            if (
+                p.is_file()
+                and p.suffix in cn_model_exts
+                and cn_model_regex.search(p.name)
+            ):
+                if name_filter and name_filter not in p.name.lower():
+                    continue
+                model_paths.append(p)
+    model_paths.sort(key=lambda p: p.name)
+
+    models = []
+    for p in model_paths:
+        model_hash = sd_models.model_hash(p)
+        name = f"{p.stem} [{model_hash}]"
+        models.append(name)
+    return models
+
+
+def get_cn_models() -> list[str]:
+    if controlnet_exists:
+        return _get_cn_models()
+    return []
```

### Comparing `adetailer-24.4.1/controlnet_ext/restore.py` & `adetailer-24.4.2/controlnet_ext/restore.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from __future__ import annotations
-
-from contextlib import contextmanager
-
-from modules import img2img, processing, shared
-
-
-class CNHijackRestore:
-    def __init__(self):
-        self.process = hasattr(processing, "__controlnet_original_process_images_inner")
-        self.img2img = hasattr(img2img, "__controlnet_original_process_batch")
-
-    def __enter__(self):
-        if self.process:
-            self.orig_process = processing.process_images_inner
-            processing.process_images_inner = getattr(
-                processing, "__controlnet_original_process_images_inner"
-            )
-        if self.img2img:
-            self.orig_img2img = img2img.process_batch
-            img2img.process_batch = getattr(
-                img2img, "__controlnet_original_process_batch"
-            )
-
-    def __exit__(self, *args, **kwargs):
-        if self.process:
-            processing.process_images_inner = self.orig_process
-        if self.img2img:
-            img2img.process_batch = self.orig_img2img
-
-
-@contextmanager
-def cn_allow_script_control():
-    orig = False
-    if "control_net_allow_script_control" in shared.opts.data:
-        try:
-            orig = shared.opts.data["control_net_allow_script_control"]
-            shared.opts.data["control_net_allow_script_control"] = True
-            yield
-        finally:
-            shared.opts.data["control_net_allow_script_control"] = orig
-    else:
-        yield
+from __future__ import annotations
+
+from contextlib import contextmanager
+
+from modules import img2img, processing, shared
+
+
+class CNHijackRestore:
+    def __init__(self):
+        self.process = hasattr(processing, "__controlnet_original_process_images_inner")
+        self.img2img = hasattr(img2img, "__controlnet_original_process_batch")
+
+    def __enter__(self):
+        if self.process:
+            self.orig_process = processing.process_images_inner
+            processing.process_images_inner = getattr(
+                processing, "__controlnet_original_process_images_inner"
+            )
+        if self.img2img:
+            self.orig_img2img = img2img.process_batch
+            img2img.process_batch = getattr(
+                img2img, "__controlnet_original_process_batch"
+            )
+
+    def __exit__(self, *args, **kwargs):
+        if self.process:
+            processing.process_images_inner = self.orig_process
+        if self.img2img:
+            img2img.process_batch = self.orig_img2img
+
+
+@contextmanager
+def cn_allow_script_control():
+    orig = False
+    if "control_net_allow_script_control" in shared.opts.data:
+        try:
+            orig = shared.opts.data["control_net_allow_script_control"]
+            shared.opts.data["control_net_allow_script_control"] = True
+            yield
+        finally:
+            shared.opts.data["control_net_allow_script_control"] = orig
+    else:
+        yield
```

### Comparing `adetailer-24.4.1/scripts/!adetailer.py` & `adetailer-24.4.2/scripts/!adetailer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,1039 +1,1046 @@
-from __future__ import annotations
-
-import platform
-import re
-import sys
-import traceback
-from contextlib import suppress
-from copy import copy
-from functools import partial
-from pathlib import Path
-from textwrap import dedent
-from typing import TYPE_CHECKING, Any, NamedTuple, cast
-
-import gradio as gr
-from PIL import Image, ImageChops
-from rich import print
-
-import modules
-from aaaaaa.conditional import create_binary_mask, schedulers
-from aaaaaa.helper import (
-    change_torch_load,
-    copy_extra_params,
-    pause_total_tqdm,
-    preseve_prompts,
-)
-from aaaaaa.p_method import (
-    get_i,
-    is_img2img_inpaint,
-    is_inpaint_only_masked,
-    need_call_postprocess,
-    need_call_process,
-)
-from adetailer import (
-    AFTER_DETAILER,
-    __version__,
-    get_models,
-    mediapipe_predict,
-    ultralytics_predict,
-)
-from adetailer.args import BBOX_SORTBY, SCRIPT_DEFAULT, ADetailerArgs, SkipImg2ImgOrig
-from adetailer.common import PredictOutput, ensure_pil_image, safe_mkdir
-from adetailer.mask import (
-    filter_by_ratio,
-    filter_k_largest,
-    has_intersection,
-    is_all_black,
-    mask_preprocess,
-    sort_bboxes,
-)
-from adetailer.traceback import rich_traceback
-from adetailer.ui import WebuiInfo, adui, ordinal, suffix
-from controlnet_ext import (
-    CNHijackRestore,
-    ControlNetExt,
-    cn_allow_script_control,
-    controlnet_exists,
-    controlnet_type,
-    get_cn_models,
-)
-from modules import images, paths, script_callbacks, scripts, shared
-from modules.devices import NansException
-from modules.processing import (
-    Processed,
-    StableDiffusionProcessingImg2Img,
-    create_infotext,
-    process_images,
-)
-from modules.sd_samplers import all_samplers
-from modules.shared import cmd_opts, opts, state
-
-if TYPE_CHECKING:
-    from fastapi import FastAPI
-
-no_huggingface = getattr(cmd_opts, "ad_no_huggingface", False)
-adetailer_dir = Path(paths.models_path, "adetailer")
-safe_mkdir(adetailer_dir)
-
-extra_models_dir = shared.opts.data.get("ad_extra_models_dir", "")
-model_mapping = get_models(
-    adetailer_dir,
-    extra_models_dir,
-    huggingface=not no_huggingface,
-)
-
-txt2img_submit_button = img2img_submit_button = None
-txt2img_submit_button = cast(gr.Button, txt2img_submit_button)
-img2img_submit_button = cast(gr.Button, img2img_submit_button)
-
-print(
-    f"[-] ADetailer initialized. version: {__version__}, num models: {len(model_mapping)}"
-)
-
-
-class AfterDetailerScript(scripts.Script):
-    def __init__(self):
-        super().__init__()
-        self.ultralytics_device = self.get_ultralytics_device()
-
-        self.controlnet_ext = None
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}(version={__version__})"
-
-    def title(self):
-        return AFTER_DETAILER
-
-    def show(self, is_img2img):
-        return scripts.AlwaysVisible
-
-    def ui(self, is_img2img):
-        num_models = opts.data.get("ad_max_models", 2)
-        ad_model_list = list(model_mapping.keys())
-        sampler_names = [sampler.name for sampler in all_samplers]
-        scheduler_names = [x.label for x in schedulers]
-
-        try:
-            checkpoint_list = modules.sd_models.checkpoint_tiles(use_shorts=True)
-        except TypeError:
-            checkpoint_list = modules.sd_models.checkpoint_tiles()
-        vae_list = modules.shared_items.sd_vae_items()
-
-        webui_info = WebuiInfo(
-            ad_model_list=ad_model_list,
-            sampler_names=sampler_names,
-            scheduler_names=scheduler_names,
-            t2i_button=txt2img_submit_button,
-            i2i_button=img2img_submit_button,
-            checkpoints_list=checkpoint_list,
-            vae_list=vae_list,
-        )
-
-        components, infotext_fields = adui(num_models, is_img2img, webui_info)
-
-        self.infotext_fields = infotext_fields
-        return components
-
-    def init_controlnet_ext(self) -> None:
-        if self.controlnet_ext is not None:
-            return
-        self.controlnet_ext = ControlNetExt()
-
-        if controlnet_exists:
-            try:
-                self.controlnet_ext.init_controlnet()
-            except ImportError:
-                error = traceback.format_exc()
-                print(
-                    f"[-] ADetailer: ControlNetExt init failed:\n{error}",
-                    file=sys.stderr,
-                )
-
-    def update_controlnet_args(self, p, args: ADetailerArgs) -> None:
-        if self.controlnet_ext is None:
-            self.init_controlnet_ext()
-
-        if (
-            self.controlnet_ext is not None
-            and self.controlnet_ext.cn_available
-            and args.ad_controlnet_model != "None"
-        ):
-            self.controlnet_ext.update_scripts_args(
-                p,
-                model=args.ad_controlnet_model,
-                module=args.ad_controlnet_module,
-                weight=args.ad_controlnet_weight,
-                guidance_start=args.ad_controlnet_guidance_start,
-                guidance_end=args.ad_controlnet_guidance_end,
-            )
-
-    def is_ad_enabled(self, *args_) -> bool:
-        arg_list = [arg for arg in args_ if isinstance(arg, dict)]
-        if not args_ or not arg_list:
-            message = f"""
-                       [-] ADetailer: Invalid arguments passed to ADetailer.
-                           input: {args_!r}
-                           ADetailer disabled.
-                       """
-            print(dedent(message), file=sys.stderr)
-            return False
-
-        ad_enabled = args_[0] if isinstance(args_[0], bool) else True
-        not_none = any(arg.get("ad_model", "None") != "None" for arg in arg_list)
-        return ad_enabled and not_none
-
-    def set_skip_img2img(self, p, *args_) -> None:
-        if (
-            hasattr(p, "_ad_skip_img2img")
-            or not hasattr(p, "init_images")
-            or not p.init_images
-        ):
-            return
-
-        if len(args_) >= 2 and isinstance(args_[1], bool):
-            p._ad_skip_img2img = args_[1]
-        else:
-            p._ad_skip_img2img = False
-
-        if not p._ad_skip_img2img:
-            return
-
-        if is_img2img_inpaint(p):
-            p._ad_disabled = True
-            msg = "[-] ADetailer: img2img inpainting with skip img2img is not supported. (because it's buggy)"
-            print(msg)
-            return
-
-        p._ad_orig = SkipImg2ImgOrig(
-            steps=p.steps,
-            sampler_name=p.sampler_name,
-            width=p.width,
-            height=p.height,
-        )
-        p.steps = 1
-        p.sampler_name = "Euler"
-        p.width = 128
-        p.height = 128
-
-    def get_args(self, p, *args_) -> list[ADetailerArgs]:
-        """
-        `args_` is at least 1 in length by `is_ad_enabled` immediately above
-        """
-        args = [arg for arg in args_ if isinstance(arg, dict)]
-
-        if not args:
-            message = f"[-] ADetailer: Invalid arguments passed to ADetailer: {args_!r}"
-            raise ValueError(message)
-
-        if hasattr(p, "_ad_xyz"):
-            args[0] = {**args[0], **p._ad_xyz}
-
-        all_inputs = []
-
-        for n, arg_dict in enumerate(args, 1):
-            try:
-                inp = ADetailerArgs(**arg_dict)
-            except ValueError as e:
-                msg = f"[-] ADetailer: ValidationError when validating {ordinal(n)} arguments"
-                if hasattr(e, "add_note"):
-                    e.add_note(msg)
-                else:
-                    print(msg, file=sys.stderr)
-                raise
-
-            all_inputs.append(inp)
-
-        return all_inputs
-
-    def extra_params(self, arg_list: list[ADetailerArgs]) -> dict:
-        params = {}
-        for n, args in enumerate(arg_list):
-            params.update(args.extra_params(suffix=suffix(n)))
-        params["ADetailer version"] = __version__
-        return params
-
-    @staticmethod
-    def get_ultralytics_device() -> str:
-        if "adetailer" in shared.cmd_opts.use_cpu:
-            return "cpu"
-
-        if platform.system() == "Darwin":
-            return ""
-
-        vram_args = ["lowvram", "medvram", "medvram_sdxl"]
-        if any(getattr(cmd_opts, vram, False) for vram in vram_args):
-            return "cpu"
-
-        return ""
-
-    def prompt_blank_replacement(
-        self, all_prompts: list[str], i: int, default: str
-    ) -> str:
-        if not all_prompts:
-            return default
-        if i < len(all_prompts):
-            return all_prompts[i]
-        j = i % len(all_prompts)
-        return all_prompts[j]
-
-    def _get_prompt(
-        self,
-        ad_prompt: str,
-        all_prompts: list[str],
-        i: int,
-        default: str,
-        replacements: list[PromptSR],
-    ) -> list[str]:
-        prompts = re.split(r"\s*\[SEP\]\s*", ad_prompt)
-        blank_replacement = self.prompt_blank_replacement(all_prompts, i, default)
-        for n in range(len(prompts)):
-            if not prompts[n]:
-                prompts[n] = blank_replacement
-            elif "[PROMPT]" in prompts[n]:
-                prompts[n] = prompts[n].replace("[PROMPT]", blank_replacement)
-
-            for pair in replacements:
-                prompts[n] = prompts[n].replace(pair.s, pair.r)
-        return prompts
-
-    def get_prompt(self, p, args: ADetailerArgs) -> tuple[list[str], list[str]]:
-        i = get_i(p)
-        prompt_sr = p._ad_xyz_prompt_sr if hasattr(p, "_ad_xyz_prompt_sr") else []
-
-        prompt = self._get_prompt(
-            ad_prompt=args.ad_prompt,
-            all_prompts=p.all_prompts,
-            i=i,
-            default=p.prompt,
-            replacements=prompt_sr,
-        )
-        negative_prompt = self._get_prompt(
-            ad_prompt=args.ad_negative_prompt,
-            all_prompts=p.all_negative_prompts,
-            i=i,
-            default=p.negative_prompt,
-            replacements=prompt_sr,
-        )
-
-        return prompt, negative_prompt
-
-    def get_seed(self, p) -> tuple[int, int]:
-        i = get_i(p)
-
-        if not p.all_seeds:
-            seed = p.seed
-        elif i < len(p.all_seeds):
-            seed = p.all_seeds[i]
-        else:
-            j = i % len(p.all_seeds)
-            seed = p.all_seeds[j]
-
-        if not p.all_subseeds:
-            subseed = p.subseed
-        elif i < len(p.all_subseeds):
-            subseed = p.all_subseeds[i]
-        else:
-            j = i % len(p.all_subseeds)
-            subseed = p.all_subseeds[j]
-
-        return seed, subseed
-
-    def get_width_height(self, p, args: ADetailerArgs) -> tuple[int, int]:
-        if args.ad_use_inpaint_width_height:
-            width = args.ad_inpaint_width
-            height = args.ad_inpaint_height
-        elif hasattr(p, "_ad_orig"):
-            width = p._ad_orig.width
-            height = p._ad_orig.height
-        else:
-            width = p.width
-            height = p.height
-
-        return width, height
-
-    def get_steps(self, p, args: ADetailerArgs) -> int:
-        if args.ad_use_steps:
-            return args.ad_steps
-        if hasattr(p, "_ad_orig"):
-            return p._ad_orig.steps
-        return p.steps
-
-    def get_cfg_scale(self, p, args: ADetailerArgs) -> float:
-        return args.ad_cfg_scale if args.ad_use_cfg_scale else p.cfg_scale
-
-    def get_sampler(self, p, args: ADetailerArgs) -> str:
-        if args.ad_use_sampler:
-            return args.ad_sampler
-        if hasattr(p, "_ad_orig"):
-            return p._ad_orig.sampler_name
-        return p.sampler_name
-
-    def get_scheduler(self, p, args: ADetailerArgs) -> dict[str, str]:
-        "webui >= 1.9.0"
-        if not args.ad_use_sampler:
-            return {}
-
-        if args.ad_scheduler == "Use same scheduler":
-            value = getattr(p, "scheduler", "Automatic")
-        else:
-            value = args.ad_scheduler
-        return {"scheduler": value}
-
-    def get_override_settings(self, p, args: ADetailerArgs) -> dict[str, Any]:
-        d = {}
-
-        if args.ad_use_clip_skip:
-            d["CLIP_stop_at_last_layers"] = args.ad_clip_skip
-
-        if (
-            args.ad_use_checkpoint
-            and args.ad_checkpoint
-            and args.ad_checkpoint not in ("None", "Use same checkpoint")
-        ):
-            d["sd_model_checkpoint"] = args.ad_checkpoint
-
-        if (
-            args.ad_use_vae
-            and args.ad_vae
-            and args.ad_vae not in ("None", "Use same VAE")
-        ):
-            d["sd_vae"] = args.ad_vae
-        return d
-
-    def get_initial_noise_multiplier(self, p, args: ADetailerArgs) -> float | None:
-        return args.ad_noise_multiplier if args.ad_use_noise_multiplier else None
-
-    @staticmethod
-    def infotext(p) -> str:
-        return create_infotext(
-            p, p.all_prompts, p.all_seeds, p.all_subseeds, None, 0, 0
-        )
-
-    def write_params_txt(self, content: str) -> None:
-        params_txt = Path(paths.data_path, "params.txt")
-        with suppress(Exception):
-            params_txt.write_text(content, encoding="utf-8")
-
-    @staticmethod
-    def script_args_copy(script_args):
-        type_: type[list] | type[tuple] = type(script_args)
-        result = []
-        for arg in script_args:
-            try:
-                a = copy(arg)
-            except TypeError:
-                a = arg
-            result.append(a)
-        return type_(result)
-
-    def script_filter(self, p, args: ADetailerArgs):
-        script_runner = copy(p.scripts)
-        script_args = self.script_args_copy(p.script_args)
-
-        ad_only_seleted_scripts = opts.data.get("ad_only_seleted_scripts", True)
-        if not ad_only_seleted_scripts:
-            return script_runner, script_args
-
-        ad_script_names = opts.data.get("ad_script_names", SCRIPT_DEFAULT)
-        script_names_set = {
-            name
-            for script_name in ad_script_names.split(",")
-            for name in (script_name, script_name.strip())
-        }
-
-        if args.ad_controlnet_model != "None":
-            script_names_set.add("controlnet")
-
-        filtered_alwayson = []
-        for script_object in script_runner.alwayson_scripts:
-            filepath = script_object.filename
-            filename = Path(filepath).stem
-            if filename in script_names_set:
-                filtered_alwayson.append(script_object)
-
-        script_runner.alwayson_scripts = filtered_alwayson
-        return script_runner, script_args
-
-    def disable_controlnet_units(
-        self, script_args: list[Any] | tuple[Any, ...]
-    ) -> None:
-        for obj in script_args:
-            if "controlnet" in obj.__class__.__name__.lower():
-                if hasattr(obj, "enabled"):
-                    obj.enabled = False
-                if hasattr(obj, "input_mode"):
-                    obj.input_mode = getattr(obj.input_mode, "SIMPLE", "simple")
-
-            elif isinstance(obj, dict) and "module" in obj:
-                obj["enabled"] = False
-
-    def get_i2i_p(self, p, args: ADetailerArgs, image):
-        seed, subseed = self.get_seed(p)
-        width, height = self.get_width_height(p, args)
-        steps = self.get_steps(p, args)
-        cfg_scale = self.get_cfg_scale(p, args)
-        initial_noise_multiplier = self.get_initial_noise_multiplier(p, args)
-        sampler_name = self.get_sampler(p, args)
-        override_settings = self.get_override_settings(p, args)
-
-        version_args = {}
-        if schedulers:
-            version_args.update(self.get_scheduler(p, args))
-
-        i2i = StableDiffusionProcessingImg2Img(
-            init_images=[image],
-            resize_mode=0,
-            denoising_strength=args.ad_denoising_strength,
-            mask=None,
-            mask_blur=args.ad_mask_blur,
-            inpainting_fill=1,
-            inpaint_full_res=args.ad_inpaint_only_masked,
-            inpaint_full_res_padding=args.ad_inpaint_only_masked_padding,
-            inpainting_mask_invert=0,
-            initial_noise_multiplier=initial_noise_multiplier,
-            sd_model=p.sd_model,
-            outpath_samples=p.outpath_samples,
-            outpath_grids=p.outpath_grids,
-            prompt="",  # replace later
-            negative_prompt="",
-            styles=p.styles,
-            seed=seed,
-            subseed=subseed,
-            subseed_strength=p.subseed_strength,
-            seed_resize_from_h=p.seed_resize_from_h,
-            seed_resize_from_w=p.seed_resize_from_w,
-            sampler_name=sampler_name,
-            batch_size=1,
-            n_iter=1,
-            steps=steps,
-            cfg_scale=cfg_scale,
-            width=width,
-            height=height,
-            restore_faces=args.ad_restore_face,
-            tiling=p.tiling,
-            extra_generation_params=copy_extra_params(p.extra_generation_params),
-            do_not_save_samples=True,
-            do_not_save_grid=True,
-            override_settings=override_settings,
-            **version_args,
-        )
-
-        i2i.cached_c = [None, None]
-        i2i.cached_uc = [None, None]
-        i2i.scripts, i2i.script_args = self.script_filter(p, args)
-        i2i._ad_disabled = True
-        i2i._ad_inner = True
-
-        if args.ad_controlnet_model != "Passthrough" and controlnet_type != "forge":
-            self.disable_controlnet_units(i2i.script_args)
-
-        if args.ad_controlnet_model not in ["None", "Passthrough"]:
-            self.update_controlnet_args(i2i, args)
-        elif args.ad_controlnet_model == "None":
-            i2i.control_net_enabled = False
-
-        return i2i
-
-    def save_image(self, p, image, *, condition: str, suffix: str) -> None:
-        i = get_i(p)
-        if p.all_prompts:
-            i %= len(p.all_prompts)
-            save_prompt = p.all_prompts[i]
-        else:
-            save_prompt = p.prompt
-        seed, _ = self.get_seed(p)
-
-        if opts.data.get(condition, False):
-            images.save_image(
-                image=image,
-                path=p.outpath_samples,
-                basename="",
-                seed=seed,
-                prompt=save_prompt,
-                extension=opts.samples_format,
-                info=self.infotext(p),
-                p=p,
-                suffix=suffix,
-            )
-
-    def get_ad_model(self, name: str):
-        if name not in model_mapping:
-            msg = f"[-] ADetailer: Model {name!r} not found. Available models: {list(model_mapping.keys())}"
-            raise ValueError(msg)
-        return model_mapping[name]
-
-    def sort_bboxes(self, pred: PredictOutput) -> PredictOutput:
-        sortby = opts.data.get("ad_bbox_sortby", BBOX_SORTBY[0])
-        sortby_idx = BBOX_SORTBY.index(sortby)
-        return sort_bboxes(pred, sortby_idx)
-
-    def pred_preprocessing(self, p, pred: PredictOutput, args: ADetailerArgs):
-        pred = filter_by_ratio(
-            pred, low=args.ad_mask_min_ratio, high=args.ad_mask_max_ratio
-        )
-        pred = filter_k_largest(pred, k=args.ad_mask_k_largest)
-        pred = self.sort_bboxes(pred)
-        masks = mask_preprocess(
-            pred.masks,
-            kernel=args.ad_dilate_erode,
-            x_offset=args.ad_x_offset,
-            y_offset=args.ad_y_offset,
-            merge_invert=args.ad_mask_merge_invert,
-        )
-
-        if is_img2img_inpaint(p) and not is_inpaint_only_masked(p):
-            image_mask = self.get_image_mask(p)
-            masks = self.inpaint_mask_filter(image_mask, masks)
-        return masks
-
-    @staticmethod
-    def i2i_prompts_replace(
-        i2i, prompts: list[str], negative_prompts: list[str], j: int
-    ) -> None:
-        i1 = min(j, len(prompts) - 1)
-        i2 = min(j, len(negative_prompts) - 1)
-        prompt = prompts[i1]
-        negative_prompt = negative_prompts[i2]
-        i2i.prompt = prompt
-        i2i.negative_prompt = negative_prompt
-
-    @staticmethod
-    def compare_prompt(p, extra_params: dict[str, Any], processed, n: int = 0):
-        if not hasattr(p, "_ad_extra_params_result"):
-            p._ad_extra_params_result = {}
-
-        pt = "ADetailer prompt" + suffix(n)
-        if pt in extra_params and extra_params[pt] != processed.all_prompts[0]:
-            print(
-                f"[-] ADetailer: applied {ordinal(n + 1)} ad_prompt: {processed.all_prompts[0]!r}"
-            )
-            p._ad_extra_params_result[pt] = processed.all_prompts[0]
-
-        ng = "ADetailer negative prompt" + suffix(n)
-        if ng in extra_params and extra_params[ng] != processed.all_negative_prompts[0]:
-            print(
-                f"[-] ADetailer: applied {ordinal(n + 1)} ad_negative_prompt: {processed.all_negative_prompts[0]!r}"
-            )
-            p._ad_extra_params_result[ng] = processed.all_negative_prompts[0]
-
-    @staticmethod
-    def get_i2i_init_image(p, pp):
-        if getattr(p, "_ad_skip_img2img", False):
-            return p.init_images[0]
-        return pp.image
-
-    @staticmethod
-    def get_each_tap_seed(seed: int, i: int):
-        use_same_seed = shared.opts.data.get("ad_same_seed_for_each_tap", False)
-        return seed if use_same_seed else seed + i
-
-    @staticmethod
-    def inpaint_mask_filter(
-        img2img_mask: Image.Image, ad_mask: list[Image.Image]
-    ) -> list[Image.Image]:
-        if ad_mask and img2img_mask.size != ad_mask[0].size:
-            img2img_mask = img2img_mask.resize(ad_mask[0].size, resample=images.LANCZOS)
-        return [mask for mask in ad_mask if has_intersection(img2img_mask, mask)]
-
-    @staticmethod
-    def get_image_mask(p) -> Image.Image:
-        mask = p.image_mask
-        if getattr(p, "inpainting_mask_invert", False):
-            mask = ImageChops.invert(mask)
-        mask = create_binary_mask(mask)
-
-        if getattr(p, "_ad_skip_img2img", False):
-            if hasattr(p, "init_images") and p.init_images:
-                width, height = p.init_images[0].size
-            else:
-                msg = "[-] ADetailer: no init_images."
-                raise RuntimeError(msg)
-        else:
-            width, height = p.width, p.height
-        return images.resize_image(p.resize_mode, mask, width, height)
-
-    @rich_traceback
-    def process(self, p, *args_):
-        if getattr(p, "_ad_disabled", False):
-            return
-
-        if is_img2img_inpaint(p) and is_all_black(self.get_image_mask(p)):
-            p._ad_disabled = True
-            msg = (
-                "[-] ADetailer: img2img inpainting with no mask -- adetailer disabled."
-            )
-            print(msg)
-            return
-
-        if not self.is_ad_enabled(*args_):
-            p._ad_disabled = True
-            return
-
-        self.set_skip_img2img(p, *args_)
-        if getattr(p, "_ad_disabled", False):
-            # case when img2img inpainting with skip img2img
-            return
-
-        arg_list = self.get_args(p, *args_)
-
-        if hasattr(p, "_ad_xyz_prompt_sr"):
-            replaced_positive_prompt, replaced_negative_prompt = self.get_prompt(
-                p, arg_list[0]
-            )
-            arg_list[0].ad_prompt = replaced_positive_prompt[0]
-            arg_list[0].ad_negative_prompt = replaced_negative_prompt[0]
-
-        extra_params = self.extra_params(arg_list)
-        p.extra_generation_params.update(extra_params)
-
-    def _postprocess_image_inner(
-        self, p, pp, args: ADetailerArgs, *, n: int = 0
-    ) -> bool:
-        """
-        Returns
-        -------
-            bool
-
-            `True` if image was processed, `False` otherwise.
-        """
-        if state.interrupted or state.skipped:
-            return False
-
-        i = get_i(p)
-
-        i2i = self.get_i2i_p(p, args, pp.image)
-        seed, subseed = self.get_seed(p)
-        ad_prompts, ad_negatives = self.get_prompt(p, args)
-
-        is_mediapipe = args.ad_model.lower().startswith("mediapipe")
-
-        kwargs = {}
-        if is_mediapipe:
-            predictor = mediapipe_predict
-            ad_model = args.ad_model
-        else:
-            predictor = ultralytics_predict
-            ad_model = self.get_ad_model(args.ad_model)
-            kwargs["device"] = self.ultralytics_device
-            kwargs["classes"] = args.ad_model_classes
-
-        with change_torch_load():
-            pred = predictor(ad_model, pp.image, args.ad_confidence, **kwargs)
-
-        if pred.preview is None:
-            print(
-                f"[-] ADetailer: nothing detected on image {i + 1} with {ordinal(n + 1)} settings."
-            )
-            return False
-
-        masks = self.pred_preprocessing(p, pred, args)
-        shared.state.assign_current_image(pred.preview)
-
-        self.save_image(
-            p,
-            pred.preview,
-            condition="ad_save_previews",
-            suffix="-ad-preview" + suffix(n, "-"),
-        )
-
-        steps = len(masks)
-        processed = None
-        state.job_count += steps
-
-        if is_mediapipe:
-            print(f"mediapipe: {steps} detected.")
-
-        p2 = copy(i2i)
-        for j in range(steps):
-            p2.image_mask = masks[j]
-            p2.init_images[0] = ensure_pil_image(p2.init_images[0], "RGB")
-            self.i2i_prompts_replace(p2, ad_prompts, ad_negatives, j)
-
-            if re.match(r"^\s*\[SKIP\]\s*$", p2.prompt):
-                continue
-
-            p2.seed = self.get_each_tap_seed(seed, j)
-            p2.subseed = self.get_each_tap_seed(subseed, j)
-
-            try:
-                processed = process_images(p2)
-            except NansException as e:
-                msg = f"[-] ADetailer: 'NansException' occurred with {ordinal(n + 1)} settings.\n{e}"
-                print(msg, file=sys.stderr)
-                continue
-            finally:
-                p2.close()
-
-            self.compare_prompt(p, p.extra_generation_params, processed, n=n)
-            p2 = copy(i2i)
-            p2.init_images = [processed.images[0]]
-
-        if processed is not None:
-            pp.image = processed.images[0]
-            return True
-
-        return False
-
-    @rich_traceback
-    def postprocess_image(self, p, pp, *args_):
-        if getattr(p, "_ad_disabled", False) or not self.is_ad_enabled(*args_):
-            return
-
-        pp.image = self.get_i2i_init_image(p, pp)
-        pp.image = ensure_pil_image(pp.image, "RGB")
-        init_image = copy(pp.image)
-        arg_list = self.get_args(p, *args_)
-        params_txt_content = Path(paths.data_path, "params.txt").read_text("utf-8")
-
-        if need_call_postprocess(p):
-            dummy = Processed(p, [], p.seed, "")
-            with preseve_prompts(p):
-                p.scripts.postprocess(copy(p), dummy)
-
-        is_processed = False
-        with CNHijackRestore(), pause_total_tqdm(), cn_allow_script_control():
-            for n, args in enumerate(arg_list):
-                if args.ad_model == "None":
-                    continue
-                is_processed |= self._postprocess_image_inner(p, pp, args, n=n)
-
-        if is_processed and not getattr(p, "_ad_skip_img2img", False):
-            self.save_image(
-                p, init_image, condition="ad_save_images_before", suffix="-ad-before"
-            )
-
-        if need_call_process(p):
-            with preseve_prompts(p):
-                copy_p = copy(p)
-                if hasattr(p.scripts, "before_process"):
-                    p.scripts.before_process(copy_p)
-                p.scripts.process(copy_p)
-
-        self.write_params_txt(params_txt_content)
-
-        if hasattr(p, "_ad_extra_params_result"):
-            p.extra_generation_params.update(p._ad_extra_params_result)
-
-
-def on_after_component(component, **_kwargs):
-    global txt2img_submit_button, img2img_submit_button
-    if getattr(component, "elem_id", None) == "txt2img_generate":
-        txt2img_submit_button = component
-        return
-
-    if getattr(component, "elem_id", None) == "img2img_generate":
-        img2img_submit_button = component
-
-
-def on_ui_settings():
-    section = ("ADetailer", AFTER_DETAILER)
-    shared.opts.add_option(
-        "ad_max_models",
-        shared.OptionInfo(
-            default=2,
-            label="Max models",
-            component=gr.Slider,
-            component_args={"minimum": 1, "maximum": 10, "step": 1},
-            section=section,
-        ),
-    )
-
-    shared.opts.add_option(
-        "ad_extra_models_dir",
-        shared.OptionInfo(
-            default="",
-            label="Extra path to scan adetailer models",
-            component=gr.Textbox,
-            section=section,
-        ),
-    )
-
-    shared.opts.add_option(
-        "ad_save_previews",
-        shared.OptionInfo(False, "Save mask previews", section=section),
-    )
-
-    shared.opts.add_option(
-        "ad_save_images_before",
-        shared.OptionInfo(False, "Save images before ADetailer", section=section),
-    )
-
-    shared.opts.add_option(
-        "ad_only_seleted_scripts",
-        shared.OptionInfo(
-            True, "Apply only selected scripts to ADetailer", section=section
-        ),
-    )
-
-    textbox_args = {
-        "placeholder": "comma-separated list of script names",
-        "interactive": True,
-    }
-
-    shared.opts.add_option(
-        "ad_script_names",
-        shared.OptionInfo(
-            default=SCRIPT_DEFAULT,
-            label="Script names to apply to ADetailer (separated by comma)",
-            component=gr.Textbox,
-            component_args=textbox_args,
-            section=section,
-        ),
-    )
-
-    shared.opts.add_option(
-        "ad_bbox_sortby",
-        shared.OptionInfo(
-            default="None",
-            label="Sort bounding boxes by",
-            component=gr.Radio,
-            component_args={"choices": BBOX_SORTBY},
-            section=section,
-        ),
-    )
-
-    shared.opts.add_option(
-        "ad_same_seed_for_each_tap",
-        shared.OptionInfo(
-            False, "Use same seed for each tab in adetailer", section=section
-        ),
-    )
-
-
-# xyz_grid
-
-
-class PromptSR(NamedTuple):
-    s: str
-    r: str
-
-
-def set_value(p, x: Any, xs: Any, *, field: str):
-    if not hasattr(p, "_ad_xyz"):
-        p._ad_xyz = {}
-    p._ad_xyz[field] = x
-
-
-def search_and_replace_prompt(p, x: Any, xs: Any, replace_in_main_prompt: bool):
-    if replace_in_main_prompt:
-        p.prompt = p.prompt.replace(xs[0], x)
-        p.negative_prompt = p.negative_prompt.replace(xs[0], x)
-
-    if not hasattr(p, "_ad_xyz_prompt_sr"):
-        p._ad_xyz_prompt_sr = []
-    p._ad_xyz_prompt_sr.append(PromptSR(s=xs[0], r=x))
-
-
-def make_axis_on_xyz_grid():
-    xyz_grid = None
-    for script in scripts.scripts_data:
-        if script.script_class.__module__ == "xyz_grid.py":
-            xyz_grid = script.module
-            break
-
-    if xyz_grid is None:
-        return
-
-    model_list = ["None", *model_mapping.keys()]
-    samplers = [sampler.name for sampler in all_samplers]
-
-    axis = [
-        xyz_grid.AxisOption(
-            "[ADetailer] ADetailer model 1st",
-            str,
-            partial(set_value, field="ad_model"),
-            choices=lambda: model_list,
-        ),
-        xyz_grid.AxisOption(
-            "[ADetailer] ADetailer prompt 1st",
-            str,
-            partial(set_value, field="ad_prompt"),
-        ),
-        xyz_grid.AxisOption(
-            "[ADetailer] ADetailer negative prompt 1st",
-            str,
-            partial(set_value, field="ad_negative_prompt"),
-        ),
-        xyz_grid.AxisOption(
-            "[ADetailer] Prompt S/R (AD 1st)",
-            str,
-            partial(search_and_replace_prompt, replace_in_main_prompt=False),
-        ),
-        xyz_grid.AxisOption(
-            "[ADetailer] Prompt S/R (AD 1st and main prompt)",
-            str,
-            partial(search_and_replace_prompt, replace_in_main_prompt=True),
-        ),
-        xyz_grid.AxisOption(
-            "[ADetailer] Mask erosion / dilation 1st",
-            int,
-            partial(set_value, field="ad_dilate_erode"),
-        ),
-        xyz_grid.AxisOption(
-            "[ADetailer] Inpaint denoising strength 1st",
-            float,
-            partial(set_value, field="ad_denoising_strength"),
-        ),
-        xyz_grid.AxisOption(
-            "[ADetailer] Inpaint only masked 1st",
-            str,
-            partial(set_value, field="ad_inpaint_only_masked"),
-            choices=lambda: ["True", "False"],
-        ),
-        xyz_grid.AxisOption(
-            "[ADetailer] Inpaint only masked padding 1st",
-            int,
-            partial(set_value, field="ad_inpaint_only_masked_padding"),
-        ),
-        xyz_grid.AxisOption(
-            "[ADetailer] ADetailer sampler 1st",
-            str,
-            partial(set_value, field="ad_sampler"),
-            choices=lambda: samplers,
-        ),
-        xyz_grid.AxisOption(
-            "[ADetailer] ControlNet model 1st",
-            str,
-            partial(set_value, field="ad_controlnet_model"),
-            choices=lambda: ["None", "Passthrough", *get_cn_models()],
-        ),
-    ]
-
-    if not any(x.label.startswith("[ADetailer]") for x in xyz_grid.axis_options):
-        xyz_grid.axis_options.extend(axis)
-
-
-def on_before_ui():
-    try:
-        make_axis_on_xyz_grid()
-    except Exception:
-        error = traceback.format_exc()
-        print(
-            f"[-] ADetailer: xyz_grid error:\n{error}",
-            file=sys.stderr,
-        )
-
-
-# api
-
-
-def add_api_endpoints(_: gr.Blocks, app: FastAPI):
-    @app.get("/adetailer/v1/version")
-    async def version():
-        return {"version": __version__}
-
-    @app.get("/adetailer/v1/schema")
-    async def schema():
-        if hasattr(ADetailerArgs, "model_json_schema"):
-            return ADetailerArgs.model_json_schema()
-        return ADetailerArgs.schema()
-
-    @app.get("/adetailer/v1/ad_model")
-    async def ad_model():
-        return {"ad_model": list(model_mapping)}
-
-
-script_callbacks.on_ui_settings(on_ui_settings)
-script_callbacks.on_after_component(on_after_component)
-script_callbacks.on_app_started(add_api_endpoints)
-script_callbacks.on_before_ui(on_before_ui)
+from __future__ import annotations
+
+import platform
+import re
+import sys
+import traceback
+from copy import copy
+from functools import partial
+from pathlib import Path
+from textwrap import dedent
+from typing import TYPE_CHECKING, Any, NamedTuple, cast
+
+import gradio as gr
+from PIL import Image, ImageChops
+from rich import print
+
+import modules
+from aaaaaa.conditional import create_binary_mask, schedulers
+from aaaaaa.helper import (
+    change_torch_load,
+    copy_extra_params,
+    pause_total_tqdm,
+    preseve_prompts,
+)
+from aaaaaa.p_method import (
+    get_i,
+    is_img2img_inpaint,
+    is_inpaint_only_masked,
+    need_call_postprocess,
+    need_call_process,
+)
+from adetailer import (
+    AFTER_DETAILER,
+    __version__,
+    get_models,
+    mediapipe_predict,
+    ultralytics_predict,
+)
+from adetailer.args import BBOX_SORTBY, SCRIPT_DEFAULT, ADetailerArgs, SkipImg2ImgOrig
+from adetailer.common import PredictOutput, ensure_pil_image, safe_mkdir
+from adetailer.mask import (
+    filter_by_ratio,
+    filter_k_largest,
+    has_intersection,
+    is_all_black,
+    mask_preprocess,
+    sort_bboxes,
+)
+from adetailer.traceback import rich_traceback
+from adetailer.ui import WebuiInfo, adui, ordinal, suffix
+from controlnet_ext import (
+    CNHijackRestore,
+    ControlNetExt,
+    cn_allow_script_control,
+    controlnet_exists,
+    controlnet_type,
+    get_cn_models,
+)
+from modules import images, paths, script_callbacks, scripts, shared
+from modules.devices import NansException
+from modules.processing import (
+    Processed,
+    StableDiffusionProcessingImg2Img,
+    create_infotext,
+    process_images,
+)
+from modules.sd_samplers import all_samplers
+from modules.shared import cmd_opts, opts, state
+
+if TYPE_CHECKING:
+    from fastapi import FastAPI
+
+PARAMS_TXT = "params.txt"
+
+no_huggingface = getattr(cmd_opts, "ad_no_huggingface", False)
+adetailer_dir = Path(paths.models_path, "adetailer")
+safe_mkdir(adetailer_dir)
+
+extra_models_dir = shared.opts.data.get("ad_extra_models_dir", "")
+model_mapping = get_models(
+    adetailer_dir,
+    extra_models_dir,
+    huggingface=not no_huggingface,
+)
+
+txt2img_submit_button = img2img_submit_button = None
+txt2img_submit_button = cast(gr.Button, txt2img_submit_button)
+img2img_submit_button = cast(gr.Button, img2img_submit_button)
+
+print(
+    f"[-] ADetailer initialized. version: {__version__}, num models: {len(model_mapping)}"
+)
+
+
+class AfterDetailerScript(scripts.Script):
+    def __init__(self):
+        super().__init__()
+        self.ultralytics_device = self.get_ultralytics_device()
+
+        self.controlnet_ext = None
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}(version={__version__})"
+
+    def title(self):
+        return AFTER_DETAILER
+
+    def show(self, is_img2img):
+        return scripts.AlwaysVisible
+
+    def ui(self, is_img2img):
+        num_models = opts.data.get("ad_max_models", 2)
+        ad_model_list = list(model_mapping.keys())
+        sampler_names = [sampler.name for sampler in all_samplers]
+        scheduler_names = [x.label for x in schedulers]
+
+        try:
+            checkpoint_list = modules.sd_models.checkpoint_tiles(use_shorts=True)
+        except TypeError:
+            checkpoint_list = modules.sd_models.checkpoint_tiles()
+        vae_list = modules.shared_items.sd_vae_items()
+
+        webui_info = WebuiInfo(
+            ad_model_list=ad_model_list,
+            sampler_names=sampler_names,
+            scheduler_names=scheduler_names,
+            t2i_button=txt2img_submit_button,
+            i2i_button=img2img_submit_button,
+            checkpoints_list=checkpoint_list,
+            vae_list=vae_list,
+        )
+
+        components, infotext_fields = adui(num_models, is_img2img, webui_info)
+
+        self.infotext_fields = infotext_fields
+        return components
+
+    def init_controlnet_ext(self) -> None:
+        if self.controlnet_ext is not None:
+            return
+        self.controlnet_ext = ControlNetExt()
+
+        if controlnet_exists:
+            try:
+                self.controlnet_ext.init_controlnet()
+            except ImportError:
+                error = traceback.format_exc()
+                print(
+                    f"[-] ADetailer: ControlNetExt init failed:\n{error}",
+                    file=sys.stderr,
+                )
+
+    def update_controlnet_args(self, p, args: ADetailerArgs) -> None:
+        if self.controlnet_ext is None:
+            self.init_controlnet_ext()
+
+        if (
+            self.controlnet_ext is not None
+            and self.controlnet_ext.cn_available
+            and args.ad_controlnet_model != "None"
+        ):
+            self.controlnet_ext.update_scripts_args(
+                p,
+                model=args.ad_controlnet_model,
+                module=args.ad_controlnet_module,
+                weight=args.ad_controlnet_weight,
+                guidance_start=args.ad_controlnet_guidance_start,
+                guidance_end=args.ad_controlnet_guidance_end,
+            )
+
+    def is_ad_enabled(self, *args_) -> bool:
+        arg_list = [arg for arg in args_ if isinstance(arg, dict)]
+        if not args_ or not arg_list:
+            message = f"""
+                       [-] ADetailer: Invalid arguments passed to ADetailer.
+                           input: {args_!r}
+                           ADetailer disabled.
+                       """
+            print(dedent(message), file=sys.stderr)
+            return False
+
+        ad_enabled = args_[0] if isinstance(args_[0], bool) else True
+        not_none = any(arg.get("ad_model", "None") != "None" for arg in arg_list)
+        return ad_enabled and not_none
+
+    def set_skip_img2img(self, p, *args_) -> None:
+        if (
+            hasattr(p, "_ad_skip_img2img")
+            or not hasattr(p, "init_images")
+            or not p.init_images
+        ):
+            return
+
+        if len(args_) >= 2 and isinstance(args_[1], bool):
+            p._ad_skip_img2img = args_[1]
+        else:
+            p._ad_skip_img2img = False
+
+        if not p._ad_skip_img2img:
+            return
+
+        if is_img2img_inpaint(p):
+            p._ad_disabled = True
+            msg = "[-] ADetailer: img2img inpainting with skip img2img is not supported. (because it's buggy)"
+            print(msg)
+            return
+
+        p._ad_orig = SkipImg2ImgOrig(
+            steps=p.steps,
+            sampler_name=p.sampler_name,
+            width=p.width,
+            height=p.height,
+        )
+        p.steps = 1
+        p.sampler_name = "Euler"
+        p.width = 128
+        p.height = 128
+
+    def get_args(self, p, *args_) -> list[ADetailerArgs]:
+        """
+        `args_` is at least 1 in length by `is_ad_enabled` immediately above
+        """
+        args = [arg for arg in args_ if isinstance(arg, dict)]
+
+        if not args:
+            message = f"[-] ADetailer: Invalid arguments passed to ADetailer: {args_!r}"
+            raise ValueError(message)
+
+        if hasattr(p, "_ad_xyz"):
+            args[0] = {**args[0], **p._ad_xyz}
+
+        all_inputs = []
+
+        for n, arg_dict in enumerate(args, 1):
+            try:
+                inp = ADetailerArgs(**arg_dict)
+            except ValueError as e:
+                msg = f"[-] ADetailer: ValidationError when validating {ordinal(n)} arguments"
+                if hasattr(e, "add_note"):
+                    e.add_note(msg)
+                else:
+                    print(msg, file=sys.stderr)
+                raise
+
+            all_inputs.append(inp)
+
+        return all_inputs
+
+    def extra_params(self, arg_list: list[ADetailerArgs]) -> dict:
+        params = {}
+        for n, args in enumerate(arg_list):
+            params.update(args.extra_params(suffix=suffix(n)))
+        params["ADetailer version"] = __version__
+        return params
+
+    @staticmethod
+    def get_ultralytics_device() -> str:
+        if "adetailer" in shared.cmd_opts.use_cpu:
+            return "cpu"
+
+        if platform.system() == "Darwin":
+            return ""
+
+        vram_args = ["lowvram", "medvram", "medvram_sdxl"]
+        if any(getattr(cmd_opts, vram, False) for vram in vram_args):
+            return "cpu"
+
+        return ""
+
+    def prompt_blank_replacement(
+        self, all_prompts: list[str], i: int, default: str
+    ) -> str:
+        if not all_prompts:
+            return default
+        if i < len(all_prompts):
+            return all_prompts[i]
+        j = i % len(all_prompts)
+        return all_prompts[j]
+
+    def _get_prompt(
+        self,
+        ad_prompt: str,
+        all_prompts: list[str],
+        i: int,
+        default: str,
+        replacements: list[PromptSR],
+    ) -> list[str]:
+        prompts = re.split(r"\s*\[SEP\]\s*", ad_prompt)
+        blank_replacement = self.prompt_blank_replacement(all_prompts, i, default)
+        for n in range(len(prompts)):
+            if not prompts[n]:
+                prompts[n] = blank_replacement
+            elif "[PROMPT]" in prompts[n]:
+                prompts[n] = prompts[n].replace("[PROMPT]", blank_replacement)
+
+            for pair in replacements:
+                prompts[n] = prompts[n].replace(pair.s, pair.r)
+        return prompts
+
+    def get_prompt(self, p, args: ADetailerArgs) -> tuple[list[str], list[str]]:
+        i = get_i(p)
+        prompt_sr = p._ad_xyz_prompt_sr if hasattr(p, "_ad_xyz_prompt_sr") else []
+
+        prompt = self._get_prompt(
+            ad_prompt=args.ad_prompt,
+            all_prompts=p.all_prompts,
+            i=i,
+            default=p.prompt,
+            replacements=prompt_sr,
+        )
+        negative_prompt = self._get_prompt(
+            ad_prompt=args.ad_negative_prompt,
+            all_prompts=p.all_negative_prompts,
+            i=i,
+            default=p.negative_prompt,
+            replacements=prompt_sr,
+        )
+
+        return prompt, negative_prompt
+
+    def get_seed(self, p) -> tuple[int, int]:
+        i = get_i(p)
+
+        if not p.all_seeds:
+            seed = p.seed
+        elif i < len(p.all_seeds):
+            seed = p.all_seeds[i]
+        else:
+            j = i % len(p.all_seeds)
+            seed = p.all_seeds[j]
+
+        if not p.all_subseeds:
+            subseed = p.subseed
+        elif i < len(p.all_subseeds):
+            subseed = p.all_subseeds[i]
+        else:
+            j = i % len(p.all_subseeds)
+            subseed = p.all_subseeds[j]
+
+        return seed, subseed
+
+    def get_width_height(self, p, args: ADetailerArgs) -> tuple[int, int]:
+        if args.ad_use_inpaint_width_height:
+            width = args.ad_inpaint_width
+            height = args.ad_inpaint_height
+        elif hasattr(p, "_ad_orig"):
+            width = p._ad_orig.width
+            height = p._ad_orig.height
+        else:
+            width = p.width
+            height = p.height
+
+        return width, height
+
+    def get_steps(self, p, args: ADetailerArgs) -> int:
+        if args.ad_use_steps:
+            return args.ad_steps
+        if hasattr(p, "_ad_orig"):
+            return p._ad_orig.steps
+        return p.steps
+
+    def get_cfg_scale(self, p, args: ADetailerArgs) -> float:
+        return args.ad_cfg_scale if args.ad_use_cfg_scale else p.cfg_scale
+
+    def get_sampler(self, p, args: ADetailerArgs) -> str:
+        if args.ad_use_sampler:
+            return args.ad_sampler
+        if hasattr(p, "_ad_orig"):
+            return p._ad_orig.sampler_name
+        return p.sampler_name
+
+    def get_scheduler(self, p, args: ADetailerArgs) -> dict[str, str]:
+        "webui >= 1.9.0"
+        if not args.ad_use_sampler:
+            return {}
+
+        if args.ad_scheduler == "Use same scheduler":
+            value = getattr(p, "scheduler", "Automatic")
+        else:
+            value = args.ad_scheduler
+        return {"scheduler": value}
+
+    def get_override_settings(self, p, args: ADetailerArgs) -> dict[str, Any]:
+        d = {}
+
+        if args.ad_use_clip_skip:
+            d["CLIP_stop_at_last_layers"] = args.ad_clip_skip
+
+        if (
+            args.ad_use_checkpoint
+            and args.ad_checkpoint
+            and args.ad_checkpoint not in ("None", "Use same checkpoint")
+        ):
+            d["sd_model_checkpoint"] = args.ad_checkpoint
+
+        if (
+            args.ad_use_vae
+            and args.ad_vae
+            and args.ad_vae not in ("None", "Use same VAE")
+        ):
+            d["sd_vae"] = args.ad_vae
+        return d
+
+    def get_initial_noise_multiplier(self, p, args: ADetailerArgs) -> float | None:
+        return args.ad_noise_multiplier if args.ad_use_noise_multiplier else None
+
+    @staticmethod
+    def infotext(p) -> str:
+        return create_infotext(
+            p, p.all_prompts, p.all_seeds, p.all_subseeds, None, 0, 0
+        )
+
+    def read_params_txt(self) -> str:
+        params_txt = Path(paths.data_path, PARAMS_TXT)
+        if params_txt.exists():
+            return params_txt.read_text(encoding="utf-8")
+        return ""
+
+    def write_params_txt(self, content: str) -> None:
+        params_txt = Path(paths.data_path, PARAMS_TXT)
+        if params_txt.exists() and content:
+            params_txt.write_text(content, encoding="utf-8")
+
+    @staticmethod
+    def script_args_copy(script_args):
+        type_: type[list] | type[tuple] = type(script_args)
+        result = []
+        for arg in script_args:
+            try:
+                a = copy(arg)
+            except TypeError:
+                a = arg
+            result.append(a)
+        return type_(result)
+
+    def script_filter(self, p, args: ADetailerArgs):
+        script_runner = copy(p.scripts)
+        script_args = self.script_args_copy(p.script_args)
+
+        ad_only_seleted_scripts = opts.data.get("ad_only_seleted_scripts", True)
+        if not ad_only_seleted_scripts:
+            return script_runner, script_args
+
+        ad_script_names = opts.data.get("ad_script_names", SCRIPT_DEFAULT)
+        script_names_set = {
+            name
+            for script_name in ad_script_names.split(",")
+            for name in (script_name, script_name.strip())
+        }
+
+        if args.ad_controlnet_model != "None":
+            script_names_set.add("controlnet")
+
+        filtered_alwayson = []
+        for script_object in script_runner.alwayson_scripts:
+            filepath = script_object.filename
+            filename = Path(filepath).stem
+            if filename in script_names_set:
+                filtered_alwayson.append(script_object)
+
+        script_runner.alwayson_scripts = filtered_alwayson
+        return script_runner, script_args
+
+    def disable_controlnet_units(
+        self, script_args: list[Any] | tuple[Any, ...]
+    ) -> None:
+        for obj in script_args:
+            if "controlnet" in obj.__class__.__name__.lower():
+                if hasattr(obj, "enabled"):
+                    obj.enabled = False
+                if hasattr(obj, "input_mode"):
+                    obj.input_mode = getattr(obj.input_mode, "SIMPLE", "simple")
+
+            elif isinstance(obj, dict) and "module" in obj:
+                obj["enabled"] = False
+
+    def get_i2i_p(self, p, args: ADetailerArgs, image):
+        seed, subseed = self.get_seed(p)
+        width, height = self.get_width_height(p, args)
+        steps = self.get_steps(p, args)
+        cfg_scale = self.get_cfg_scale(p, args)
+        initial_noise_multiplier = self.get_initial_noise_multiplier(p, args)
+        sampler_name = self.get_sampler(p, args)
+        override_settings = self.get_override_settings(p, args)
+
+        version_args = {}
+        if schedulers:
+            version_args.update(self.get_scheduler(p, args))
+
+        i2i = StableDiffusionProcessingImg2Img(
+            init_images=[image],
+            resize_mode=0,
+            denoising_strength=args.ad_denoising_strength,
+            mask=None,
+            mask_blur=args.ad_mask_blur,
+            inpainting_fill=1,
+            inpaint_full_res=args.ad_inpaint_only_masked,
+            inpaint_full_res_padding=args.ad_inpaint_only_masked_padding,
+            inpainting_mask_invert=0,
+            initial_noise_multiplier=initial_noise_multiplier,
+            sd_model=p.sd_model,
+            outpath_samples=p.outpath_samples,
+            outpath_grids=p.outpath_grids,
+            prompt="",  # replace later
+            negative_prompt="",
+            styles=p.styles,
+            seed=seed,
+            subseed=subseed,
+            subseed_strength=p.subseed_strength,
+            seed_resize_from_h=p.seed_resize_from_h,
+            seed_resize_from_w=p.seed_resize_from_w,
+            sampler_name=sampler_name,
+            batch_size=1,
+            n_iter=1,
+            steps=steps,
+            cfg_scale=cfg_scale,
+            width=width,
+            height=height,
+            restore_faces=args.ad_restore_face,
+            tiling=p.tiling,
+            extra_generation_params=copy_extra_params(p.extra_generation_params),
+            do_not_save_samples=True,
+            do_not_save_grid=True,
+            override_settings=override_settings,
+            **version_args,
+        )
+
+        i2i.cached_c = [None, None]
+        i2i.cached_uc = [None, None]
+        i2i.scripts, i2i.script_args = self.script_filter(p, args)
+        i2i._ad_disabled = True
+        i2i._ad_inner = True
+
+        if args.ad_controlnet_model != "Passthrough" and controlnet_type != "forge":
+            self.disable_controlnet_units(i2i.script_args)
+
+        if args.ad_controlnet_model not in ["None", "Passthrough"]:
+            self.update_controlnet_args(i2i, args)
+        elif args.ad_controlnet_model == "None":
+            i2i.control_net_enabled = False
+
+        return i2i
+
+    def save_image(self, p, image, *, condition: str, suffix: str) -> None:
+        i = get_i(p)
+        if p.all_prompts:
+            i %= len(p.all_prompts)
+            save_prompt = p.all_prompts[i]
+        else:
+            save_prompt = p.prompt
+        seed, _ = self.get_seed(p)
+
+        if opts.data.get(condition, False):
+            images.save_image(
+                image=image,
+                path=p.outpath_samples,
+                basename="",
+                seed=seed,
+                prompt=save_prompt,
+                extension=opts.samples_format,
+                info=self.infotext(p),
+                p=p,
+                suffix=suffix,
+            )
+
+    def get_ad_model(self, name: str):
+        if name not in model_mapping:
+            msg = f"[-] ADetailer: Model {name!r} not found. Available models: {list(model_mapping.keys())}"
+            raise ValueError(msg)
+        return model_mapping[name]
+
+    def sort_bboxes(self, pred: PredictOutput) -> PredictOutput:
+        sortby = opts.data.get("ad_bbox_sortby", BBOX_SORTBY[0])
+        sortby_idx = BBOX_SORTBY.index(sortby)
+        return sort_bboxes(pred, sortby_idx)
+
+    def pred_preprocessing(self, p, pred: PredictOutput, args: ADetailerArgs):
+        pred = filter_by_ratio(
+            pred, low=args.ad_mask_min_ratio, high=args.ad_mask_max_ratio
+        )
+        pred = filter_k_largest(pred, k=args.ad_mask_k_largest)
+        pred = self.sort_bboxes(pred)
+        masks = mask_preprocess(
+            pred.masks,
+            kernel=args.ad_dilate_erode,
+            x_offset=args.ad_x_offset,
+            y_offset=args.ad_y_offset,
+            merge_invert=args.ad_mask_merge_invert,
+        )
+
+        if is_img2img_inpaint(p) and not is_inpaint_only_masked(p):
+            image_mask = self.get_image_mask(p)
+            masks = self.inpaint_mask_filter(image_mask, masks)
+        return masks
+
+    @staticmethod
+    def i2i_prompts_replace(
+        i2i, prompts: list[str], negative_prompts: list[str], j: int
+    ) -> None:
+        i1 = min(j, len(prompts) - 1)
+        i2 = min(j, len(negative_prompts) - 1)
+        prompt = prompts[i1]
+        negative_prompt = negative_prompts[i2]
+        i2i.prompt = prompt
+        i2i.negative_prompt = negative_prompt
+
+    @staticmethod
+    def compare_prompt(p, extra_params: dict[str, Any], processed, n: int = 0):
+        if not hasattr(p, "_ad_extra_params_result"):
+            p._ad_extra_params_result = {}
+
+        pt = "ADetailer prompt" + suffix(n)
+        if pt in extra_params and extra_params[pt] != processed.all_prompts[0]:
+            print(
+                f"[-] ADetailer: applied {ordinal(n + 1)} ad_prompt: {processed.all_prompts[0]!r}"
+            )
+            p._ad_extra_params_result[pt] = processed.all_prompts[0]
+
+        ng = "ADetailer negative prompt" + suffix(n)
+        if ng in extra_params and extra_params[ng] != processed.all_negative_prompts[0]:
+            print(
+                f"[-] ADetailer: applied {ordinal(n + 1)} ad_negative_prompt: {processed.all_negative_prompts[0]!r}"
+            )
+            p._ad_extra_params_result[ng] = processed.all_negative_prompts[0]
+
+    @staticmethod
+    def get_i2i_init_image(p, pp):
+        if getattr(p, "_ad_skip_img2img", False):
+            return p.init_images[0]
+        return pp.image
+
+    @staticmethod
+    def get_each_tap_seed(seed: int, i: int):
+        use_same_seed = shared.opts.data.get("ad_same_seed_for_each_tap", False)
+        return seed if use_same_seed else seed + i
+
+    @staticmethod
+    def inpaint_mask_filter(
+        img2img_mask: Image.Image, ad_mask: list[Image.Image]
+    ) -> list[Image.Image]:
+        if ad_mask and img2img_mask.size != ad_mask[0].size:
+            img2img_mask = img2img_mask.resize(ad_mask[0].size, resample=images.LANCZOS)
+        return [mask for mask in ad_mask if has_intersection(img2img_mask, mask)]
+
+    @staticmethod
+    def get_image_mask(p) -> Image.Image:
+        mask = p.image_mask
+        if getattr(p, "inpainting_mask_invert", False):
+            mask = ImageChops.invert(mask)
+        mask = create_binary_mask(mask)
+
+        if getattr(p, "_ad_skip_img2img", False):
+            if hasattr(p, "init_images") and p.init_images:
+                width, height = p.init_images[0].size
+            else:
+                msg = "[-] ADetailer: no init_images."
+                raise RuntimeError(msg)
+        else:
+            width, height = p.width, p.height
+        return images.resize_image(p.resize_mode, mask, width, height)
+
+    @rich_traceback
+    def process(self, p, *args_):
+        if getattr(p, "_ad_disabled", False):
+            return
+
+        if is_img2img_inpaint(p) and is_all_black(self.get_image_mask(p)):
+            p._ad_disabled = True
+            msg = (
+                "[-] ADetailer: img2img inpainting with no mask -- adetailer disabled."
+            )
+            print(msg)
+            return
+
+        if not self.is_ad_enabled(*args_):
+            p._ad_disabled = True
+            return
+
+        self.set_skip_img2img(p, *args_)
+        if getattr(p, "_ad_disabled", False):
+            # case when img2img inpainting with skip img2img
+            return
+
+        arg_list = self.get_args(p, *args_)
+
+        if hasattr(p, "_ad_xyz_prompt_sr"):
+            replaced_positive_prompt, replaced_negative_prompt = self.get_prompt(
+                p, arg_list[0]
+            )
+            arg_list[0].ad_prompt = replaced_positive_prompt[0]
+            arg_list[0].ad_negative_prompt = replaced_negative_prompt[0]
+
+        extra_params = self.extra_params(arg_list)
+        p.extra_generation_params.update(extra_params)
+
+    def _postprocess_image_inner(
+        self, p, pp, args: ADetailerArgs, *, n: int = 0
+    ) -> bool:
+        """
+        Returns
+        -------
+            bool
+
+            `True` if image was processed, `False` otherwise.
+        """
+        if state.interrupted or state.skipped:
+            return False
+
+        i = get_i(p)
+
+        i2i = self.get_i2i_p(p, args, pp.image)
+        seed, subseed = self.get_seed(p)
+        ad_prompts, ad_negatives = self.get_prompt(p, args)
+
+        is_mediapipe = args.ad_model.lower().startswith("mediapipe")
+
+        kwargs = {}
+        if is_mediapipe:
+            predictor = mediapipe_predict
+            ad_model = args.ad_model
+        else:
+            predictor = ultralytics_predict
+            ad_model = self.get_ad_model(args.ad_model)
+            kwargs["device"] = self.ultralytics_device
+            kwargs["classes"] = args.ad_model_classes
+
+        with change_torch_load():
+            pred = predictor(ad_model, pp.image, args.ad_confidence, **kwargs)
+
+        if pred.preview is None:
+            print(
+                f"[-] ADetailer: nothing detected on image {i + 1} with {ordinal(n + 1)} settings."
+            )
+            return False
+
+        masks = self.pred_preprocessing(p, pred, args)
+        shared.state.assign_current_image(pred.preview)
+
+        self.save_image(
+            p,
+            pred.preview,
+            condition="ad_save_previews",
+            suffix="-ad-preview" + suffix(n, "-"),
+        )
+
+        steps = len(masks)
+        processed = None
+        state.job_count += steps
+
+        if is_mediapipe:
+            print(f"mediapipe: {steps} detected.")
+
+        p2 = copy(i2i)
+        for j in range(steps):
+            p2.image_mask = masks[j]
+            p2.init_images[0] = ensure_pil_image(p2.init_images[0], "RGB")
+            self.i2i_prompts_replace(p2, ad_prompts, ad_negatives, j)
+
+            if re.match(r"^\s*\[SKIP\]\s*$", p2.prompt):
+                continue
+
+            p2.seed = self.get_each_tap_seed(seed, j)
+            p2.subseed = self.get_each_tap_seed(subseed, j)
+
+            try:
+                processed = process_images(p2)
+            except NansException as e:
+                msg = f"[-] ADetailer: 'NansException' occurred with {ordinal(n + 1)} settings.\n{e}"
+                print(msg, file=sys.stderr)
+                continue
+            finally:
+                p2.close()
+
+            self.compare_prompt(p, p.extra_generation_params, processed, n=n)
+            p2 = copy(i2i)
+            p2.init_images = [processed.images[0]]
+
+        if processed is not None:
+            pp.image = processed.images[0]
+            return True
+
+        return False
+
+    @rich_traceback
+    def postprocess_image(self, p, pp, *args_):
+        if getattr(p, "_ad_disabled", False) or not self.is_ad_enabled(*args_):
+            return
+
+        pp.image = self.get_i2i_init_image(p, pp)
+        pp.image = ensure_pil_image(pp.image, "RGB")
+        init_image = copy(pp.image)
+        arg_list = self.get_args(p, *args_)
+        params_txt_content = self.read_params_txt()
+
+        if need_call_postprocess(p):
+            dummy = Processed(p, [], p.seed, "")
+            with preseve_prompts(p):
+                p.scripts.postprocess(copy(p), dummy)
+
+        is_processed = False
+        with CNHijackRestore(), pause_total_tqdm(), cn_allow_script_control():
+            for n, args in enumerate(arg_list):
+                if args.ad_model == "None":
+                    continue
+                is_processed |= self._postprocess_image_inner(p, pp, args, n=n)
+
+        if is_processed and not getattr(p, "_ad_skip_img2img", False):
+            self.save_image(
+                p, init_image, condition="ad_save_images_before", suffix="-ad-before"
+            )
+
+        if need_call_process(p):
+            with preseve_prompts(p):
+                copy_p = copy(p)
+                if hasattr(p.scripts, "before_process"):
+                    p.scripts.before_process(copy_p)
+                p.scripts.process(copy_p)
+
+        self.write_params_txt(params_txt_content)
+
+        if hasattr(p, "_ad_extra_params_result"):
+            p.extra_generation_params.update(p._ad_extra_params_result)
+
+
+def on_after_component(component, **_kwargs):
+    global txt2img_submit_button, img2img_submit_button
+    if getattr(component, "elem_id", None) == "txt2img_generate":
+        txt2img_submit_button = component
+        return
+
+    if getattr(component, "elem_id", None) == "img2img_generate":
+        img2img_submit_button = component
+
+
+def on_ui_settings():
+    section = ("ADetailer", AFTER_DETAILER)
+    shared.opts.add_option(
+        "ad_max_models",
+        shared.OptionInfo(
+            default=2,
+            label="Max models",
+            component=gr.Slider,
+            component_args={"minimum": 1, "maximum": 10, "step": 1},
+            section=section,
+        ),
+    )
+
+    shared.opts.add_option(
+        "ad_extra_models_dir",
+        shared.OptionInfo(
+            default="",
+            label="Extra path to scan adetailer models",
+            component=gr.Textbox,
+            section=section,
+        ),
+    )
+
+    shared.opts.add_option(
+        "ad_save_previews",
+        shared.OptionInfo(False, "Save mask previews", section=section),
+    )
+
+    shared.opts.add_option(
+        "ad_save_images_before",
+        shared.OptionInfo(False, "Save images before ADetailer", section=section),
+    )
+
+    shared.opts.add_option(
+        "ad_only_seleted_scripts",
+        shared.OptionInfo(
+            True, "Apply only selected scripts to ADetailer", section=section
+        ),
+    )
+
+    textbox_args = {
+        "placeholder": "comma-separated list of script names",
+        "interactive": True,
+    }
+
+    shared.opts.add_option(
+        "ad_script_names",
+        shared.OptionInfo(
+            default=SCRIPT_DEFAULT,
+            label="Script names to apply to ADetailer (separated by comma)",
+            component=gr.Textbox,
+            component_args=textbox_args,
+            section=section,
+        ),
+    )
+
+    shared.opts.add_option(
+        "ad_bbox_sortby",
+        shared.OptionInfo(
+            default="None",
+            label="Sort bounding boxes by",
+            component=gr.Radio,
+            component_args={"choices": BBOX_SORTBY},
+            section=section,
+        ),
+    )
+
+    shared.opts.add_option(
+        "ad_same_seed_for_each_tap",
+        shared.OptionInfo(
+            False, "Use same seed for each tab in adetailer", section=section
+        ),
+    )
+
+
+# xyz_grid
+
+
+class PromptSR(NamedTuple):
+    s: str
+    r: str
+
+
+def set_value(p, x: Any, xs: Any, *, field: str):
+    if not hasattr(p, "_ad_xyz"):
+        p._ad_xyz = {}
+    p._ad_xyz[field] = x
+
+
+def search_and_replace_prompt(p, x: Any, xs: Any, replace_in_main_prompt: bool):
+    if replace_in_main_prompt:
+        p.prompt = p.prompt.replace(xs[0], x)
+        p.negative_prompt = p.negative_prompt.replace(xs[0], x)
+
+    if not hasattr(p, "_ad_xyz_prompt_sr"):
+        p._ad_xyz_prompt_sr = []
+    p._ad_xyz_prompt_sr.append(PromptSR(s=xs[0], r=x))
+
+
+def make_axis_on_xyz_grid():
+    xyz_grid = None
+    for script in scripts.scripts_data:
+        if script.script_class.__module__ == "xyz_grid.py":
+            xyz_grid = script.module
+            break
+
+    if xyz_grid is None:
+        return
+
+    model_list = ["None", *model_mapping.keys()]
+    samplers = [sampler.name for sampler in all_samplers]
+
+    axis = [
+        xyz_grid.AxisOption(
+            "[ADetailer] ADetailer model 1st",
+            str,
+            partial(set_value, field="ad_model"),
+            choices=lambda: model_list,
+        ),
+        xyz_grid.AxisOption(
+            "[ADetailer] ADetailer prompt 1st",
+            str,
+            partial(set_value, field="ad_prompt"),
+        ),
+        xyz_grid.AxisOption(
+            "[ADetailer] ADetailer negative prompt 1st",
+            str,
+            partial(set_value, field="ad_negative_prompt"),
+        ),
+        xyz_grid.AxisOption(
+            "[ADetailer] Prompt S/R (AD 1st)",
+            str,
+            partial(search_and_replace_prompt, replace_in_main_prompt=False),
+        ),
+        xyz_grid.AxisOption(
+            "[ADetailer] Prompt S/R (AD 1st and main prompt)",
+            str,
+            partial(search_and_replace_prompt, replace_in_main_prompt=True),
+        ),
+        xyz_grid.AxisOption(
+            "[ADetailer] Mask erosion / dilation 1st",
+            int,
+            partial(set_value, field="ad_dilate_erode"),
+        ),
+        xyz_grid.AxisOption(
+            "[ADetailer] Inpaint denoising strength 1st",
+            float,
+            partial(set_value, field="ad_denoising_strength"),
+        ),
+        xyz_grid.AxisOption(
+            "[ADetailer] Inpaint only masked 1st",
+            str,
+            partial(set_value, field="ad_inpaint_only_masked"),
+            choices=lambda: ["True", "False"],
+        ),
+        xyz_grid.AxisOption(
+            "[ADetailer] Inpaint only masked padding 1st",
+            int,
+            partial(set_value, field="ad_inpaint_only_masked_padding"),
+        ),
+        xyz_grid.AxisOption(
+            "[ADetailer] ADetailer sampler 1st",
+            str,
+            partial(set_value, field="ad_sampler"),
+            choices=lambda: samplers,
+        ),
+        xyz_grid.AxisOption(
+            "[ADetailer] ControlNet model 1st",
+            str,
+            partial(set_value, field="ad_controlnet_model"),
+            choices=lambda: ["None", "Passthrough", *get_cn_models()],
+        ),
+    ]
+
+    if not any(x.label.startswith("[ADetailer]") for x in xyz_grid.axis_options):
+        xyz_grid.axis_options.extend(axis)
+
+
+def on_before_ui():
+    try:
+        make_axis_on_xyz_grid()
+    except Exception:
+        error = traceback.format_exc()
+        print(
+            f"[-] ADetailer: xyz_grid error:\n{error}",
+            file=sys.stderr,
+        )
+
+
+# api
+
+
+def add_api_endpoints(_: gr.Blocks, app: FastAPI):
+    @app.get("/adetailer/v1/version")
+    async def version():
+        return {"version": __version__}
+
+    @app.get("/adetailer/v1/schema")
+    async def schema():
+        if hasattr(ADetailerArgs, "model_json_schema"):
+            return ADetailerArgs.model_json_schema()
+        return ADetailerArgs.schema()
+
+    @app.get("/adetailer/v1/ad_model")
+    async def ad_model():
+        return {"ad_model": list(model_mapping)}
+
+
+script_callbacks.on_ui_settings(on_ui_settings)
+script_callbacks.on_after_component(on_after_component)
+script_callbacks.on_app_started(add_api_endpoints)
+script_callbacks.on_before_ui(on_before_ui)
```

### Comparing `adetailer-24.4.1/tests/test_mask.py` & `adetailer-24.4.2/tests/test_mask.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,236 +1,236 @@
-import cv2
-import numpy as np
-import pytest
-from PIL import Image, ImageDraw
-
-from adetailer.mask import (
-    bbox_area,
-    dilate_erode,
-    has_intersection,
-    is_all_black,
-    mask_invert,
-    mask_merge,
-    offset,
-)
-
-
-def test_dilate_positive_value():
-    img = Image.new("L", (10, 10), color="black")
-    draw = ImageDraw.Draw(img)
-    draw.rectangle((3, 3, 5, 5), fill="white")
-    value = 3
-
-    result = dilate_erode(img, value)
-
-    assert isinstance(result, Image.Image)
-    assert result.size == (10, 10)
-
-    expect = np.array(
-        [
-            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
-            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
-            [0, 0, 255, 255, 255, 255, 255, 0, 0, 0],
-            [0, 0, 255, 255, 255, 255, 255, 0, 0, 0],
-            [0, 0, 255, 255, 255, 255, 255, 0, 0, 0],
-            [0, 0, 255, 255, 255, 255, 255, 0, 0, 0],
-            [0, 0, 255, 255, 255, 255, 255, 0, 0, 0],
-            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
-            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
-            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
-        ],
-        dtype=np.uint8,
-    )
-    assert np.array_equal(np.array(result), expect)
-
-
-def test_offset():
-    img = Image.new("L", (10, 10), color="black")
-    draw = ImageDraw.Draw(img)
-    draw.rectangle((4, 4, 5, 5), fill="white")
-
-    result = offset(img, x=1, y=2)
-
-    assert isinstance(result, Image.Image)
-    assert result.size == (10, 10)
-
-    expect = np.array(
-        [
-            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
-            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
-            [0, 0, 0, 0, 0, 255, 255, 0, 0, 0],
-            [0, 0, 0, 0, 0, 255, 255, 0, 0, 0],
-            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
-            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
-            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
-            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
-            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
-            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
-        ],
-        dtype=np.uint8,
-    )
-    assert np.array_equal(np.array(result), expect)
-
-
-class TestIsAllBlack:
-    def test_is_all_black_1(self):
-        img = Image.new("L", (10, 10), color="black")
-        assert is_all_black(img)
-
-        draw = ImageDraw.Draw(img)
-        draw.rectangle((4, 4, 5, 5), fill="white")
-        assert not is_all_black(img)
-
-    def test_is_all_black_2(self):
-        img = np.zeros((10, 10), dtype=np.uint8)
-        assert is_all_black(img)
-
-        img[4:6, 4:6] = 255
-        assert not is_all_black(img)
-
-    def test_is_all_black_rgb_image_pil(self):
-        img = Image.new("RGB", (10, 10), color="red")
-        assert not is_all_black(img)
-
-        img = Image.new("RGBA", (10, 10), color="red")
-        assert not is_all_black(img)
-
-    def test_is_all_black_rgb_image_numpy(self):
-        img = np.full((10, 10, 4), 127, dtype=np.uint8)
-        with pytest.raises(cv2.error):
-            is_all_black(img)
-
-        img = np.full((4, 10, 10), 0.5, dtype=np.float32)
-        with pytest.raises(cv2.error):
-            is_all_black(img)
-
-
-class TestHasIntersection:
-    def test_has_intersection_1(self):
-        arr1 = np.array(
-            [
-                [0, 0, 0, 0],
-                [0, 0, 0, 0],
-                [0, 0, 0, 0],
-                [0, 0, 0, 0],
-            ],
-            dtype=np.uint8,
-        )
-        arr2 = arr1.copy()
-        assert not has_intersection(arr1, arr2)
-
-    def test_has_intersection_2(self):
-        arr1 = np.array(
-            [
-                [0, 0, 0, 0],
-                [0, 255, 255, 0],
-                [0, 255, 255, 0],
-                [0, 0, 0, 0],
-            ],
-            dtype=np.uint8,
-        )
-        arr2 = np.array(
-            [
-                [0, 0, 0, 0],
-                [0, 0, 0, 0],
-                [0, 0, 255, 255],
-                [0, 0, 255, 255],
-            ],
-            dtype=np.uint8,
-        )
-        assert has_intersection(arr1, arr2)
-
-        arr3 = np.array(
-            [
-                [255, 0, 0, 0],
-                [0, 0, 0, 0],
-                [0, 0, 0, 255],
-                [0, 0, 255, 255],
-            ],
-            dtype=np.uint8,
-        )
-        assert not has_intersection(arr1, arr3)
-
-    def test_has_intersection_3(self):
-        img1 = Image.new("L", (10, 10), color="black")
-        draw1 = ImageDraw.Draw(img1)
-        draw1.rectangle((3, 3, 5, 5), fill="white")
-        img2 = Image.new("L", (10, 10), color="black")
-        draw2 = ImageDraw.Draw(img2)
-        draw2.rectangle((6, 6, 8, 8), fill="white")
-        assert not has_intersection(img1, img2)
-
-        img3 = Image.new("L", (10, 10), color="black")
-        draw3 = ImageDraw.Draw(img3)
-        draw3.rectangle((2, 2, 8, 8), fill="white")
-        assert has_intersection(img1, img3)
-
-    def test_has_intersection_4(self):
-        img1 = Image.new("RGB", (10, 10), color="black")
-        draw1 = ImageDraw.Draw(img1)
-        draw1.rectangle((3, 3, 5, 5), fill="white")
-        img2 = Image.new("RGBA", (10, 10), color="black")
-        draw2 = ImageDraw.Draw(img2)
-        draw2.rectangle((2, 2, 8, 8), fill="white")
-        assert has_intersection(img1, img2)
-
-    def test_has_intersection_5(self):
-        img1 = Image.new("RGB", (10, 10), color="black")
-        draw1 = ImageDraw.Draw(img1)
-        draw1.rectangle((4, 4, 5, 5), fill="white")
-        img2 = np.full((10, 10, 4), 255, dtype=np.uint8)
-        assert has_intersection(img1, img2)
-
-
-def test_bbox_area():
-    bbox = [0.0, 0.0, 10.0, 10.0]
-    assert bbox_area(bbox) == 100
-
-
-class TestMaskMerge:
-    def test_mask_merge(self):
-        img1 = Image.new("L", (10, 10), color="black")
-        draw1 = ImageDraw.Draw(img1)
-        draw1.rectangle((3, 3, 5, 5), fill="white")
-
-        img2 = Image.new("L", (10, 10), color="black")
-        draw2 = ImageDraw.Draw(img2)
-        draw2.rectangle((6, 6, 8, 8), fill="white")
-
-        merged = mask_merge([img1, img2])
-        assert len(merged) == 1
-
-        expect = Image.new("L", (10, 10), color="black")
-        draw3 = ImageDraw.Draw(expect)
-        draw3.rectangle((3, 3, 5, 5), fill="white")
-        draw3.rectangle((6, 6, 8, 8), fill="white")
-
-        assert np.array_equal(np.array(merged[0]), np.array(expect))
-
-    def test_merge_mask_different_size(self):
-        img1 = Image.new("L", (10, 10), color="black")
-        draw1 = ImageDraw.Draw(img1)
-        draw1.rectangle((3, 3, 5, 5), fill="white")
-
-        img2 = Image.new("L", (20, 20), color="black")
-        draw2 = ImageDraw.Draw(img2)
-        draw2.rectangle((6, 6, 8, 8), fill="white")
-
-        with pytest.raises(
-            cv2.error, match="-209:Sizes of input arguments do not match"
-        ):
-            mask_merge([img1, img2])
-
-
-def test_mask_invert():
-    img = Image.new("L", (10, 10), color="black")
-    draw = ImageDraw.Draw(img)
-    draw.rectangle((3, 3, 5, 5), fill="white")
-
-    inverted = mask_invert([img])
-    assert len(inverted) == 1
-
-    expect = Image.new("L", (10, 10), color="white")
-    draw = ImageDraw.Draw(expect)
-    draw.rectangle((3, 3, 5, 5), fill="black")
-
-    assert np.array_equal(np.array(inverted[0]), np.array(expect))
+import cv2
+import numpy as np
+import pytest
+from PIL import Image, ImageDraw
+
+from adetailer.mask import (
+    bbox_area,
+    dilate_erode,
+    has_intersection,
+    is_all_black,
+    mask_invert,
+    mask_merge,
+    offset,
+)
+
+
+def test_dilate_positive_value():
+    img = Image.new("L", (10, 10), color="black")
+    draw = ImageDraw.Draw(img)
+    draw.rectangle((3, 3, 5, 5), fill="white")
+    value = 3
+
+    result = dilate_erode(img, value)
+
+    assert isinstance(result, Image.Image)
+    assert result.size == (10, 10)
+
+    expect = np.array(
+        [
+            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
+            [0, 0, 255, 255, 255, 255, 255, 0, 0, 0],
+            [0, 0, 255, 255, 255, 255, 255, 0, 0, 0],
+            [0, 0, 255, 255, 255, 255, 255, 0, 0, 0],
+            [0, 0, 255, 255, 255, 255, 255, 0, 0, 0],
+            [0, 0, 255, 255, 255, 255, 255, 0, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
+        ],
+        dtype=np.uint8,
+    )
+    assert np.array_equal(np.array(result), expect)
+
+
+def test_offset():
+    img = Image.new("L", (10, 10), color="black")
+    draw = ImageDraw.Draw(img)
+    draw.rectangle((4, 4, 5, 5), fill="white")
+
+    result = offset(img, x=1, y=2)
+
+    assert isinstance(result, Image.Image)
+    assert result.size == (10, 10)
+
+    expect = np.array(
+        [
+            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0, 255, 255, 0, 0, 0],
+            [0, 0, 0, 0, 0, 255, 255, 0, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
+        ],
+        dtype=np.uint8,
+    )
+    assert np.array_equal(np.array(result), expect)
+
+
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
+
+
+def test_mask_invert():
+    img = Image.new("L", (10, 10), color="black")
+    draw = ImageDraw.Draw(img)
+    draw.rectangle((3, 3, 5, 5), fill="white")
+
+    inverted = mask_invert([img])
+    assert len(inverted) == 1
+
+    expect = Image.new("L", (10, 10), color="white")
+    draw = ImageDraw.Draw(expect)
+    draw.rectangle((3, 3, 5, 5), fill="black")
+
+    assert np.array_equal(np.array(inverted[0]), np.array(expect))
```

### Comparing `adetailer-24.4.1/.gitignore` & `adetailer-24.4.2/.gitignore`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,196 +1,196 @@
-# Created by https://www.toptal.com/developers/gitignore/api/python,visualstudiocode
-# Edit at https://www.toptal.com/developers/gitignore?templates=python,visualstudiocode
-
-### Python ###
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-cover/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-.pybuilder/
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-#   For a library or package, you might want to ignore these files since the code is
-#   intended to run in multiple environments; otherwise, check them in:
-# .python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# poetry
-#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
-#   This is especially recommended for binary packages to ensure reproducibility, and is more
-#   commonly ignored for libraries.
-#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
-#poetry.lock
-
-# pdm
-#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
-#pdm.lock
-#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
-#   in version control.
-#   https://pdm.fming.dev/#use-with-ide
-.pdm.toml
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
-
-# pytype static type analyzer
-.pytype/
-
-# Cython debug symbols
-cython_debug/
-
-# PyCharm
-#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
-#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
-#  and can be added to the global gitignore or merged into this file.  For a more nuclear
-#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
-
-### Python Patch ###
-# Poetry local configuration file - https://python-poetry.org/docs/configuration/#local-configuration
-poetry.toml
-
-# ruff
-.ruff_cache/
-
-# LSP config files
-pyrightconfig.json
-
-### VisualStudioCode ###
-.vscode/*
-!.vscode/settings.json
-!.vscode/tasks.json
-!.vscode/launch.json
-!.vscode/extensions.json
-!.vscode/*.code-snippets
-
-# Local History for Visual Studio Code
-.history/
-
-# Built Visual Studio Code Extensions
-*.vsix
-
-### VisualStudioCode Patch ###
-# Ignore all local history of files
-.history
-.ionide
-
-# End of https://www.toptal.com/developers/gitignore/api/python,visualstudiocode
-*.ipynb
+# Created by https://www.toptal.com/developers/gitignore/api/python,visualstudiocode
+# Edit at https://www.toptal.com/developers/gitignore?templates=python,visualstudiocode
+
+### Python ###
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+cover/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+.pybuilder/
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+# .python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# poetry
+#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
+#   This is especially recommended for binary packages to ensure reproducibility, and is more
+#   commonly ignored for libraries.
+#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
+#poetry.lock
+
+# pdm
+#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
+#pdm.lock
+#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
+#   in version control.
+#   https://pdm.fming.dev/#use-with-ide
+.pdm.toml
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+# pytype static type analyzer
+.pytype/
+
+# Cython debug symbols
+cython_debug/
+
+# PyCharm
+#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
+#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
+#  and can be added to the global gitignore or merged into this file.  For a more nuclear
+#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
+#.idea/
+
+### Python Patch ###
+# Poetry local configuration file - https://python-poetry.org/docs/configuration/#local-configuration
+poetry.toml
+
+# ruff
+.ruff_cache/
+
+# LSP config files
+pyrightconfig.json
+
+### VisualStudioCode ###
+.vscode/*
+!.vscode/settings.json
+!.vscode/tasks.json
+!.vscode/launch.json
+!.vscode/extensions.json
+!.vscode/*.code-snippets
+
+# Local History for Visual Studio Code
+.history/
+
+# Built Visual Studio Code Extensions
+*.vsix
+
+### VisualStudioCode Patch ###
+# Ignore all local history of files
+.history
+.ionide
+
+# End of https://www.toptal.com/developers/gitignore/api/python,visualstudiocode
+*.ipynb
```

### Comparing `adetailer-24.4.1/LICENSE.md` & `adetailer-24.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `adetailer-24.4.1/README.md` & `adetailer-24.4.2/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-# ADetailer
-
-ADetailer is an extension for the stable diffusion webui that does automatic masking and inpainting. It is similar to the Detection Detailer.
-
-## Install
-
-You can install it directly from the Extensions tab.
-
-![image](https://i.imgur.com/qaXtoI6.png)
-
-Or
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
-API request example: [wiki/REST-API](https://github.com/Bing-su/adetailer/wiki/REST-API)
-
-`[SEP], [SKIP], [PROMPT]` tokens: [wiki/Advanced](https://github.com/Bing-su/adetailer/wiki/Advanced)
-
-## Media
-
-- 🎥 [どこよりも詳しい After Detailer (adetailer)の使い方 ① 【Stable Diffusion】](https://youtu.be/sF3POwPUWCE)
-- 🎥 [どこよりも詳しい After Detailer (adetailer)の使い方 ② 【Stable Diffusion】](https://youtu.be/urNISRdbIEg)
-
-- 📜 [ADetailer Installation and 5 Usage Methods](https://kindanai.com/en/manual-adetailer/)
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
-Put your [ultralytics](https://github.com/ultralytics/ultralytics) yolo model in `models/adetailer`. The model name should end with `.pt`.
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
-ADetailer is developed and tested using the stable-diffusion 1.5 model, for the latest version of [AUTOMATIC1111/stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) repository only.
-
-## License
-
-ADetailer is a derivative work that uses two AGPL-licensed works (stable-diffusion-webui, ultralytics) and is therefore distributed under the AGPL license.
-
-## See Also
-
-- https://github.com/ototadana/sd-face-editor
-- https://github.com/continue-revolution/sd-webui-segment-anything
-- https://github.com/portu-sim/sd-webui-bmab
+# ADetailer
+
+ADetailer is an extension for the stable diffusion webui that does automatic masking and inpainting. It is similar to the Detection Detailer.
+
+## Install
+
+You can install it directly from the Extensions tab.
+
+![image](https://i.imgur.com/qaXtoI6.png)
+
+Or
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
+- 🎥 [どこよりも詳しい After Detailer (adetailer)の使い方 ① 【Stable Diffusion】](https://youtu.be/sF3POwPUWCE)
+- 🎥 [どこよりも詳しい After Detailer (adetailer)の使い方 ② 【Stable Diffusion】](https://youtu.be/urNISRdbIEg)
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
+
+## See Also
+
+- https://github.com/ototadana/sd-face-editor
+- https://github.com/continue-revolution/sd-webui-segment-anything
+- https://github.com/portu-sim/sd-webui-bmab
```

### Comparing `adetailer-24.4.1/PKG-INFO` & `adetailer-24.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: adetailer
-Version: 24.4.1
+Version: 24.4.2
 Summary: An object detection and auto-mask extension for stable diffusion webui.
 Project-URL: repository, https://github.com/Bing-su/adetailer
 Author-email: dowon <ks2515@naver.com>
 License: AGPL-3.0
 License-File: LICENSE.md
 Keywords: adetailer,stable-diffusion,stable-diffusion-webui,ultralytics
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

