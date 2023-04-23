# URP Anaglyph3D
 Anaglyph 3D (red/cyan) render feature for Unity's URP

![Sample Image](images~/sample.jpg)

## Requirements
Anaglyph3D [v2](https://github.com/ryanslikesocool/Anaglyph3D/releases/tag/v2.1.1) requires Unity 2021.3 with URP 12.1.8 or later.
Anaglyph3D [v3](https://github.com/ryanslikesocool/Anaglyph3D/releases/tag/v3.0.0) requires Unity 2022.1 or later with URP 13.1.7 or later.

## Install
**Recommended Installation** (Unity Package Manager)
- "Add package from git URL..."
- `https://github.com/ryanslikesocool/Anaglyph3D.git`

**Alternate Installation** (not recommended)
- Get the latest [release](https://github.com/ryanslikesocool/Anaglyph3D/releases)
- Import into your project's Plugins folder

## Usage
In your Forward Renderer asset, add the "Anaglyph Feature" render feature and change settings as desired.

| Property | Information |
| ----- | ----- |
| Pass Event | Leave at `Before Rendering Post Processing` for best results. |
| Layer Mask | Which layers to include when rendering the effect. |
| Spacing | The spacing between the red and cyan channels.  This value may need to be larger for orthographic cameras. |
| Look Target | The focal point, represented as units in front of the camera. |
| Opacity Mode | Which opacity mode to use when composing the final image. |
| Overlay Effect | Overlay (true) or replace (false) the effect on the final image.  Enable this if the effect should only affect some objects/layers, and not the whole screen. |
| Shader | The anaglpyh shader, located at the root directory of the package. |
