What
===

This is a simple tool to create a VERY basic HTML demo for a mobile site using a bunch of images

How
===

To create a demo create a new directory. Lets call it moby. Create a directory called img within moby and add your images. 

Next make a routes.json file, such as the example below:

`
{
	"name": "Mobile Demo",
	"description": "A demo mobile site",
	"routes": [
				{
					"name": "news",
					"order": "home.jpg, news_list.jpeg, news_single.jpeg"
				},
				
				{
					"name": "directory",
					"order": "home.jpg, directory.jpeg, large_store.jpeg, store.jpeg"
				}
			  ]
}
`

Then change directory so that you are within the moby directory and run:

`$ moby -m demo:create`


Installation
=======

Ensure you have PHP installed as CLI. Run `php -v` to check

Download the file and make it executable

`chmod a+x moby`

Either place it in your path, or add to your path.

`echo 'export PATH=YOURPATHHERE:$PATH' >> ~/.profile`

Type `moby --help` for help.

Methods
=====

`$moby -m demo:create` - create a demo based on the routes.json file


Thanks
=====

Thanks to https://github.com/pete-otaqui/ClipClop for the library to parse the command line options