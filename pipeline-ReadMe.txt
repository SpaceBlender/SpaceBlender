SpaceBlender Pipeline for the command line
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