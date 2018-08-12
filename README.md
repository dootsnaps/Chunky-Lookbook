## Welcome to the Chunky Lookbook

*Currently WIP!*

To contribute, submit a pull request. I'll take anything that isn't already covered in this guide so long as it's not total shite.

Right now, everything is just on one page. I ~~may switch~~ am currently switching the format to multiple pages. ~~in the future (one per tab, perhaps).~~

Todo: finish the main guide, provide example scenes for download, maybe videos?

## [Tab 1: General](General.md)


  
## Tab 2: Lighting

  This tab contains the lighting settings, including the intensity of the sky, emitter, and sun lights. You can also toggle emitter and sunlight here, and change the azimuth, alititude, and color of the sunlight. Here's a screenie:
  
  <img src="https://i.imgur.com/uEKiKp0.png"  class="inline"/>
  
### Sky light:
  
  Here is our reference picture, with sky light set to the default of 1.00:
  
  <img src="https://i.imgur.com/xWXwVh2.png"  class="inline"/>
  
  With sky light set to the lowest setting (0.01):
  
  <img src="https://i.imgur.com/m0Q8SrJ.png"  class="inline"/>
  
  Notice how the shadows are quite a bit darker, because they are receiving less light.
  
  Finally, as we increase the sky light, everything will recieve more light:
  
  <img src="https://i.imgur.com/mUv9mnL.png"  class="inline"/>
  
### Emitters:
  
  *wip*
  
### Sunlight:
  
  Reference: (sunlight enabled, intensity = 1.25, altitude = 40, azimuth = -301.283, sun color is white)
  
  <img src="https://i.imgur.com/uUavbGz.png"  class="inline"/>
  
  Disabling the sunlight eliminates any shadows, leaving only light from the sky and emitters (good for nighttime-looking shots):
  
  <img src="https://i.imgur.com/MkACBAa.png"  class="inline"/>
  
  Now with sunlight enabled again, let's explore the effect of changing the sunlight intensity. Firstly, with a lowered intensity (0.379):
  
  <img src="https://i.imgur.com/6NgCgV8.png"  class="inline"/>
  
  And with a much higher intensity (2.724):
  
  <img src="https://i.imgur.com/2mG6GTM.png"  class="inline"/>
  
  Adjusting azimuth changes the sun's horizontal position in the sky, starting from 0 degrees in the east. Here is a picture with an azimuth of 180 degrees (from the west, behind the camera):
  
  <img src="https://i.imgur.com/Ah1LhYF.png"  class="inline"/>
  
  Notice how the direct sunlight is extremely bright, even though we've lowered the intensity back down to the default of 1.25.

  Now, we'll try an azimuth of 0 degrees, opposite the camera:
  
  <img src="https://i.imgur.com/PcabtyU.png"  class="inline"/>
  
  And finally, at 90 degrees (from the north, left of the camera) :
  
  <img src="https://i.imgur.com/RD9vdpd.png"  class="inline"/>
  
  Now let's look at the altitude, which is the angle in degrees that the sun sits above the horizon. Setting it to a low number (5 degrees) results in longer shadows:
  
  <img src="https://i.imgur.com/TYY4phM.png"  class="inline"/>
  
  And with a higher altitude (90 degrees) the shadows are practically non-existant, as everything is lit directly from the top:
  
  <img src="https://i.imgur.com/GOsVXHr.png"  class="inline"/>
  
  Lastly, we'll try changing the sun color. You can give it any color you like, including a subtle sunset-ish orange:
  
  <img src="https://i.imgur.com/9RuqWYS.png"  class="inline"/>
  
  Or even an outlandish green:
  
  <img src="https://i.imgur.com/EmyU6R2.png"  class="inline"/>
  
## Tab 3: Sky and Fog

  This tab allows you to set the sky mode, cloud settings, and fog settings:
  
  <img src="https://i.imgur.com/obUFgN9.png"  class="inline"/>
  
### Sky Mode  

  The first set of settings is for Sky Mode. The available options are seen is this drop-down menu:
  
  <img src="https://i.imgur.com/6wAvimX.png"  class="inline"/>
  
  Here is our reference picture, with the default settings for sky mode (simulated, horizon offset = 0.1):
  
  <img src="https://i.imgur.com/iu1PTt7.png"  class="inline"/>
  
  The horizon offset changes how high or low the simulated horizon appears in the sky. Setting it to zero raises the horizon, giving us a lighter color at the physical horizon:
  
  <img src="https://i.imgur.com/IZhmZtM.png"  class="inline"/>
  
  Raising it to 1 lowers the simulated horizon, giving us a deep blue color at the physical horizon:
  
  <img src="https://i.imgur.com/fLhZTCI.png"  class="inline"/>
  
  The next mode is Solid Color. We can set any color we want. It is important to note, at this point, that whatever mode you choose, the color and brightness of the rendered sky affects the "sky light" from the previous tab, as seen here when we choose a purple sky:
  
  <img src="https://i.imgur.com/fl6fI15.png"  class="inline"/>
  
  Up next is Color Gradient. You can choose from the available presets or make your own using the given dialog:
  
  <img src="https://i.imgur.com/goEceor.png"  class="inline"/>
  
  And the result:
  
  <img src="https://i.imgur.com/BoMkLSt.png"  class="inline"/>
  
  Next we have the two skymap modes, panoramic and spherical.
  
  <img src="https://i.imgur.com/ooKEf8t.png"  class="inline"/><img src="https://i.imgur.com/L9g35Xx.png"  class="inline"/>
 
  First, load your skymap of choice using the "Load skymap" button. Here, I've aligned the rendered sun with the sun in the skymap using the "Skymap rotation" setting. In general, you'll want to do this so that the shadows in your scene and the shadows in your skymap are coherent, even if the sun isn't actually visible in your render: 
  
  <img src="https://i.imgur.com/uWAvPoE.png"  class="inline"/>
  
  For Skybox mode, you'll need to load (up to) six textures which will each make up a face of the skybox cube:
  
  <img src="https://i.imgur.com/6xuubmI.png"  class="inline"/>
  
  Here I've chosen six random pictures. With this mode, the sky's the limit!:
  
  <img src="https://i.imgur.com/CZzwaUF.png"  class="inline"/><img src="https://i.imgur.com/1MV6tGm.png"  class="inline"/>
  
  The last mode is Black. Notice that this completely disables the Sky Light, making everything quite dark except for what's lit up by sunlight:
  
  <img src="https://i.imgur.com/aLGjTq8.png"  class="inline"/>
  
### Transparent Sky:

  Enabling this keeps all the sky lighting from the selected sky mode, but makes the actual sky transparent (black in this picture):
  
  <img src="https://i.imgur.com/Y6p8uGy.png"  class="inline"/>

### Clouds:
  Clouds look similar to the in-game Minecraft clouds, and cast shadows when struck by sunlight. Here I've made them smaller than the default and raised them up to a y-level of 250. The X and Z settings simply offset the cloud pattern in their respective directions:
  
  <img src="https://i.imgur.com/1kUQe5G.png"  class="inline"/>
  
  It should be noted that you can type in numbers into the box which exceed the bounds of the sliders, enabling you to put the clouds at, for example, a y-level of 10000 blocks:

  <img src="https://i.imgur.com/8qS5LaJ.png"  class="inline"/>
  
### Fog:

  There are three settings for fog: density, sky-fog blending, and color.

  Setting the fog density to a low value, such as 0.01, gives a nice haze effect:

  <img src="https://i.imgur.com/4fMXfwE.png"  class="inline"/>
  
  A higher number (0.05) results in thicker fog:
  
  <img src="https://i.imgur.com/vcoJbwv.png"  class="inline"/>
  
  You can use high fog density (0.2) to generate a crepuscular ray effect:
  
  <img src="https://i.imgur.com/Zhv30VL.png"  class="inline"/>
  
  The sky-fog blending level decides how much the fog should blend into the sky at the horizon. Setting it to 0 results in a  sharp disconnect between the sky and horizon:
  
  <img src="https://i.imgur.com/M2vDOSL.png"  class="inline"/>
  
  Fog color can be set to whatever you want. Darker colors can produce very interesting effects:
  
  <img src="https://i.imgur.com/Geepnri.png"  class="inline"/>
  
 
  
## Tab 4: Water

  The Water tab allows you to set water visibility (how many blocks deep can you see), opacity (how "thick" does it look), height, and color. You can also toggle Still Water (no waves) and Water World mode (surrounds the scene with an infinite ocean).
  
## Tab 5: Camera
