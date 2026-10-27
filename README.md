# Awesome Denolle Lab [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of open software, workflows and reproducibility packages built by the
> [Denolle Lab](https://denolle-lab.github.io/) at the University of Washington.

We run the entire research practice through computational tools and openness. Every paper,
catalog and model below is meant to be rerun. Forks link to their upstream repository, where
the code is maintained. For climate-compounded geohazards, see the sister list
[awesome-gaia](https://github.com/gaia-hazlab/awesome-gaia).

## Contents

- [Data access and archives](#data-access-and-archives)
- [Cloud and HPC workflows](#cloud-and-hpc-workflows)
- [Ambient noise and dv/v monitoring](#ambient-noise-and-dvv-monitoring)
- [Earthquake detection, catalogs and machine learning](#earthquake-detection-catalogs-and-machine-learning)
- [Surface events and volcanoes](#surface-events-and-volcanoes)
- [Distributed acoustic sensing](#distributed-acoustic-sensing)
- [Wave physics and earthquake sources](#wave-physics-and-earthquake-sources)
- [Metascience and group practice](#metascience-and-group-practice)

## Data access and archives

- [seisfetch](https://github.com/Denolle-Lab/seisfetch): Fast miniSEED download from EarthScope, SCEDC, NCEDC and 37+ FDSN servers, without ObsPy.
- [pnwstore](https://github.com/niyiyu/pnwstore): Utilities to query the group's Pacific Northwest seismic archive.
- [CloudPyASDF](https://github.com/niyiyu/CloudPyASDF): ASDF reader for cloud object storage.

## Cloud and HPC workflows

- [seismicloud](https://github.com/Denolle-Lab/seismicloud): Template matching and ML phase picking on cloud resources.
- [seismicloud-image](https://github.com/Denolle-Lab/seismicloud-image): Public Docker image for seismicloud.
- [seisbench-jupyter](https://github.com/Denolle-Lab/seisbench-jupyter): JupyterHub-compatible Docker image with SeisBench.
- [C4-Project.jl](https://github.com/Julians42/C4-Project.jl): Ambient-noise cross-correlation at scale on AWS, in Julia.
- [SeisCore.jl](https://github.com/Julians42/SeisCore.jl): Core Julia package for the C4 project, tuned for EC2 and AWS Batch.

## Ambient noise and dv/v monitoring

- [NoisePy](https://github.com/noisepy/NoisePy): Ambient-noise seismology package for cross-correlation and monitoring, local or cloud ([docs](https://noisepy.github.io/NoisePy/)).
- [SeisNoise.jl](https://github.com/JuliaSeismo/SeisNoise.jl): Ambient-noise cross-correlation in Julia, with GPU support.
- [das-noisepy](https://github.com/Denolle-Lab/das-noisepy): End-to-end NoisePy workflows on DAS data.
- [codameter](https://github.com/Denolle-Lab/codameter): Six-phase operational workflow that reads dv/v as a stress and strain meter ([site](https://denolle-lab.github.io/codameter/), [paper repo](https://github.com/Denolle-Lab/codameter-paper)).
- [DVV_Forecast](https://github.com/Denolle-Lab/DVV_Forecast): KoopDV, Koopman-based interpolation and forecasting of dv/v in space and time.
- [DVV_Discovery](https://github.com/Denolle-Lab/DVV_Discovery): Machine-learning forecasts of dv/v time series in California.
- [Clements-Denolle-2022](https://github.com/tclements/Clements-Denolle-2022): Replication code for Clements and Denolle, "The seismic signature of California's earthquakes, droughts, and floods".
- [dvv-hydro-CompGeo-review-2024](https://github.com/Denolle-Lab/dvv-hydro-CompGeo-review-2024): Meta-analysis of dv/v sensitivity to groundwater level.
- [Mt-St-Helens](https://github.com/Denolle-Lab/Mt-St-Helens): Electronic supplement to Makus et al. (2024), 25 years of seismic velocity at Mount St. Helens.

## Earthquake detection, catalogs and machine learning

- [cascadia_obs_ensemble](https://github.com/Denolle-Lab/cascadia_obs_ensemble): Offshore Cascadia earthquake catalog from ensemble deep learning.
- [ELEP](https://github.com/congcy/ELEP): Ensemble learning for earthquake processing.
- [phasenet-retrain](https://github.com/Denolle-Lab/phasenet-retrain): Retraining PhaseNet with SeisBench for cloud computing ([site](https://denolle-lab.github.io/phasenet-retrain/)).
- [PNW_Seismic_Event_Classification](https://github.com/Akashkharita/PNW_Seismic_Event_Classification): ML and deep-learning classifiers for earthquakes, explosions and surface events in the Pacific Northwest, 2001 to 2023.
- [tiny-cnn-seismicML](https://github.com/Denolle-Lab/tiny-cnn-seismicML): Small CNN that separates urban from tectonic signals.
- [FoundationModel_GP](https://github.com/Denolle-Lab/FoundationModel_GP): GP2Vec, Wav2Vec2-style self-supervised learning on continuous seismic data in S3.
- [TeleseismicDenoiser](https://github.com/qibinshi/TeleseismicDenoiser): Separates teleseismic earthquake signals from noise.
- [expand_redpy](https://github.com/Denolle-Lab/expand_redpy): Extends the REDPy repeating-earthquake catalog with EQcorrscan and FMF, with locations and clustering.
- [cidas-badger-earthquake-catalog](https://github.com/Denolle-Lab/cidas-badger-earthquake-catalog): Detection, location and characterization with broadbands and DAS in Cook Inlet.
- [PNSN_Mag](https://github.com/Denolle-Lab/PNSN_Mag): Recomputes PNSN magnitudes and discriminates earthquakes from explosions.

## Surface events and volcanoes

- [surfcat](https://github.com/Denolle-Lab/surfcat): 25-year catalog of seismic surface events in the Pacific Northwest.
- [surface_events](https://github.com/Denolle-Lab/surface_events): Location, velocity and directivity of surface events.
- [mt-rainier-digital-model](https://github.com/Denolle-Lab/mt-rainier-digital-model): rainier3d, an open Python model of Mount Rainier built toward a digital twin ([site](https://denolle-lab.github.io/mt-rainier-digital-model/)).
- [rainier-seismic-atlas](https://github.com/yaoderek/rainier-seismic-atlas): 3D view of the Mount Rainier seismic network on USGS terrain and 1 m summit lidar.

## Distributed acoustic sensing

- [greenlanDAS](https://github.com/Denolle-Lab/greenlanDAS): DAS analysis at Store Glacier, Greenland.
- [Shi_etal_2023_denoiseDAS](https://github.com/Denolle-Lab/Shi_etal_2023_denoiseDAS): Denoising DAS to improve earthquake phase picking offshore.
- [FarmDAS](https://github.com/Denolle-Lab/FarmDAS): Processing DAS data from farms in England.
- [OrcaSeis](https://github.com/Denolle-Lab/OrcaSeis): Orca and other whale signals in hydrophone and DAS data.
- [badger-cidas-data-report](https://github.com/Denolle-Lab/badger-cidas-data-report): Scripts that reproduce the figures of the Cook Inlet DAS data report.

## Wave physics and earthquake sources

- [gesc-python](https://github.com/Denolle-Lab/gesc-python): Validated surface-wave modes, acoustic Scholte coupling and phase-change depth inference ([site](https://denolle-lab.github.io/gesc-python/)).
- [PyGesc](https://github.com/Denolle-Lab/PyGesc): Earlier generalized eigenproblem spectral collocation solver in Python.
- [surface_wave_sensitivity](https://github.com/kuanfufeng/Sharing_repo): Depth and frequency sensitivity kernels for surface waves.
- [da-instaseis](https://github.com/Denolle-Lab/da-instaseis): Data assimilation of global wavefields.
- [CSBP](https://github.com/yinjiuxun/CSBP): Compressive-sensing back-projection for earthquake source imaging (MATLAB).
- [STF_DTW](https://github.com/yinjiuxun/STF_DTW): Dynamic time warping clustering of earthquake source time functions (MATLAB).

## Metascience and group practice

- [meta-seismology](https://github.com/Denolle-Lab/meta-seismology): Interactive graph of 5,272 observational seismology studies, 2021 to 2025 ([site](https://denolle-lab.github.io/meta-seismology/)).
- [metascience-and-AI](https://github.com/Denolle-Lab/metascience-and-AI): Fall 2026 seminar on how research proceeds and what follows for agents in science ([site](https://denolle-lab.github.io/metascience-and-AI/)).
- [lab-skills](https://github.com/Denolle-Lab/lab-skills): Skill files for our research methods, AI tools, data analysis and writing.
- [Group_Utils](https://github.com/Denolle-Lab/Group_Utils): Onboarding, working contract and open-science policies.

## Contributing

Add your repository with a pull request: one line, the repository link, a sentence on what it
does, and a link to docs or a paper if one exists. Keep the code public and rerunnable.
