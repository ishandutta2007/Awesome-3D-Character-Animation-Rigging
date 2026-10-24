# Awesome-3D-Character-Animation-Rigging

## Top 3D Character Animation & Rigging Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Auto-Rigging, AI Motion Capture & Self-Hosted Animation Toolkits*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **3D Character Animation & Rigging**. These tools help artists and developers turn static models into animated characters—handling skeleton creation, skinning, motion capture from video, and animation retargeting—ranging from browser-based auto-riggers to AI-powered video-to-motion pipelines.



**Examples** include Mixamo, DeepMotion, Plask, Rokoko, Move.ai, Cascadeur, and the open-source leaders Mesh2Motion and MoCapAnything (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, avoiding subscription fees, and controlling the animation pipeline. The open-source landscape is anchored by **Mesh2Motion** (the MIT-licensed Mixamo alternative with CC0 assets), **MoCapAnything** (the SIGGRAPH Asia 2026 video-to-rotation framework for arbitrary skeletons), and **Reze MiPo Desktop** (the MMD-focused AI motion capture app), with **PSD2Live** serving Live2D/VTuber rigging needs.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)



## Sector Overview & Market Dynamics

The global 3D animation and character rigging software market is valued at **$15B – $30B**, with the specialized motion capture sub-segment accounting for **$300M – $1B+** as real-time tracking expands. The sector exhibits a dual market structure: foundational DCC software pipelines and high-end optical capture hardware are **highly concentrated** around legacy incumbents (e.g., Adobe, Autodesk), while AI-driven markerless capture, browser-based auto-rigging, and indie animation toolkits are **moderately to highly fragmented** with rapid startup and open-source innovation.



## SaaS/Hosted Platforms

| Product | Description | Company Scale (Revenue / Valuation) | Pricing | Free Tier Limit |
| :--- | :--- | :--- | :--- | :--- |
| **[Mixamo (Adobe)](https://www.mixamo.com/)** | Browser-based auto-rigger and animation library with 2,000+ motion-capture clips. | **~$26B Revenue / ~$250B Valuation** (Adobe Inc., NASDAQ: ADBE) | **$0** (Free with an Adobe account) | **Free forever**: Full access to 2,000+ mocap animations and auto-rigging pipeline; standard commercial use permitted. |
| **[Wonder Dynamics (Autodesk Flow Studio)](https://www.autodesk.com/)** | AI-powered character animation, mocap, and VFX pipeline from video (formerly Wonder Studio). | **~$7.8B Revenue / ~$50B Valuation** (Autodesk, NASDAQ: ADSK) | Paid tiers start at **$7/month** (Lite plan, billed annually at $84/yr) or $10/month billed monthly; Pro at $64/month | **Free forever tier**: 300 credits/mo, max 720p export, 1 concurrent job, 1 actor tracking per project, 1 GB storage, 3 custom characters, watermarked outputs. |
| **[Cascadeur](https://cascadeur.com/)** | AI-assisted keyframe animation software with physics-based posing. | **~$20M – $50M Est. Revenue** (Nekki, parent gaming studio) | **$8/month** (Indie plan, billed annually at $96/yr) or $19/month billed monthly; Pro at $33/month | **Free forever plan**: Non-commercial use only, export strictly limited to proprietary `.casc` format (no standard FBX/DAE/USD export). |
| **[Rokoko Studio](https://www.rokoko.com/products/studio)** | Motion capture suite for Rokoko hardware and AI video tracking. | **~$50M – $100M Valuation** (~$13.7M venture funding raised) | **$10/month** (Basic plan, billed annually) or $15/month billed monthly; Plus at $20/month, Pro at $50/month | **Starter plan (free forever)**: Basic recording and motion capture editing, 30 seconds/month Vision AI video mocap processing, 5 text-to-motion imports/mo, 1 month cloud storage. |
| **[AccuRIG (Reallusion)](https://www.reallusion.com/auto-rig/accurig.html)** | Standalone auto-rigging tool for humanoid 3D characters. | **~$7M – $9M Annual Revenue** (Reallusion Inc., TPEX: 6882) | **$0** (Standalone software is completely free; optional ActorCore motions priced individually or via packs) | **Free forever plan**: Unlimited auto-rigging and FBX/USD exports with full commercial rights; limited to humanoid biped meshes and ~30 free sample motions from ActorCore. |
| **[Move.ai](https://www.move.ai/)** | Markerless single-camera (Move One iOS) and multi-camera motion capture. | **<$50M Valuation** ($1M – $10M ARR est., venture-backed) | **$18/month** (Move One Starter tier, credit-based) or usage-based at $0.012/sec (s1 single-cam); custom enterprise pricing for Genesis multi-cam volumes | **Free plan (Move One iOS)**: One-time allotment of 30 credits (non-expiring), max 30 seconds per video capture; multi-camera Genesis workflows require a scheduled enterprise demo/trial. |
| **[DeepMotion](https://www.deepmotion.com/)** | AI video-to-3D motion capture and real-time body tracking platform. | **~$1.4M ARR est.** (Venture-backed / strategic AI footprint) | **$9/month** (Starter plan for Animate 3D, billed annually at $108/yr) or $15/month billed monthly | **Freemium plan (free forever)**: 25 animation credits/month (1 credit = 1 sec body animation), max 20 seconds per video, max 2 persons tracked, 1080p@30fps, strictly personal non-commercial use. |
| **[Plask Motion](https://plask.ai/)** | Browser-based AI motion capture from video for animators and digital creators. | **~$1.4M ARR est.** ($2.56M total venture funding raised) | **$18/month** (Standard plan, billed annually) or $40/month billed monthly; Pro tier at $50/month (billed annually) | **Freemium plan (free forever)**: Up to 900 daily credits (~15–30s of AI mocap processing daily), basic keyframe editing, limited personal non-commercial export. |



## Open-Source GitHub Projects



- **[Mesh2Motion](https://github.com/Mesh2Motion/mesh2motion-app)** [![GitHub Stars](https://img.shields.io/github/stars/Mesh2Motion/mesh2motion-app?style=social&color=white)](https://github.com/Mesh2Motion/mesh2motion-app/stargazers)  

  **The MIT-licensed Mixamo alternative.** Import a 3D model (GLB/GLTF), pick a skeleton type, adjust the skeleton to fit, test animations, and export—all in the browser. **Key differentiator**: explicitly designed to be more flexible than Mixamo, supporting other model and skeleton types through open-source extensibility . **Assets**: all 3D models, rigs, and animations are **CC0 licensed**—fully free for any use . **Deployment**: run locally with Node.js, or Docker (`docker-compose up -d` → localhost:3000) . Best for developers and artists wanting a self-hosted, hackable alternative to Mixamo's auto-rigging and animation library.



- **[MoCapAnything V2](https://github.com/phongdaot/MocapAnything)** [![GitHub Stars](https://img.shields.io/github/stars/phongdaot/MocapAnything?style=social&color=white)](https://github.com/phongdaot/MocapAnything/stargazers)  

  **The SIGGRAPH Asia 2026 video-to-rotation framework.** End-to-end motion capture for **arbitrary skeletons**—animals, humans, objects, and custom rigs—without template-specific body models. **Pipeline**: video → 3D pose → BVH-ready joint rotations, jointly optimized without analytical IK. **Key advantages**: mesh-free and **~20× faster** than mesh-based pipelines; supports bringing your own rigged FBX character . **Status**: pretrained V2 weights released, live Hugging Face demo available (ZeroGPU, free), local demo via `python demo/app.py` . **Training data**: gated (~25 GB), requires Truebones Zoo access . Best for researchers and technical artists needing motion capture for non-humanoid or custom skeletons.



- **[Reze MiPo Desktop](https://github.com/BesingBG/reze-mipo-desktop)** [![GitHub Stars](https://img.shields.io/github/stars/BesingBG/reze-mipo-desktop?style=social&color=white)](https://github.com/BesingBG/reze-mipo-desktop/stargazers)  

  **The MMD-focused AI motion capture app.** Cross-platform (Windows/macOS), **fully offline**—no dedicated mocap hardware needed. **Input modes**: real-time webcam, video frame-by-frame, or single photo → static VMD pose. **Output**: standard `.vmd` motion files for MikuMikuDance models. **Features**: full body + both hands + face via MediaPipe; custom PMX model import; WebGPU rendering. GPL-3.0 licensed. Best for MMD users and VTubers wanting free, offline motion capture from video or webcam.



- **[PSD2Live](https://github.com/tsunehimatoi/psd2live)** [![GitHub Stars](https://img.shields.io/github/stars/tsunehimatoi/psd2live?style=social&color=white)](https://github.com/tsunehimatoi/psd2live/stargazers)  

  **The Live2D/VTuber rigging pipeline.** Generates Live2D Cubism models from layered PSD files, with **Rigging, Animation, Physics, and Texture workspaces**. **Exports**: `.moc3`/`.cmo3` for Cubism Editor, `.model3.json` bundles for Cubism runtime, and VTube Studio-ready packages with face tracking mapped to standard parameters . **Platforms**: Windows 10/11 (x64, ARM64), Linux (x86_64/arm64). **Limitations**: macOS requires JDK 21 and running from source; Linux native preview needs X11/GLX (XWayland works) . Best for VTubers and Live2D artists wanting an open pipeline from PSD to rigged, animatable model without manual Cubism setup.



### Additional Strong Open-Source Options



- **mesh2motion-assets** — The CC0 asset repository (models, rigs, animations) supporting Mesh2Motion . Best for contributors wanting to expand the animation library.

- **Reze MiPo (core)** — The underlying real-time motion capture tool and WebGPU renderer that Reze MiPo Desktop builds upon . Best for developers wanting the core engine without the desktop wrapper.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- **Mixamo remains the most generous free tier in the category**: 2,000+ animations, auto-rigging, and commercial use allowed—all free with an Adobe account . Open-source alternatives like Mesh2Motion are catching up but have smaller animation libraries.

- **"Free" tools have restrictions**: Cascadeur's free plan is **non-commercial only** and exports only proprietary format ; Move.ai has no free tier and bills per second ; AccuRIG's free tier is feature-limited .

- **Motion capture quality varies by input**: Move.ai's multi-camera setup produces higher fidelity than single-camera; Reze MiPo and MoCapAnything are single-video solutions with corresponding accuracy trade-offs.

- **Plask's current offering appears to have pivoted**: the pricing page describes a product analytics tool, not motion capture. Verify before pursuing it for animation needs .



---



**Made for 3D artists, animators, game developers, and VTubers building character animation pipelines.**  

Let's make character animation and rigging more open, accessible, and self-hostable.
