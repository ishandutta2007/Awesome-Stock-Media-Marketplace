# Awesome-Stock-Media-Marketplace

## Top Stock Media Marketplace Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Self-Hosted Digital Asset Management, Royalty-Free Libraries & Decentralized Media Sharing*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Stock Media Marketplaces**. These tools provide access to royalty-free photos, videos, and graphics — either through commercial licensing marketplaces or open-source platforms where creators share media freely — with a spectrum running from per-asset licensing to fully self-hosted digital asset management systems.

**Examples** include Longpoint, UnoPim DAM, ResourceSpace, Damselfly, and ShutterSea (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, AI-powered asset organization, and transparent licensing — especially relevant as **Adobe Stock charges per-asset licensing while open-source alternatives provide unlimited assets from your own library or free sources like Unsplash and Pexels**.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **Adobe Stock** — Adobe's stock media marketplace integrated with Creative Cloud. **Subscription or per-asset licensing** with millions of photos, videos, and vectors. **Best for Adobe users** needing licensed commercial assets with integration into Photoshop and Illustrator workflows.

- **Shutterstock** — One of the largest commercial stock libraries with photos, videos, music, and 3D assets. **Subscription-based** per-download pricing. **Best for teams** needing a vast licensed catalog with enterprise licensing options.

- **Getty Images** — Premium editorial and creative stock photography with rights-managed and royalty-free options. **Per-asset licensing** at premium pricing. **Best for editorial and high-end commercial use** where exclusivity and provenance matter.

- **Unsplash** — **Free high-quality stock photos** under the Unsplash License (free for commercial use, no attribution required). **Free to use** with Unsplash+ subscription for exclusive content. **Best for creators** needing high-quality free imagery without licensing fees, though the license does not permit selling unmodified copies or building a competing service.

- **Pexels** — **Free stock photos and videos** under the Pexels License (free for commercial use, attribution appreciated but not required). **Free to use** with API access for developers. **Best for developers and creators** wanting free media with a generous API for building applications.

## Open-Source GitHub Projects

- **Longpoint** — **The AI-powered digital asset management system for building media-rich applications.** **FSL-1.1-Apache-2.0 licensed** (converts to Apache 2.0 after two years), with MIT-licensed SDK and plugins . **Self-hosted with full control** — run on your own infrastructure, bring your own AI models (Claude, GPT, open-source, or custom) . **Robust media pipeline**: upload and storage with multiple backends, automatic transcoding and thumbnail generation, secure delivery with URL signing and CDN integration, documented REST API with TypeScript SDK . **Intelligent organization**: **semantic search** using natural language rather than filenames, **automatic classification** with scene detection and tagging, multimodal understanding across images, videos, audio, and documents . **Best for teams wanting a modern, AI-native DAM** with self-hosting, API-first design, and a path to full open-source licensing.

- **UnoPim DAM** — **The open-source digital asset management solution within the UnoPim PIM ecosystem.** **Free and open-source** with no licensing costs . **Comprehensive asset management**: directory tree with search, breadcrumbs, and per-folder asset counts; explorer view with tabs, grid/list modes, bookmarks, and bulk operations; drag-and-drop and background uploads with pause/resume/cancel . **Rich previews**: zoomable images, custom video/audio players, in-browser PDF viewing, and real thumbnails for PDFs and videos . **Image editor** with crop, adjust, rotate, filter, and AI-generated background replacement . **Shared links** with expiring, revocable access for external collaborators . **AI auto-tagging** via vision-capable Magic AI platform (optional, disabled by default) . **REST API** with full coverage for assets, directories, tags, properties, comments, shares, and linked resources . **Requirements**: PHP 8.4.1+, UnoPim v3.0.x, with optional ffmpeg for video thumbnails and Imagick for SVG conversion . **Best for teams already using UnoPim** or wanting a free, feature-rich DAM with AI tagging and product-asset linking.

- **ResourceSpace** — **The veteran open-source DAM with a focus on organizational asset management.** **PHP/MySQL based**, free and open-source . **Manages digital assets** including images, videos, audio files, and design resources within a company or organization . **Deployment on CentOS/RHEL** with Apache, MariaDB, and required dependencies including ffmpeg, ImageMagick, and ExifTool . **The installation guide** covers system updates, PHP configuration (memory_limit >512M, post_max_size 512M, upload_max_filesize 512M), MariaDB setup, and database creation . **Best for organizations** wanting a mature, widely-deployed DAM with a proven track record, accepting the PHP/MySQL stack and traditional installation process.

- **Damselfly** — **The server-hosted DAM for photos and videos with AI face detection.** **GPL-3.0 licensed** . **Photo management** with thumbnail browsing by folder structure or timeline . **AI face detection** automatically detects and groups faces, letting you tag names and quickly find specific people . **Search and filter** across filenames, keywords, EXIF data, and face tags, with filtering by date, camera model, or location . **Tagging** with IPTC keywords written back to image files, individually or in bulk . **Batch export** with scaling options . **Docker deployment** via `docker pull qdraw/starsky:latest`, running on port 12837, with support for amd64, arm64, and arm/v7 (Raspberry Pi except Pi 1 and Zero) . **Best for photographers and families** wanting a self-hosted photo management system with AI face recognition and straightforward Docker deployment.

- **ShutterSea** — **The decentralized open-source Unsplash alternative.** Built at HackFS 2021, **open-source and decentralized** where photographers share images freely usable without attribution, even commercially . **Images stored on IPFS** with metadata in decentralized databases (Textile ThreadDB) . **Ceramic IDX for identity** and authorization — authors sign changes with their private key . **Uploaded images are converted to multiple sizes** and stored on IPFS via web3.storage, with CIDs and EXIF-parsed metadata stored in ThreadDB . **Best for developers exploring decentralized media sharing** where no central authority controls the library, accepting the experimental nature of the Web3 stack.

### Additional Strong Open-Source Options

- **Starsky** — **The photo management tool that runs on your server or web-space.** Free, open-source, Docker-deployable (`qdraw/starsky`) . **Acts as an accelerator to find and organize images driven by meta information** — browse and search images in your own cloud . **Damselfly is the successor project** to Starsky, with AI face detection and more active development . **Best for users wanting a lightweight, self-hosted photo DAM** with metadata-driven search, though the project has been superseded by Damselfly.
- **Phrasea** — **Open-source DAM solution from Alchemy.** **Modular platform** with Databox (main DAM module), Expose (CMS for static asset extracts), and Uploader (dedicated capture app) . **Each service consists of multiple containers** (API, client, worker, Nginx) for scalability and modularity, deployable via Docker Compose or Helm . **Best for organizations** wanting a modular, containerized DAM with separate concerns for management, publishing, and ingestion.
- **Jamā** — **Django-based media repository application from Université de Caen Normandie.** **Open-source, Python 3.13+ and Django 6** . **Projects, collections, resources, files, metadata, and access control** with JSON-RPC API and web UI . **Chunked uploads, hash-based storage, background media processing** with IIIF tiled images, HLS video generation, OCR, and ExifTool metadata extraction . **Project snapshot export and restore** for backup and migration . **Best for research and academic institutions** needing a standards-based media repository with IIIF and HDR support.

**Frameworks for building custom systems**: Combine **Longpoint** for AI-native DAM with semantic search and self-hosting, **UnoPim DAM** for a free, feature-rich DAM with product-asset linking and AI tagging, **ResourceSpace** for a mature organizational DAM with a proven deployment history, **Damselfly** for photo management with AI face recognition and Docker simplicity, and **ShutterSea** for exploring decentralized media sharing — to build a stock media or internal asset library stack tailored to your need for AI organization, product integration, or decentralization.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Stock media marketplaces and DAM tools differ significantly in licensing model, AI capability, and deployment requirements. **Commercial marketplaces (Adobe Stock, Shutterstock, Getty) charge per-asset or subscription fees** for licensed content, while **Unsplash and Pexels offer free licenses** with restrictions on resale and competing services. **Longpoint's FSL license converts to Apache 2.0 after two years** — verify the current license status before commercial deployment . **UnoPim DAM requires PHP 8.4.1+** and is part of the broader UnoPim PIM ecosystem . **ResourceSpace requires significant PHP configuration** (memory_limit >512M) and traditional LAMP stack deployment . **Damselfly is the successor to Starsky** — Starsky is no longer actively developed . **ShutterSea is a hackathon project from 2021** — evaluate maintenance activity before production use . **Self-hosting shifts responsibility to you** — storage durability, backup strategies, and media processing pipelines become your operations.
- Self-hosted open-source solutions require proper storage backend configuration (local or S3-compatible), media processing dependencies (ffmpeg, ImageMagick, ExifTool), and awareness that AI-powered features may require API keys or GPU resources.

---

**Made for creative teams, media organizations, and developers building stock media libraries and digital asset management systems they can own and control.**
Let's make stock media and asset management more open, AI-native, and licensing-transparent.
