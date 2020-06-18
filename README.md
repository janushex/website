# Dungeon Cube website
Testing option of wordpress + export to static -> hosted on GitHub Pages.

### How to create website in wordpress and host it on GitHub Pages like I did?
1. Install XAMPP (if you are using Windows or MAMP for Macs) and Wordpress or your PC. [How to install XAMPP and Wordpress (pl)](https://blog.lh.pl/jak-zainstalowac-wordpressa-na-swoim-komputerze-xampp/).
2. Download [this](https://github.com/grrr-amsterdam/simply-static) fork of _Simply Static_ plugin and put its directory in c:\xampp\htdocs\wordpress\wp-content\plugins\ (if you are using Windows). Unfortunatelly original _Simply Static_ plugin is not compatible with PHP 7.3 used in latest Wordpress version.
3. When XAMPP (Apache + MySQL) is launched on your PC, go to [http://127.0.0.1/wordpress/wp-admin/](http://127.0.0.1/wordpress/wp-admin/) and create a Wordpress site on your local PC. You can use this [Guide](https://websitesetup.org/), from Step #4. 
4. Create a new GitHub repository and clone it to some directory on your PC.
5. Go to Settings of _Simply Static_ plugin in left menu of Wordpress:
	- Destination URLs = Use absolute URLs (this is a must!)
	- Delivery Method = Local Directory
	- Local Directory = path to your local directory with just cloned git repository
6. Go to Generate of _Simply Static_ plugin and press Generate Static Pages button. After some time they should be ready. 
7. Go to the output Local Directory and check it that site works fine offline. If so, you can commit and push changes to your GitHub repo.
8. Go to Settings of your GitHub repo, scroll down to GitHub Pages and enable that option. 
Congratulations! You have just published static wordpress site on GitHub Pages!