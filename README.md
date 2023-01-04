# Image Resize Helper for MMPEG

This is a small script that makes it easier to use FFMPEG to manage resizing images in bulk. Before you can use this, you first have to install [FFMPEG](https://ffmpeg.org/).

## Showcase
### First step
[Select JPG file format to reduce](https://user-images.githubusercontent.com/53581066/210546652-ba69340e-9850-470b-a7e9-431d25a137f2.webm)

## Second step
[Set desired image width and the name for the output folder](https://user-images.githubusercontent.com/53581066/210546729-2c63854a-34eb-4814-a276-921f41045364.webm)

## Installation
Once you have FFMPEG working this is how you make this work:
- download the `image_resize.sh` file to your computer and store it in a folder for scripts in your account (for example <username>/scripts)
- make the script executable by running this comand `sudo +x ./image_resize.sh`
- check the script is working by running `./image_resize.sh`, you should get the prompt asking you to choose the image format, exit the script by presing `CTRL + C`, if you did not get the prompt asking for image format, you either misstyped something, or there is some other problem, you will have to debug that issue
- once you got the script working, it is recomended to create a symlink so you can easily run the script from anywhere on your computer
- run this command in the terminal: `sudo ln -s /path/to/where/the/file/is/located/image_resize.sh` symlinkname (replace the path to where... with actual path to the file on your machine, and symlinkname with the name of the command you with to run this util with, i use `image_resize`)
- if you do not know the path to your file, go to the folder where you script is located (with the terminal) and type: `pwd` you will get the path, and just add the file name at the end of that path
- close the terminal, and open it again, type `which symlinkname` (use the actual symlink name you created), and terminal should ouput the path to the file, if the path is correct, you should be done

## Usage
- Go to the folder with the images you want to resize
- Type `symlinkname` (use actual symlinkname you have created)
- Prompt will appear asking for fileformats
- Type the number that is in front of the option you need/want
- Confirm with Enter key
- Prompt appears asking for image width
- Enter the desired image width (number only, no px)
- Confirm with Enter key
- Prompt appears asking the name of the folder where to save the reduce images (folder will be created in the current folder)
- Type the name and confirm with Enter key
- Wait untile conversion is done
- Go to the file manager and ispect the images

## Bye
Hope you find this useful