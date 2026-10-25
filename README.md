# Mobile Computational Photography — Companion Code

This repository contains the source code for the book **"Mobile Computational Photography"**. Each chapter's code lives in its own folder and its own Git repository. This parent repository ties them all together using [Git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules), so you can grab everything with a single command.

## Repository Structure

| Folder | Chapter(s) | Topic |
|--------|-----------|-------|
| `AI_ISP` | 3–6 | Image Signal Processing pipeline |
| `Autofocus` | 5 | PDAF / CDAF autofocus algorithms |
| `camera_tuning` | 7 | AI-driven ISP tuning automation |
| `AutoWhiteBalance` | 9 | Automatic white balance correction |
| `AutoExposure` | 9 | Automatic exposure control |
| `HDR` | 13 | High Dynamic Range imaging |
| `MultiCamera` | 15 | Multi-camera calibration and fusion |
| `video_stablization` | 17 | Video stabilization techniques |
| `video_bokeh` | 19 | Video bokeh effects |
| `super_resolution` | 22 | Super resolution algorithms |

## Getting Started

### Option A — Clone everything (recommended)

This downloads the parent repo **and** all chapter code in one step:

```bash
git clone --recursive https://github.com/JeffRen1977/mobile_computational_photograph.git
cd mobile_computational_photograph
```

> **What does `--recursive` do?**  Each chapter folder is a Git submodule — a pointer to a separate repository. The `--recursive` flag tells Git to also clone every submodule so the folders are populated with code instead of being empty.

### Option B — Clone a single chapter

If you only need one chapter, clone its repository directly:

```bash
# Example: clone just the HDR chapter
git clone https://github.com/JeffRen1977/hdr.git
```

See the [Individual Repositories](#individual-repositories) section below for all links.

### Option C — You already cloned without `--recursive`

If the chapter folders are empty, run:

```bash
git submodule update --init --recursive
```

This initializes and downloads all submodules after the fact.

## Setting Up the Python Environment

All chapters share a single virtual environment located one level above each chapter folder:

```bash
# Create the shared virtual environment (run once)
python3 -m venv virtual_env

# Activate it
source virtual_env/bin/activate      # macOS / Linux
# virtual_env\Scripts\activate       # Windows

# Install a chapter's dependencies
cd HDR
pip install -r requirements.txt
```

Each chapter folder has its own `requirements.txt`. Activate the environment, `cd` into a chapter, and install.

## Updating to the Latest Code

To pull the latest changes for every chapter:

```bash
git pull
git submodule update --remote --recursive
```

This fetches the newest commit from each chapter's repository.

## Running Tests

Every chapter includes a pytest test suite. From any chapter folder:

```bash
source ../virtual_env/bin/activate
python3 -m pytest tests/ -v
```

## Individual Repositories

You can also visit or clone each chapter's code independently:

| Chapter | Repository |
|---------|-----------|
| AI ISP (Ch. 3–6) | [JeffRen1977/isp_pipeline](https://github.com/JeffRen1977/isp_pipeline) |
| Autofocus (Ch. 5) | [JeffRen1977/auto-focus](https://github.com/JeffRen1977/auto-focus) |
| Camera Tuning (Ch. 7) | [JeffRen1977/camera_tuning](https://github.com/JeffRen1977/camera_tuning) |
| Auto White Balance (Ch. 9) | [JeffRen1977/auto-white-balance](https://github.com/JeffRen1977/auto-white-balance) |
| Auto Exposure (Ch. 9) | [JeffRen1977/auto-exposure](https://github.com/JeffRen1977/auto-exposure) |
| HDR (Ch. 13) | [JeffRen1977/hdr](https://github.com/JeffRen1977/hdr) |
| MultiCamera (Ch. 15) | [JeffRen1977/multicamera](https://github.com/JeffRen1977/multicamera) |
| Video Stabilization (Ch. 17) | [JeffRen1977/video_stablization](https://github.com/JeffRen1977/video_stablization) |
| Video Bokeh (Ch. 19) | [JeffRen1977/video_bokeh](https://github.com/JeffRen1977/video_bokeh) |
| Super Resolution (Ch. 22) | [JeffRen1977/super_resolution](https://github.com/JeffRen1977/super_resolution) |

## License

Please refer to individual chapter repositories for license information.
