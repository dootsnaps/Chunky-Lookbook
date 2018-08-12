## Welcome to the Chunky Lookbook

*Currently WIP!*


## Tab 1: General

  The first tab of the render controls dialog is the "General" tab. It looks like this:
  
  <img src="https://i.imgur.com/AjaeGFx.png"  class="inline"/>
  
  On this tab you will find the main controls for rendering the scene itself, including the canvas size (resolution of the rendered picture), the Y clipping settings (for taking out a vertical "slice" of the scene"), and the Target SPP (what quality do you want to render to).
  
  At the top you'll find some buttons for scene operations (loading, saving, etc...) You can save and load render settings separately from the scene so that you could, for example, apply settings from one scene to a different one. You can also load the chunks you've selected in the main window and completely reload the scene from here.
  
  You can toggle player loading and biome colors on this page as well.
  
## Tab 2: Lighting

  This tab contains the lighting settings, including the intensity of the sky, emitter, and sun lights. You can also toggle emitter and sunlight here, and change the azimuth, alititude, and color of the sunlight.
  
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

  This tab allows you to set the sky mode, cloud settings, and fog settings.
  
## Tab 4: Water

  The Water tab allows you to set water visibility (how many blocks deep can you see), opacity (how "thick" does it look), height, and color. You can also toggle Still Water (no waves) and Water World mode (surrounds the scene with an infinite ocean).
  
## Tab 5: Camera
