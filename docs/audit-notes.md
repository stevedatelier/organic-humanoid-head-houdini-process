# Audit and selection notes

[Back to the case study](../README.md)

## Scope

The confirmed set contains House of Fireborn, Back to My Roots, and Organic Humanoid Head / MetalMask. Palm is excluded at the ownerâ€™s request. The two head pages describe overlapping material and are represented by one repository.

The audit recursively covered the supplied Fireborn process folder, chair screenshots, every folder in `playblast_files_folders_links.txt`, the project pages and their local asset folders. Review included movie metadata and sampled frames, numbered-sequence detection, sample comparisons with existing videos, and inspection of process screenshots.

## Evidence and exclusions

- The separate `REEL01_Knitting / SC030` branch contains cloth camera experiments, Vellum captures and six AVI files. It was audited, but no reliable attribution to these four projects was established; its footage is excluded from their narratives. This includes 425 MiB AVIs and numerous similar camera paths.
- Automata is outside the confirmed scope. Sparse numbered hero stills and separate clay viewpoints are not treated as animation.
- Repeated movie copies were identified by SHA-256. The Fireborn collection duplicates nine movies in the linked R&D directories; each selected movie is included once.
- The charcoal JPG batch matches its 93-frame AVI. The coating JPG batch matches its 136-frame movie. Existing movies were used, with delivery compression, rather than rebuilding these sequences.
- The incomplete `Viscosity_By_8.avi` cannot be decoded. Its numbered `.pic` batch was recoverable through Houdini `iconvert` and is included in the head repository.
- Movie frame rates are preserved. 24 fps is the documented review assumption for newly encoded image sequences, based on adjacent playblasts. No scene FPS was recovered directly.
- Masters, Houdini scenes and caches remain in their original locations. This repository is a process-media case study, not a reproducible simulation project.

## New sequence encodes

| Review | Original batch | Frames | FPS |
|---|---|---:|---:|
| [surface-transformation-render](../media/video/surface-transformation-render.mp4) | `D:\SELF\WORKING_FILES\REEL01_Metamask\REEL01_ANIMATION\A_PROJ\HOUD\R&D\HoudiniProjects\Metamask_LiquidDrop_01\LiquidDrop\flip\untitled{frame}.jpg` | 1â€“129 (129) | 24 |
| [rough-playbook-capture](../media/video/rough-playbook-capture.mp4) | `D:\SELF\WORKING_FILES\REEL01_Metamask\REEL01_ANIMATION\A_PROJ\HOUD\R&D\HoudiniProjects\Metamask_LiquidDrop_01\LiquidDrop\flip\Playbook_2\untitled{frame}.pic` | 1â€“105 (105) | 24 |
| [rough-adhesion-capture](../media/video/rough-adhesion-capture.mp4) | `D:\SELF\WORKING_FILES\REEL01_Metamask\REEL01_ANIMATION\A_PROJ\HOUD\R&D\HoudiniProjects\Metamask_LiquidDrop_01\LiquidDrop\flip\PL_Fl_Adhesion\untitled{frame}.pic` | 1â€“100 (100) | 24 |
| [rough-viscosity-by-12](../media/video/rough-viscosity-by-12.mp4) | `D:\SELF\WORKING_FILES\REEL01_Metamask\REEL01_ANIMATION\A_PROJ\HOUD\R&D\HoudiniProjects\Metamask_LiquidDrop_01\LiquidDrop\flip\PL_Fl_Adhesion_Viscosity_Tests\PL_FL_Adhesion_viscosity-by-12\untitled{frame}.pic` | 1â€“250 (250) | 24 |
| [rough-viscosity-by-8](../media/video/rough-viscosity-by-8.mp4) | `D:\SELF\WORKING_FILES\REEL01_Metamask\REEL01_ANIMATION\A_PROJ\HOUD\R&D\HoudiniProjects\Metamask_LiquidDrop_01\LiquidDrop\flip\PL_Fl_Adhesion_Viscosity_Tests\PL_FL_Adhesion_viscosity-by-8\untitled{frame}.pic` | 1â€“250 (250) | 24 |
| [rough-vorticity-droplets](../media/video/rough-vorticity-droplets.mp4) | `D:\SELF\WORKING_FILES\REEL01_Metamask\REEL01_ANIMATION\A_PROJ\HOUD\R&D\HoudiniProjects\Metamask_LiquidDrop_01\LiquidDrop\flip\Vorticity_n_Droplets\untitled{frame}.pic` | 1â€“250 (250) | 24 |

## Delivery

H.264, yuv420p, fast-start MP4; source aspect ratio retained, up to 1920 Ã— 1080. Images are web delivery copies, resized only above 2800 pixels; larger PNGs in the head, chair and Palm archives use high-quality WebP compression. Most GIFs are 640 pixels wide; the noisy HQ transformation preview uses 480 pixels and 8 fps. Compression settings and file checksums are recorded in the manifest.

## Larger source files

| Source | Original | Delivery |
|---|---:|---:|
| `Mercury_Viscosity1.mov` | 65.43 MiB | [2.34 MiB](../media/video/mercury-viscosity-1.mp4) |
| `Bubbles_Closeup_1.mov` | 61.75 MiB | [4.48 MiB](../media/video/bubbles-closeup-1.mp4) |
| `FLuid_compressed_cache_visc2-8_gridscale2_Best.mov` | 239.06 MiB | [0.86 MiB](../media/video/coating-viscosity-2-8.mp4) |
| `Mercury_Viscosity2_Alt.mov` | 80.64 MiB | [3.05 MiB](../media/video/mercury-viscosity-2-alt.mp4) |
| `Rand_visc2-8.mov` | 77.34 MiB | [0.52 MiB](../media/video/random-viscosity-2-8.mp4) |

## Added imagery

The source folders were re-inspected after 35 files were added. Earlier head shell/lighting captures were assigned to the combined head repository by subject, despite being placed in the Fireborn source folder. Foundry and structural reference images are clearly labeled as supplied references; they are not represented as original project renders. The foundry-concept filename labels that reference as AI-generated.

## Artist-identified inspiration update

The supplied references are now captioned as artist-identified inspiration, with [source records and attribution status](references.md). Unverified authorship remains explicitly marked.
