SpaceBlender Pipeline for the command line
Download the latest plugin from https://github.com/SpaceBlender/SpaceBlender
or by going to our website http://www.cefns.nau.edu/capstone/projects/CS/2014/SpaceBlenders/
The name of the folder has changed to SpaceBlender. If the downloaded folder has the
name SpaceBlender-master or any other name change it before adding it to Blender.
For the pipeline to work the folder placed in Blender **must** be name SpaceBlender
Place this script in any directory you want and cd into that directory with the
command line. Place your DEM image into that directory and then run the pipeline
according to these instructions

To use the SpaceBlender Pipeline your command should look like:
blender -b -P space_blend.py test_dem.IMG

Default settings are: Linear Flyover, Saturated Rainbow color pattern, 1080p

You can add options in any order and they are case insensitive

Available options include flyover patterns, colors, resolution, stars, and mist

Here are the options:
Flyover patterns:
		['noflyover', 'linear', 'circle', 'diamond']
Available colors:
			['NoColorPattern',
                        'Rainbow_Saturated',
                        'Rainbow_Medium',
                        'Rainbow_Light',
                        'Blue_Steel',
                        'Earth',
                        'Diverging_BrownBlue',
                        'Diverging_RedGray',
                        'Diverging_BlueRed',
                        'Diverging_RedBrown',
                        'Diverging_RedBlue',
                        'Diverging_GreenRed',
                        'Sequential_Blue',
                        'Sequential_Green',
                        'Sequential_Red',
                        'Sequential_BlueGreen',
                        'Sequential_YellowBrown']

Resolutions:
		['180p', '360p', '480p', '720p', '1080p']

A sample command with options could look like:
blender -b -P space_blend.py test_dem.IMG 480p Linear Stars Mist
blender -b -P space_blend.py test_dem.IMG circle 720p stars

If you choose to not do a flyover a still image will be saved to the current directory.
A command for no flyover can look like:
blender -b -P space_blend.py test_dem.IMG 720p stars noflyover