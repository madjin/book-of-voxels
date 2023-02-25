# Archiving as glTF 2.0

###### tags: `cv`

{%hackmd @xr/dark %}

**Required**

Blender 3.3.0 https://www.blender.org/download/

**Collection**

- https://skfb.ly/oyOxO - Cryptovoxels districts 12-13-19 snapshot
- https://github.com/madjin/cryptovoxels-vr - FBX and GLB files


![](https://i.imgur.com/b77RBuX.jpg)

![](https://i.imgur.com/kL5jDtG.jpg)


| Column 1 | Column 2 |
| -------- | -------- |
| ![](https://i.imgur.com/7Z23zCU.png) | ![](https://i.imgur.com/Rn91LAF.jpg) |

![](https://i.imgur.com/sbNxVPX.jpg)

![](https://i.imgur.com/XlBVwNU.jpg)

---

## Process trial 1 (jin)

:::warning
I did things wrong the first time starting with the glTF files, keeping the documentation here for learning / showing process.
:::

**Before**

![](https://i.imgur.com/uHtExsM.jpg)

![](https://i.imgur.com/pCevZqX.jpg)


I first started with glTF 2.0 files of the districts that were exported out of Unity with the Plattar UnityGLTF plugin back in 2019.

![](https://i.imgur.com/Mq04wAQ.png)

There are two atlas textures, one default and another for when a person chose to invert the colors for the blocks. The 12-13-2019 glTF exports do not seem to have information on which one is for which so for now I'm using the default Atlas. 

| Atlas 1 (default) | Atlas 2 (Inverted) |
| -------- | -------- |
| [![](https://i.imgur.com/EWTyFUa.jpg)](https://i.imgur.com/EWTyFUa.jpg) | [![](https://i.imgur.com/lL4lGeJ.png)](https://i.imgur.com/lL4lGeJ.png) |



**Glass tiles**

Getting glass to look beautiful in the web can be tricky. The blender glTF exporter recently got updates in version 3.3 to support `KHR_materials_volume` extension, [see docs](https://docs.blender.org/manual/en/3.3/addons/import_export/scene_gltf2.html#volume).

![](https://i.imgur.com/8gESMBK.jpg)

Can tweak the glass on the Sketchfab preview too: https://help.sketchfab.com/hc/en-us/articles/202602073-Transparency

![](https://i.imgur.com/8AtSYrz.jpg)

Here's how one district looks in hyperfy: https://hyperfy.io/thecenter
![](https://i.imgur.com/Xklu9LC.png)



---

## Optimization

I was able to compress a 3D model from

**1.44 GB** down to **18.3 MB**

with 0 visual quality loss

150mb 1.7M tri model down to 3.3mb via Draco compression using http://gltf.report and can still gzip 30% to 2.1mb. Meshopt only went to 25mb and broke collision

![](https://i.imgur.com/h6Dlyxh.jpg)
https://twitter.com/dankvr/status/1583596977312641024

Only major complaints I heard about Draco is that the decoder is 100kb, which is no biggie since the difference with gltfpack / meshopt for converted voxels is substantial.

![](https://i.imgur.com/YofZCrM.png)
https://twitter.com/cryptovoxels/status/1580641383815053312
https://github.com/ephtracy/voxel-model/issues/56

---

## Wearables

Compressed

Software used:

[svox-tools](https://github.com/jel-app/svox-tools), 7zip for gzip, [7-Zip-Zstd](https://github.com/mcmilk/7-Zip-Zstd) for [brotli](https://github.com/google/brotli) method, and [gltf.report](https://gltf.report/) for Draco / Meshopt



- 2.vox: 56.5 KB
- 2.svox: 9.57 KB
  - 2.svox.gz: 383 bytes
  - 2.svox.7z:  452 bytes
- 2.glb: 149 KB
  - 2.glb.gz: 16.8 KB
  - 2.7z 13.6 KB 
  - 2-draco.glb: 8.04 KB 
    - 2-draco.glb.gz: 7.32 KB
    - 2-draco.7z: 7.36 KB
  - 2-meshopt.glb: 40.0 KB
    - 2-meshopt.glb.gz: 17.7 KB 
    - 2-meshopt.7z: 17.0 KB 



---

### Ash tests

1) gltfpack -cc -noq -tc -si 0.1 = 281mb and 38s decoding time (1.7G gpu / 30 draws)

![](https://i.imgur.com/6pOqnTl.jpg)

2) draco pulled from (1) = 27mb and 28s decoding time (looks the same) (1.7G gpu / 30 draws)




---

## Notes

![](https://i.imgur.com/pwHd0PL.png)


---

## 12-17-22 Dataset


### Glass material

Before
![](https://i.imgur.com/Q8DSKbq.png)
After
![](https://i.imgur.com/yV6BzJv.png)

Blender nodes
![](https://i.imgur.com/U9FJicH.png)

Import new district

![](https://i.imgur.com/D3dKf46.png)
![](https://i.imgur.com/UmEM1Qx.png)


Import
![](https://i.imgur.com/QUrHIYt.png)

select glass / atlas, reassign original material


## Merged vs Unmerged vertices

Testing glTF import with merge vertices on / off
![](https://i.imgur.com/MzQidnb.png)

![](https://i.imgur.com/ctJrSjQ.png)
