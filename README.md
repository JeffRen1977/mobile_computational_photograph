# Mobile Computational Photography

A comprehensive collection of computational photography projects and implementations, organized as a monorepo with git submodules.

## 📁 Project Structure

This repository contains the following projects, each maintained as a separate git repository:

- **AI_ISP** - AI-powered Image Signal Processing pipeline
- **AutoExposure** - Automatic exposure control system
- **Autofocus** - Autofocus algorithms and implementations
- **AutoWhiteBalance** - Automatic white balance correction
- **camera_tuning** - Camera tuning and adaptive ISP demos
- **HDR** - High Dynamic Range imaging
- **MultiCamera** - Multi-camera calibration and processing
- **super_resolution** - Super resolution algorithms
- **video_bokeh** - Video bokeh effects
- **video_stablization** - Video stabilization techniques

## 🚀 Quick Start

### Clone Everything at Once

To clone this repository and all submodules in one command:

```bash
git clone --recursive https://github.com/YOUR_USERNAME/Mobile_Computational_photograph.git
cd Mobile_Computational_photograph
```

If you've already cloned the repository without submodules, initialize them with:

```bash
git submodule update --init --recursive
```

### Update All Submodules

To update all submodules to their latest commits:

```bash
git submodule update --remote --recursive
```

### Work with Individual Projects

Each project is a separate git repository. You can:

- Navigate to any project directory and work with it independently
- Each project has its own README with specific setup instructions
- Check individual project requirements in their respective `requirements.txt` files

## 📋 Requirements

Each project has its own requirements. Please refer to the individual project READMEs for specific setup instructions.

## 🔧 Setup

1. Clone the repository with submodules (see Quick Start above)
2. Navigate to the project you want to work with
3. Follow the project-specific setup instructions in that project's README
4. Install project-specific requirements

## 📝 Notes

- The `virtual_env` folder is excluded from version control
- Each project maintains its own git history and can be updated independently
- The `data` folder contains shared data files used across projects

## 🤝 Contributing

Each project is maintained separately. Please contribute to individual projects through their respective repositories.

## 📚 Documentation

Each project contains its own documentation:
- Individual README files in each project directory
- Project-specific documentation and guides
- Example scripts and demos

## 🔗 Individual Repositories

- [AI ISP Pipeline](https://github.com/JeffRen1977/isp_pipeline)
- [Auto Exposure](https://github.com/JeffRen1977/auto-exposure)
- [Autofocus](https://github.com/JeffRen1977/auto-focus)
- [Auto White Balance](https://github.com/JeffRen1977/auto-white-balance)
- [Camera Tuning](https://github.com/JeffRen1977/camera_tuning)
- [HDR](https://github.com/JeffRen1977/hdr)
- [MultiCamera](https://github.com/JeffRen1977/multicamera)
- [Super Resolution](https://github.com/JeffRen1977/super_resolution)
- [Video Bokeh](https://github.com/JeffRen1977/video_bokeh)
- [Video Stabilization](https://github.com/JeffRen1977/video_stablization)

## 📄 License

Please refer to individual project repositories for license information.

