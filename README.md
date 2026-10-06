# Organic Humanoid Head / MetalMask

**Procedural modeling and fluid tests in Houdini. Maison d’Atelier.**

![Houdini crease-weight inspection](media/images/houdini-crease-weights.webp)

A Houdini study in porous geometry, viscous fluid and dark materials. The aim is to push the surface without losing the face.

## References

![Bone-like structural diagram with vector traces and a porous shell](media/images/reference-porous-structure.jpg)

<sub>Structural reference via <a href="https://i.pinimg.com/1200x/c7/33/46/c7334632abbf40ce4c7e9c8b8be9a52b.jpg" rel="nofollow">Pinterest</a>; original designer and publication unverified.</sub>

## Geometry and Lighting Tests

![Open ribs beside a denser shell](media/images/early-shell-pair.webp)
![Shell comparison inside Houdini](media/images/houdini-shell-comparison.webp)
![Pale solid-shell inspection](media/images/houdini-solid-shell.webp)

Early geometry tests, moving between open ribs and a denser shell.

![Early edge-light test](media/images/edge-light-test-1.webp)
![Second edge-light test](media/images/edge-light-test-2.webp)

Lighting tests before committing to the final material. Leaving parts of the face in shadow makes the portrait more interesting.

## 01 / Procedural Modeling

A point wrangle for checking `creaseweight`, transcribed from the project capture:

```vex
@Cd.x = @creaseweight;
@Cd.y = 1-@creaseweight;
@Cd.z = 0;
```

For weights from 0 to 1, this maps green to red. It makes the attribute much quicker to check in the viewport.

![Assembled porous form in Houdini](media/images/houdini-volume-assembly.webp)
![Houdini shell viewport and network — Screenshot 2026-04-19 014613](media/images/houdini-shell-2026-04-19-014613.webp)

The setup combines scattering, VDB operations and crease-weight transfers. Keeping those stages separate makes the geometry easier to inspect.

## 02 / Clay Renders

![Pale skull study](media/images/skull_view_1.webp)

Clay checks before shading. If the face needs reflections to work, the geometry still needs attention.

<a href="docs/media-index.md#images">More geometric and clay views</a>

## 03 / Fluid Simulation

![Full coating experiment](media/gif/coating-viscosity-2-8.gif)

Viscosity and contact tests on the head. The useful comparison is how long the coating holds together before it starts to drip.

<a href="media/video/coating-viscosity-2-8.mp4">Full coating clip</a> · <a href="media/video/viscous-mask.mp4">viscous mask</a> · <a href="media/video/driplets.mp4">driplets</a> · <a href="media/video/immersion.mp4">immersion</a>

## 04 / Surface Tests

<a href="media/video/bubbles-closeup-1.mp4">Close-up 1</a> · <a href="media/video/bubbles-closeup-3.mp4">close-up 3</a>

## 05 / Simulation Playblasts

Rough playblasts for viscosity, adhesion and vorticity. These are working tests, with the original viewport framing.

<a href="media/video/rough-viscosity-by-12.mp4">Viscosity by 12</a> · <a href="media/video/rough-adhesion-capture.mp4">adhesion capture</a> · <a href="media/video/rough-vorticity-droplets.mp4">vorticity / droplets</a> · <a href="media/video/rough-playbook-capture.mp4">rough playbook</a>

For the adhesion tests: <a href="media/video/adhesion-viewport-001.mp4">001</a>, <a href="media/video/adhesion-viewport-002.mp4">002</a>, <a href="media/video/adhesion-viewport-003.mp4">003</a>.

## 06 / Texturing and Lighting

![Substance material study — Screenshot 2022-10-16 134815](media/images/substance-material-2022-10-16-134815.jpg)

![Dark head detail](media/images/final-detail.webp)

The final material is about catching just enough light. A few sharp reflections do more for the portrait than lighting every cavity.

<a href="media/video/final-organic-head.mp4">Final organic-head motion</a> · <a href="media/video/metalmask-portrait.mp4">MetalMask portrait motion</a>

## Files

[Media](docs/media-index.md) · [Source notes](docs/media-manifest.json) · [Archive details](docs/audit-notes.md)

---

![Portfolio — metalmask cover](media/portfolio/metalmask-cover.webp)

![Portfolio — metalmask gallery](media/portfolio/metalmask-gallery.webp)

![Portfolio — metalmask comparison](media/portfolio/metalmask-comparison.webp)

![Portfolio — organic head cover](media/portfolio/organic-head-cover.webp)

![Portfolio — organic head gallery](media/portfolio/organic-head-gallery.webp)
