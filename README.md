<p align="center">
    <img src="https://modelscope.oss-cn-beijing.aliyuncs.com/model-repo/codefuse-ai/CodeFuse-logo-1.png" width="500"/>
<p>
<br>

<p align="center">
    <a href="https://modelscope.cn/models/codefuse-ai/CodeFuse-Code-Generation-Model/summary">
        <img src="https://img.shields.io/badge/ModelScope-Open%20Source-blue">
    </a>
    <a href="https://huggingface.co/codefuse-ai">
        <img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-yellow">
    </a>
    <a href="LICENSE">
        <img src="https://img.shields.io/badge/License-Apache--2.0-green">
    </a>
    <a href="https://github.com/codefuse-ai/CodeFuse-CGM/issues">
        <img src="https://img.shields.io/github/issues/codefuse-ai/CodeFuse-CGM?color=red">
    </a>
    <a href="https://github.com/codefuse-ai/CodeFuse-CGM/stargazers">
        <img src="https://img.shields.io/github/stars/codefuse-ai/CodeFuse-CGM?color=yellow">
    </a>
</p>

English | [简体中文](README-zh.md)

# CodeFuse-Code-Generation-Model

`CodeFuse-Code-Generation-Model` is a suite of open-source code generation models launched by the Ant Group's CodeFuse team. This release includes two code generation models with parameter sizes of 13B and 7B.

- `CodeFuse-13B`: Pre-trained on 1.3 trillion tokens of code data, it excels in code generation tasks. Through instruction fine-tuning with a mixture of approximately 100,000 high-quality instruction samples, it has demonstrated outstanding performance in cross-lingual code generation (e.g., from other languages to Python) and in generating code for specific scenarios such as database operations, cloud-native development, and GUI generation. The model supports a context window of up to 16k.
- `CodeFuse-7B`: Pre-trained on 800 billion tokens of code data, it supports a context window of up to 8k and is suitable for deployment on consumer-grade graphics cards.

Both `CodeFuse-13B` and `CodeFuse-7B` support code generation in over 40 programming languages.

## Model Download

| Model        | Description                               | Parameter Size | Context Length | Download Link                                                                                    |
|--------------|-------------------------------------------|----------------|----------------|--------------------------------------------------------------------------------------------------|
| `CodeFuse-13B` | Base model, instruction fine-tuned | 13B            | 16K            | [HuggingFace](https://huggingface.co/codefuse-ai/CodeFuse-13B) / [ModelScope](https://modelscope.cn/models/codefuse-ai/CodeFuse-13B/summary) |
| `CodeFuse-7B`  | Base model, instruction fine-tuned | 7B             | 8K             | [HuggingFace](https://huggingface.co/codefuse-ai/CodeFuse-7B) / [ModelScope](https://modelscope.cn/models/codefuse-ai/CodeFuse-7B/summary)   |

## Quick Start

### Environmental Setup

First, you need to configure the relevant environment and install the required third-party libraries.

```bash
# Recommended Python version >= 3.8
# Create a virtual environment
conda create -n codefuse_dev python=3.10
conda activate codefuse_dev

# Install dependencies
pip install -r requirements.txt
