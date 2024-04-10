# Comparing `tmp/llm_toolkit-0.1.4.tar.gz` & `tmp/llm_toolkit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_toolkit-0.1.4.tar", max compression
+gzip compressed data, was "llm_toolkit-0.2.0.tar", max compression
```

## Comparing `llm_toolkit-0.1.4.tar` & `llm_toolkit-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0    10763 2024-04-05 21:23:10.325485 llm_toolkit-0.1.4/LICENSE
--rw-r--r--   0        0        0     8751 2024-04-05 21:23:10.325485 llm_toolkit-0.1.4/README.md
--rw-r--r--   0        0        0      601 2024-04-05 21:24:55.536638 llm_toolkit-0.1.4/llmtune/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/cli/__init__.py
--rw-r--r--   0        0        0     3722 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/cli/toolkit.py
--rw-r--r--   0        0        0        0 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/data/__init__.py
--rw-r--r--   0        0        0     2917 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/data/dataset_generator.py
--rw-r--r--   0        0        0     1477 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/data/ingestor.py
--rw-r--r--   0        0        0        0 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/finetune/__init__.py
--rw-r--r--   0        0        0      176 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/finetune/generics.py
--rw-r--r--   0        0        0     4475 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/finetune/lora.py
--rw-r--r--   0        0        0        0 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/inference/__init__.py
--rw-r--r--   0        0        0      190 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/inference/generics.py
--rw-r--r--   0        0        0     3823 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/inference/lora.py
--rw-r--r--   0        0        0        0 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/pydantic_models/__init__.py
--rw-r--r--   0        0        0     8549 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/pydantic_models/config_model.py
--rw-r--r--   0        0        0        0 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/qa/__init__.py
--rw-r--r--   0        0        0     2550 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/qa/generics.py
--rw-r--r--   0        0        0     5503 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/qa/qa_tests.py
--rw-r--r--   0        0        0        0 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/ui/__init__.py
--rw-r--r--   0        0        0     2149 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/ui/generics.py
--rw-r--r--   0        0        0     5933 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/ui/rich_ui.py
--rw-r--r--   0        0        0        0 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/utils/__init__.py
--rw-r--r--   0        0        0     3338 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/utils/ablation_utils.py
--rw-r--r--   0        0        0     1335 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/utils/rich_print_utils.py
--rw-r--r--   0        0        0     2429 2024-04-05 21:23:10.357484 llm_toolkit-0.1.4/llmtune/utils/save_utils.py
--rw-r--r--   0        0        0     2044 2024-04-05 21:24:55.528638 llm_toolkit-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    10894 1970-01-01 00:00:00.000000 llm_toolkit-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    10763 2024-04-10 14:13:37.411021 llm_toolkit-0.2.0/LICENSE
+-rw-r--r--   0        0        0     9473 2024-04-10 14:13:37.411021 llm_toolkit-0.2.0/README.md
+-rw-r--r--   0        0        0      601 2024-04-10 14:18:50.033213 llm_toolkit-0.2.0/llmtune/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/cli/__init__.py
+-rw-r--r--   0        0        0     4450 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/cli/toolkit.py
+-rw-r--r--   0        0        0      407 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/constants/files.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/data/__init__.py
+-rw-r--r--   0        0        0     2917 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/data/dataset_generator.py
+-rw-r--r--   0        0        0     1905 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/data/ingestor.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/finetune/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/finetune/generics.py
+-rw-r--r--   0        0        0     3458 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/finetune/lora.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/inference/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/inference/generics.py
+-rw-r--r--   0        0        0     3570 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/inference/lora.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/pydantic_models/__init__.py
+-rw-r--r--   0        0        0    11642 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/pydantic_models/config_model.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/qa/__init__.py
+-rw-r--r--   0        0        0     2550 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/qa/generics.py
+-rw-r--r--   0        0        0     5503 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/qa/qa_tests.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/ui/__init__.py
+-rw-r--r--   0        0        0     2149 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/ui/generics.py
+-rw-r--r--   0        0        0     6098 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/ui/rich_ui.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/utils/__init__.py
+-rw-r--r--   0        0        0     3338 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/utils/ablation_utils.py
+-rw-r--r--   0        0        0     1335 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/utils/rich_print_utils.py
+-rw-r--r--   0        0        0     2821 2024-04-10 14:13:37.447021 llm_toolkit-0.2.0/llmtune/utils/save_utils.py
+-rw-r--r--   0        0        0     2044 2024-04-10 14:18:50.033213 llm_toolkit-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11616 1970-01-01 00:00:00.000000 llm_toolkit-0.2.0/PKG-INFO
```

### Comparing `llm_toolkit-0.1.4/LICENSE` & `llm_toolkit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.4/README.md` & `llm_toolkit-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,46 +9,76 @@
 LLM Finetuning toolkit is a config-based CLI tool for launching a series of LLM finetuning experiments on your data and gathering their results. From one single `yaml` config file, control all elements of a typical experimentation pipeline - **prompts**, **open-source LLMs**, **optimization strategy** and **LLM testing**.
 
 <p align="center">
 <img src="https://github.com/georgian-io/LLM-Finetuning-Toolkit/blob/main/assets/overview_diagram.png?raw=true" width="900" />
 </p>
 
 ## Installation
+
 ### pipx (recommended)
+
 pipx installs the package and depdencies in a seperate virtual environment
+
 ```shell
 pipx install llm-toolkit
 ```
 
 ### pip
+
 ```shell
 pip install llm-toolkit
 ```
 
-
 ## Quick Start
 
 This guide contains 3 stages that will enable you to get the most out of this toolkit!
 
 - **Basic**: Run your first LLM fine-tuning experiment
-- **Intermediate**: Run a custom experiment by changing the componenets of the YAML configuration file
+- **Intermediate**: Run a custom experiment by changing the components of the YAML configuration file
 - **Advanced**: Launch series of fine-tuning experiments across different prompt templates, LLMs, optimization techniques -- all through **one** YAML configuration file
 
 ### Basic
 
-```python
-   llmtune --config-path ./config.yml
+```shell
+   llmtune generate config
+   llmtune run --config-path ./config.yml
 ```
 
-This command initiates the fine-tuning process using the settings specified in the default YAML configuration file `config.yaml`.
+The first command generates a helpful starter `config.yml` file and saves in the current working directory. This is provided to users to quickly get started and as a base for further modification.
+
+Then the second command initiates the fine-tuning process using the settings specified in the default YAML configuration file `config.yaml`.
 
 ### Intermediate
 
 The configuration file is the central piece that defines the behavior of the toolkit. It is written in YAML format and consists of several sections that control different aspects of the process, such as data ingestion, model definition, training, inference, and quality assurance. We highlight some of the critical sections.
 
+#### Flash Attention 2
+
+To enable Flash-attention for [supported models](https://huggingface.co/docs/transformers/perf_infer_gpu_one#flashattention-2). First install `flash-attn`:
+
+**pipx**
+
+```shell
+pipx inject llm-toolkit flash-attn --pip-args=--no-build-isolation
+```
+
+**pip**
+
+```
+pip install flash-attn --no-build-isolation
+```
+
+Then, add to config file.
+
+```yaml
+model:
+  torch_dtype: "bfloat16" # or "float16" if using older GPU
+  attn_implementation: "flash_attention_2"
+```
+
 #### Data Ingestion
 
 An example of what the data ingestion may look like:
 
 ```yaml
 data:
   file_type: "huggingface"
@@ -243,49 +273,47 @@
 
 ```shell
    # CPU
    docker run -it llm-toolkit
    # GPU
    docker run -it --gpus all llm-toolkit
 ```
+
 </details>
 
 <details>
 <summary>Poetry (recommended)</summary>
 
 See poetry documentation page for poetry [installation instructions](https://python-poetry.org/docs/#installation)
 
 ```shell
    poetry install
 ```
+
 </details>
 <details>
 <summary>pip</summary>
 We recommend using a virtual environment like `venv` or `conda` for installation
 
 ```shell
    pip install -e .
 ```
+
 </details>
 </details>
 
-
-
 ### Checklist Before Pull Request (Optional)
 
 1. Use `ruff check --fix` to check and fix lint errors
 2. Use `ruff format` to apply formatting
 
 NOTE: Ruff linting and formatting checks are done when PR is raised via Git Action. Before raising a PR, it is a good practice to check and fix lint errors, as well as apply formatting.
 
-
 ### Releasing
 
-
-To manually release a PyPI package, please run: 
+To manually release a PyPI package, please run:
 
 ```shell
    make build-release
 ```
 
 Note: Make sure you have pypi token for this [PyPI repo](https://pypi.org/project/llm-toolkit/).
-
```

### Comparing `llm_toolkit-0.1.4/llmtune/__init__.py` & `llm_toolkit-0.2.0/llmtune/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.4"
+__version__ = "0.2.0"
```

### Comparing `llm_toolkit-0.1.4/llmtune/cli/toolkit.py` & `llm_toolkit-0.2.0/llmtune/cli/toolkit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,58 @@
 import logging
-from os import listdir
-from os.path import exists, join
+import shutil
+from pathlib import Path
 
 import torch
+import transformers
 import typer
 import yaml
 from pydantic import ValidationError
-from transformers import utils as hf_utils
+from typing_extensions import Annotated
 
+import llmtune
+from llmtune.constants.files import EXAMPLE_CONFIG_FNAME
 from llmtune.data.dataset_generator import DatasetGenerator
 from llmtune.finetune.lora import LoRAFinetune
 from llmtune.inference.lora import LoRAInference
 from llmtune.pydantic_models.config_model import Config
 from llmtune.ui.rich_ui import RichUI
 from llmtune.utils.ablation_utils import generate_permutations
 from llmtune.utils.save_utils import DirectoryHelper
 
 
-hf_utils.logging.set_verbosity_error()
+transformers.logging.set_verbosity(transformers.logging.CRITICAL)
 torch._logging.set_logs(all=logging.CRITICAL)
+logging.captureWarnings(True)
 
 
 app = typer.Typer()
+generate_app = typer.Typer()
 
+app.add_typer(
+    generate_app,
+    name="generate",
+    help="Generate various artefacts, such as config files",
+)
 
-def run_one_experiment(config: Config, config_path: str) -> None:
+
+def run_one_experiment(config: Config, config_path: Path) -> None:
     dir_helper = DirectoryHelper(config_path, config)
 
     # Loading Data -------------------------------
     RichUI.before_dataset_creation()
 
     with RichUI.during_dataset_creation("Injecting Values into Prompt", "monkey"):
         dataset_generator = DatasetGenerator(**config.data.model_dump())
 
     _ = dataset_generator.train_columns
     test_column = dataset_generator.test_column
 
     dataset_path = dir_helper.save_paths.dataset
-    if not exists(dataset_path):
+    if not dataset_path.exists():
         train, test = dataset_generator.get_dataset()
         dataset_generator.save_dataset(dataset_path)
     else:
         RichUI.dataset_found(dataset_path)
         train, test = dataset_generator.load_dataset_from_pickle(dataset_path)
 
     RichUI.dataset_display_one_example(train[0], test[0])
@@ -49,65 +60,78 @@
 
     # Loading Model -------------------------------
     RichUI.before_finetune()
 
     weights_path = dir_helper.save_paths.weights
 
     # model_loader = ModelLoader(config, console, dir_helper)
-    if not exists(weights_path) or not listdir(weights_path):
+    if not weights_path.exists() or not any(weights_path.iterdir()):
         finetuner = LoRAFinetune(config, dir_helper)
         with RichUI.during_finetune():
             finetuner.finetune(train)
         finetuner.save_model()
         RichUI.after_finetune()
     else:
         RichUI.finetune_found(weights_path)
 
     # Inference -------------------------------
     RichUI.before_inference()
     results_path = dir_helper.save_paths.results
-    results_file_path = join(dir_helper.save_paths.results, "results.csv")
-    if not exists(results_path) or exists(results_file_path):
+    results_file_path = dir_helper.save_paths.results_file
+    if not results_file_path.exists():
         inference_runner = LoRAInference(test, test_column, config, dir_helper)
         inference_runner.infer_all()
         RichUI.after_inference(results_path)
     else:
-        RichUI.inference_found(results_path)
+        RichUI.results_found(results_path)
 
     # QA -------------------------------
     # RichUI.before_qa()
     # qa_path = dir_helper.save_paths.qa
     # if not exists(qa_path) or not listdir(qa_path):
     #     # TODO: Instantiate unit test classes
     #     # TODO: Load results.csv
     #     # TODO: Run Unit Tests
     #     # TODO: Save Unit Test Results
     #     pass
 
 
-@app.command()
-def run(config_path: str = "./config.yml") -> None:
+@app.command("run")
+def run(config_path: Annotated[str, typer.Argument(help="Path of the config yaml file")] = "./config.yml") -> None:
+    """Run the entire exmperiment pipeline"""
     # Load YAML config
-    with open(config_path, "r") as file:
+    with Path(config_path).open("r") as file:
         config = yaml.safe_load(file)
         configs = (
             generate_permutations(config, Config) if config.get("ablation", {}).get("use_ablate", False) else [config]
         )
     for config in configs:
         # validate data with pydantic
         try:
             config = Config(**config)
         except ValidationError as e:
             print(e.json())
 
         dir_helper = DirectoryHelper(config_path, config)
 
         # Reload config from saved config
-        with open(join(dir_helper.save_paths.config, "config.yml"), "r") as file:
+        with dir_helper.save_paths.config_file.open("r") as file:
             config = yaml.safe_load(file)
             config = Config(**config)
 
         run_one_experiment(config, config_path)
 
 
+@generate_app.command("config")
+def generate_config():
+    """
+    Generate an example `config.yml` file in current directory
+    """
+    module_path = Path(llmtune.__file__).parent
+    example_config_path = module_path.parent / EXAMPLE_CONFIG_FNAME
+    destination = Path.cwd()
+    shutil.copy(example_config_path, destination)
+    RichUI.generate_config(EXAMPLE_CONFIG_FNAME)
+
+
 def cli():
     app()
```

### Comparing `llm_toolkit-0.1.4/llmtune/data/dataset_generator.py` & `llm_toolkit-0.2.0/llmtune/data/dataset_generator.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.4/llmtune/data/ingestor.py` & `llm_toolkit-0.2.0/llmtune/data/ingestor.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 import ijson
 from datasets import Dataset, concatenate_datasets, load_dataset
 
 
 def get_ingestor(data_type: str):
     if data_type == "json":
         return JsonIngestor
+    elif data_type == "jsonl":
+        return JsonlIngestor
     elif data_type == "csv":
         return CsvIngestor
     elif data_type == "huggingface":
         return HuggingfaceIngestor
     else:
-        raise ValueError(f"'type' must be one of 'json', 'csv', or 'huggingface', you have {data_type}")
+        raise ValueError(f"'type' must be one of 'json', 'jsonl', 'csv', or 'huggingface', you have {data_type}")
 
 
 class Ingestor(ABC):
     @abstractmethod
     def to_dataset(self) -> Dataset:
         pass
 
@@ -31,14 +33,27 @@
             for item in ijson.items(f, "item"):
                 yield item
 
     def to_dataset(self) -> Dataset:
         return Dataset.from_generator(self._json_generator)
 
 
+class JsonlIngestor(Ingestor):
+    def __init__(self, path: str):
+        self.path = path
+
+    def _jsonl_generator(self):
+        with open(self.path, "rb") as f:
+            for item in ijson.items(f, "", multiple_values=True):
+                yield item
+
+    def to_dataset(self) -> Dataset:
+        return Dataset.from_generator(self._jsonl_generator)
+
+
 class CsvIngestor(Ingestor):
     def __init__(self, path: str):
         self.path = path
 
     def _csv_generator(self):
         with open(self.path) as csvfile:
             reader = csv.DictReader(csvfile)
```

### Comparing `llm_toolkit-0.1.4/llmtune/inference/lora.py` & `llm_toolkit-0.2.0/llmtune/inference/lora.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,32 +36,23 @@
         self.model, self.tokenizer = self._get_merged_model(dir_helper.save_paths.weights)
 
     def _get_merged_model(self, weights_path: str):
         # purge VRAM
         torch.cuda.empty_cache()
 
         # Load from path
-        dtype = (
-            torch.float16
-            if self.config.training.training_args.fp16
-            else (torch.bfloat16 if self.config.training.training_args.bf16 else torch.float32)
-        )
 
         self.model = AutoPeftModelForCausalLM.from_pretrained(
             weights_path,
-            torch_dtype=dtype,
+            torch_dtype=self.config.model.casted_torch_dtype,
+            quantization_config=BitsAndBytesConfig(**self.config.model.bitsandbytes.model_dump()),
             device_map=self.device_map,
-            quantization_config=(BitsAndBytesConfig(**self.config.model.bitsandbytes.model_dump())),
+            attn_implementation=self.config.model.attn_implementation,
         )
 
-        """TODO: figure out multi-gpu
-        if self.config.accelerate:
-            self.model = self.accelerator.prepare(self.model)
-        """
-
         model = self.model.merge_and_unload()
 
         tokenizer = AutoTokenizer.from_pretrained(self._weights_path, device_map=self.device_map)
 
         return model, tokenizer
 
     def infer_all(self):
```

### Comparing `llm_toolkit-0.1.4/llmtune/pydantic_models/config_model.py` & `llm_toolkit-0.2.0/llmtune/pydantic_models/config_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class QaConfig(BaseModel):
     llm_tests: Optional[List[str]] = Field([], description="list of tests that needs to be connected")
 
 
 class DataConfig(BaseModel):
-    file_type: Literal["json", "csv", "huggingface"] = Field(None, description="File type")
+    file_type: Literal["json", "jsonl", "csv", "huggingface"] = Field(None, description="File type")
     path: Union[FilePath, HfModelPath] = Field(None, description="Path to the file or HuggingFace model")
     prompt: str = Field(None, description="Prompt for the model. Use {} brackets for column name")
     prompt_stub: str = Field(
         None,
         description="Stub for the prompt; this is injected during training. Use {} brackets for column name",
     )
     train_size: Optional[Union[float, int]] = Field(
@@ -73,15 +73,21 @@
 
 class ModelConfig(BaseModel):
     hf_model_ckpt: Optional[str] = Field(
         "NousResearch/Llama-2-7b-hf",
         description="Path to the model (huggingface repo or local path)",
     )
     device_map: Optional[str] = Field("auto", description="device onto which to load the model")
+    torch_dtype: Optional[str] = Field("auto", description="torch dtype to use for model weights")
+    attn_implementation: Optional[str] = Field(
+        None,
+        description="set desired attention implementation; leave None for default. E.g. `flash_attention_2` (please ensure `torch_dtype` is either float16 or bfloat16).",
+    )
 
+    # Quantization Config
     quantize: Optional[bool] = Field(False, description="Flag to enable quantization")
     bitsandbytes: BitsAndBytesConfig = Field(None, description="Bits and Bytes configuration")
 
     # @validator("hf_model_ckpt")
     # def validate_model(cls, v, **kwargs):
     #     if not validate_repo_id(v):
     #         raise ValueError("Invalid HuggingFace dataset path")
@@ -95,14 +101,26 @@
 
     @validator("device_map")
     def set_device_map_to_none(cls, v, values, **kwargs):
         if v.lower() == "none":
             return None
         return v
 
+    @property
+    def casted_torch_dtype(self) -> Union[str, torch.dtype]:
+        if self.torch_dtype == "auto":
+            return self.torch_dtype
+
+        try:
+            torch_dtype = getattr(torch, self.torch_dtype)
+        except AttributeError:
+            raise ValueError(f"{self.torch_dtype} is not a valid torch data type")
+
+        return torch_dtype
+
 
 class LoraConfig(BaseModel):
     r: Optional[int] = Field(8, description="Lora rank")
     task_type: Optional[str] = Field("CAUSAL_LM", description="Base Model task type during training")
 
     lora_alpha: Optional[int] = Field(16, description="The alpha parameter for Lora scaling")
     bias: Optional[str] = Field("none", description="Bias type for Lora. Can be 'none', 'all' or 'lora_only'")
@@ -122,67 +140,105 @@
     #     {}, description="The mapping from layer names or regexp expression to ranks"
     # )
     # alpha_pattern: Optional[Dict[str, int]] = Field(
     #     {}, description="The mapping from layer names or regexp expression to alphas"
     # )
 
 
-# TODO: Get comprehensive Args!
 class TrainingArgs(BaseModel):
     num_train_epochs: Optional[int] = Field(1, description="Number of training epochs")
     per_device_train_batch_size: Optional[int] = Field(1, description="Batch size per training device")
     gradient_accumulation_steps: Optional[int] = Field(1, description="Number of steps for gradient accumulation")
     gradient_checkpointing: Optional[bool] = Field(True, description="Flag to enable gradient checkpointing")
     optim: Optional[str] = Field("paged_adamw_32bit", description="Optimizer")
     logging_steps: Optional[int] = Field(100, description="Number of logging steps")
     learning_rate: Optional[float] = Field(2.0e-4, description="Learning rate")
     bf16: Optional[bool] = Field(False, description="Flag to enable bf16")
     tf32: Optional[bool] = Field(False, description="Flag to enable tf32")
     fp16: Optional[bool] = Field(False, description="Flag to enable fp16")
     max_grad_norm: Optional[float] = Field(0.3, description="Maximum gradient norm")
     warmup_ratio: Optional[float] = Field(0.03, description="Warmup ratio")
     lr_scheduler_type: Optional[str] = Field("constant", description="Learning rate scheduler type")
+    save_steps: Optional[Union[int, float]] = Field(
+        500,
+        description="Number of updates steps before checkpoint saves. Should be an integer or a float in range [0,1). If smaller than 1, will be interpreted as ratio of total training steps.",
+    )
 
 
-# TODO: Get comprehensive Args!
 class SftArgs(BaseModel):
     max_seq_length: Optional[int] = Field(None, description="Maximum sequence length")
     neftune_noise_alpha: Optional[float] = Field(
         None,
         description="If not None, this will activate NEFTune noise embeddings. This can drastically improve model performance for instruction fine-tuning.",
     )
 
 
 class TrainingConfig(BaseModel):
     training_args: TrainingArgs
     sft_args: SftArgs
 
 
-# TODO: Get comprehensive Args!
 class InferenceConfig(BaseModel):
-    max_new_tokens: Optional[int] = Field(None, description="Maximum new tokens")
-    use_cache: Optional[bool] = Field(True, description="Flag to enable cache usage")
-    do_sample: Optional[bool] = Field(True, description="Flag to enable sampling")
-    top_p: Optional[float] = Field(1.0, description="Top p value")
-    temperature: Optional[float] = Field(0.1, description="Temperature value")
-    epsilon_cutoff: Optional[float] = Field(0.0, description="epsilon cutoff value")
-    eta_cutoff: Optional[float] = Field(0.0, description="eta cutoff value")
-    top_k: Optional[int] = Field(50, description="top-k sampling")
+    # Length
+    max_length: Optional[int] = Field(None, description="The maximum length the generated tokens can have.")
+    max_new_tokens: Optional[int] = Field(None, description="The maximum numbers of tokens to generate.")
+    min_length: Optional[int] = Field(0, description="The minimum length of the sequence to be generated.")
+    min_new_tokens: Optional[int] = Field(None, description="The minimum numbers of tokens to generate.")
+    early_stopping: Optional[Union[bool, str]] = Field(
+        False, description="Controls the stopping condition for beam search."
+    )
+    max_time: Optional[float] = Field(None, description="The maximum amount of time for the computation in seconds.")
+
+    # Generation Strategy
+    do_sample: Optional[bool] = Field(False, description="Whether or not to use sampling.")
+    num_beams: Optional[int] = Field(1, description="Number of beams for beam search.")
+    num_beam_groups: Optional[int] = Field(1, description="Number of groups for diversity among beams.")
+    penalty_alpha: Optional[float] = Field(None, description="Balances model confidence and degeneration penalty.")
+    use_cache: Optional[bool] = Field(
+        True,
+        description="Whether to use past key/values attentions to speed up decoding.",
+    )
+
+    # Manipulation of Model Output Logits
+    temperature: Optional[float] = Field(1.0, description="Modulates the next token probabilities.")
+    top_k: Optional[int] = Field(
+        50,
+        description="Number of highest probability tokens to keep for top-k-filtering.",
+    )
+    top_p: Optional[float] = Field(
+        1.0,
+        description="Keeps the smallest set of most probable tokens summing up to top_p.",
+    )
+    typical_p: Optional[float] = Field(1.0, description="Local typicality measure.")
+    epsilon_cutoff: Optional[float] = Field(0.0, description="Minimum conditional probability for token sampling.")
+    eta_cutoff: Optional[float] = Field(0.0, description="Hybrid of locally typical sampling and epsilon sampling.")
+    diversity_penalty: Optional[float] = Field(
+        0.0, description="Penalty for token repetition across different beam groups."
+    )
+    repetition_penalty: Optional[float] = Field(1.0, description="Penalty for token repetition.")
+    encoder_repetition_penalty: Optional[float] = Field(
+        1.0, description="Penalty on sequences not in the original input."
+    )
+    length_penalty: Optional[float] = Field(1.0, description="Exponential penalty to the length for beam search.")
+    no_repeat_ngram_size: Optional[int] = Field(0, description="Size of ngrams that cannot occur more than once.")
+    bad_words_ids: Optional[List[List[int]]] = Field(None, description="Tokens that are not allowed to be generated.")
+    force_words_ids: Optional[List[Union[List[int], List[List[int]]]]] = Field(
+        None, description="Tokens that must be generated."
+    )
+    renormalize_logits: Optional[bool] = Field(
+        False, description="Whether to renormalize logits after all processors."
+    )
 
 
 class AblationConfig(BaseModel):
     use_ablate: Optional[bool] = Field(False, description="Flag to enable ablation")
     study_name: Optional[str] = Field("ablation", description="Name of the study")
 
 
 class Config(BaseModel):
     save_dir: Optional[str] = Field("./experiments", description="Folder to save to")
     ablation: AblationConfig
-    accelerate: Optional[bool] = Field(
-        False,
-        description="set to True if you want to use multi-gpu training; then launch with `accelerate launch --config_file ./accelerate_config toolkit.py`",
-    )
     data: DataConfig
     model: ModelConfig
     lora: LoraConfig
     training: TrainingConfig
     inference: InferenceConfig
```

### Comparing `llm_toolkit-0.1.4/llmtune/qa/generics.py` & `llm_toolkit-0.2.0/llmtune/qa/generics.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.4/llmtune/qa/qa_tests.py` & `llm_toolkit-0.2.0/llmtune/qa/qa_tests.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.4/llmtune/ui/generics.py` & `llm_toolkit-0.2.0/llmtune/ui/generics.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.4/llmtune/ui/rich_ui.py` & `llm_toolkit-0.2.0/llmtune/ui/rich_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,7 +199,15 @@
                 f"{mean_values[key]:.4f}",
                 f"{median_values[key]:.4f}",
                 f"{stdev_values[key]:.4f}",
             )
 
         # Print the table
         console.print(table)
+
+    """
+    GENERATE
+    """
+
+    @staticmethod
+    def generate_config(file_name: str):
+        console.print(f"Generated config at [bold green]./{file_name}[/]")
```

### Comparing `llm_toolkit-0.1.4/llmtune/utils/ablation_utils.py` & `llm_toolkit-0.2.0/llmtune/utils/ablation_utils.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.4/llmtune/utils/rich_print_utils.py` & `llm_toolkit-0.2.0/llmtune/utils/rich_print_utils.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.1.4/llmtune/utils/save_utils.py` & `llm_toolkit-0.2.0/llmtune/utils/save_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,103 @@
 """
 Helper functions to help managing saving and loading of experiments:
     1. Generate save directory name
     2. Check if files are present at various experiment stages
 """
 
 import hashlib
-import os
 import re
 from dataclasses import dataclass
 from functools import cached_property
-from os.path import exists
+from pathlib import Path
 
 import yaml
 from sqids import Sqids
 
+from llmtune.constants.files import (
+    CONFIG_DIR_NAME,
+    CONFIG_FILE_NAME,
+    DATASET_DIR_NAME,
+    NUM_MD5_DIGITS_FOR_SQIDS,
+    QA_DIR_NAME,
+    QA_FILE_NAME,
+    RESULTS_DIR_NAME,
+    RESULTS_FILE_NAME,
+    WEIGHTS_DIR_NAME,
+)
 from llmtune.pydantic_models.config_model import Config
 
 
-NUM_MD5_DIGITS_FOR_SQIDS = 5  # TODO: maybe move consts to a dedicated folder
-
-
 @dataclass
 class DirectoryList:
-    save_dir: str
+    save_dir: Path
     config_hash: str
 
     @property
-    def experiment(self) -> str:
-        return os.path.join(self.save_dir, self.config_hash)
+    def experiment(self) -> Path:
+        return self.save_dir / self.config_hash
+
+    @property
+    def config(self) -> Path:
+        return self.experiment / CONFIG_DIR_NAME
+
+    @property
+    def config_file(self) -> Path:
+        return self.config / CONFIG_FILE_NAME
+
+    @property
+    def dataset(self) -> Path:
+        return self.experiment / DATASET_DIR_NAME
 
     @property
-    def config(self) -> str:
-        return os.path.join(self.experiment, "config")
+    def weights(self) -> Path:
+        return self.experiment / WEIGHTS_DIR_NAME
 
     @property
-    def dataset(self) -> str:
-        return os.path.join(self.experiment, "dataset")
+    def results(self) -> Path:
+        return self.experiment / RESULTS_DIR_NAME
 
     @property
-    def weights(self) -> str:
-        return os.path.join(self.experiment, "weights")
+    def results_file(self) -> Path:
+        return self.results / RESULTS_FILE_NAME
 
     @property
-    def results(self) -> str:
-        return os.path.join(self.experiment, "results")
+    def qa(self) -> Path:
+        return self.experiment / QA_DIR_NAME
 
     @property
-    def qa(self) -> str:
-        return os.path.join(self.experiment, "qa")
+    def qa_file(self) -> Path:
+        return self.qa / QA_FILE_NAME
 
 
 class DirectoryHelper:
-    def __init__(self, config_path: str, config: Config):
-        self.config_path: str = config_path
+    def __init__(self, config_path: Path, config: Config):
+        self.config_path: Path = config_path
         self.config: Config = config
         self.sqids: Sqids = Sqids()
         self.save_paths: DirectoryList = self._get_directory_state()
 
-        os.makedirs(self.save_paths.experiment, exist_ok=True)
-        if not exists(self.save_paths.config):
+        self.save_paths.experiment.mkdir(parents=True, exist_ok=True)
+        if not self.save_paths.config.exists():
             self.save_config()
 
     @cached_property
     def config_hash(self) -> str:
         config_str = self.config.model_dump_json()
         config_str = re.sub(r"\s", "", config_str)
         hash = hashlib.md5(config_str.encode()).digest()
         return self.sqids.encode(hash[:NUM_MD5_DIGITS_FOR_SQIDS])
 
     def _get_directory_state(self) -> DirectoryList:
         save_dir = (
-            self.config.save_dir
+            Path(self.config.save_dir)
             if not self.config.ablation.use_ablate
-            else os.path.join(self.config.save_dir, self.config.ablation.study_name)
+            else Path(self.config.save_dir) / self.config.ablation.study_name
         )
         return DirectoryList(save_dir, self.config_hash)
 
     def save_config(self) -> None:
-        os.makedirs(self.save_paths.config, exist_ok=True)
+        self.save_paths.config.mkdir(parents=True, exist_ok=True)
         model_dict = self.config.model_dump()
 
-        with open(os.path.join(self.save_paths.config, "config.yml"), "w") as file:
+        with (self.save_paths.config / "config.yml").open("w") as file:
             yaml.dump(model_dict, file)
```

### Comparing `llm_toolkit-0.1.4/pyproject.toml` & `llm_toolkit-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm-toolkit"
-version = "0.1.4"
+version = "0.2.0"
 description = "LLM Finetuning resource hub + toolkit"
 authors = ["Benjamin Ye <benjamin.ye@georgian.io>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "llmtune"}]
 repository = "https://github.com/georgian-io/LLM-Finetuning-Toolkit"
 # homepage = ""
```

### Comparing `llm_toolkit-0.1.4/PKG-INFO` & `llm_toolkit-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-toolkit
-Version: 0.1.4
+Version: 0.2.0
 Summary: LLM Finetuning resource hub + toolkit
 Home-page: https://github.com/georgian-io/LLM-Finetuning-Toolkit
 License: Apache 2.0
 Keywords: llm,finetuning,language models,machine learning,deep learning
 Author: Benjamin Ye
 Author-email: benjamin.ye@georgian.io
 Requires-Python: >=3.9,<=3.12
@@ -61,46 +61,76 @@
 LLM Finetuning toolkit is a config-based CLI tool for launching a series of LLM finetuning experiments on your data and gathering their results. From one single `yaml` config file, control all elements of a typical experimentation pipeline - **prompts**, **open-source LLMs**, **optimization strategy** and **LLM testing**.
 
 <p align="center">
 <img src="https://github.com/georgian-io/LLM-Finetuning-Toolkit/blob/main/assets/overview_diagram.png?raw=true" width="900" />
 </p>
 
 ## Installation
+
 ### pipx (recommended)
+
 pipx installs the package and depdencies in a seperate virtual environment
+
 ```shell
 pipx install llm-toolkit
 ```
 
 ### pip
+
 ```shell
 pip install llm-toolkit
 ```
 
-
 ## Quick Start
 
 This guide contains 3 stages that will enable you to get the most out of this toolkit!
 
 - **Basic**: Run your first LLM fine-tuning experiment
-- **Intermediate**: Run a custom experiment by changing the componenets of the YAML configuration file
+- **Intermediate**: Run a custom experiment by changing the components of the YAML configuration file
 - **Advanced**: Launch series of fine-tuning experiments across different prompt templates, LLMs, optimization techniques -- all through **one** YAML configuration file
 
 ### Basic
 
-```python
-   llmtune --config-path ./config.yml
+```shell
+   llmtune generate config
+   llmtune run --config-path ./config.yml
 ```
 
-This command initiates the fine-tuning process using the settings specified in the default YAML configuration file `config.yaml`.
+The first command generates a helpful starter `config.yml` file and saves in the current working directory. This is provided to users to quickly get started and as a base for further modification.
+
+Then the second command initiates the fine-tuning process using the settings specified in the default YAML configuration file `config.yaml`.
 
 ### Intermediate
 
 The configuration file is the central piece that defines the behavior of the toolkit. It is written in YAML format and consists of several sections that control different aspects of the process, such as data ingestion, model definition, training, inference, and quality assurance. We highlight some of the critical sections.
 
+#### Flash Attention 2
+
+To enable Flash-attention for [supported models](https://huggingface.co/docs/transformers/perf_infer_gpu_one#flashattention-2). First install `flash-attn`:
+
+**pipx**
+
+```shell
+pipx inject llm-toolkit flash-attn --pip-args=--no-build-isolation
+```
+
+**pip**
+
+```
+pip install flash-attn --no-build-isolation
+```
+
+Then, add to config file.
+
+```yaml
+model:
+  torch_dtype: "bfloat16" # or "float16" if using older GPU
+  attn_implementation: "flash_attention_2"
+```
+
 #### Data Ingestion
 
 An example of what the data ingestion may look like:
 
 ```yaml
 data:
   file_type: "huggingface"
@@ -295,50 +325,48 @@
 
 ```shell
    # CPU
    docker run -it llm-toolkit
    # GPU
    docker run -it --gpus all llm-toolkit
 ```
+
 </details>
 
 <details>
 <summary>Poetry (recommended)</summary>
 
 See poetry documentation page for poetry [installation instructions](https://python-poetry.org/docs/#installation)
 
 ```shell
    poetry install
 ```
+
 </details>
 <details>
 <summary>pip</summary>
 We recommend using a virtual environment like `venv` or `conda` for installation
 
 ```shell
    pip install -e .
 ```
+
 </details>
 </details>
 
-
-
 ### Checklist Before Pull Request (Optional)
 
 1. Use `ruff check --fix` to check and fix lint errors
 2. Use `ruff format` to apply formatting
 
 NOTE: Ruff linting and formatting checks are done when PR is raised via Git Action. Before raising a PR, it is a good practice to check and fix lint errors, as well as apply formatting.
 
-
 ### Releasing
 
-
-To manually release a PyPI package, please run: 
+To manually release a PyPI package, please run:
 
 ```shell
    make build-release
 ```
 
 Note: Make sure you have pypi token for this [PyPI repo](https://pypi.org/project/llm-toolkit/).
 
-
```

