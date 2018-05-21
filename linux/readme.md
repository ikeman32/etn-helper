# Linux scripts for Electroneum

scripts:

detach.sh run electroneumd in detached mode

dhelp.sh show the electroneumd help without starting the deamon

dversion.sh show the current version of the electroneumd

export.sh export the current blockchain database on your system

import.sh import the blockchain.raw file you downloaded assumes the file is located in the export folder of the electroneum data folder. ".electroneum/export"

mine-etn.sh starts the electroneumd deamon and begins using the builtin cpu miner. In order for you to use this you must edit the script but only the parts labeled [wallet-address] and [num]. Just copy and paste the wallet address you want to mine to over the [wallet-address] place holder, be sure to paste over the brackets too. For [num] just replace it with the number of cpus you want to mine with. If you have a quadcore cpu you can go up to 4, etc.

salvage.sh If you ever start the electroneumd deamon and you get a segmentation error which can happen if you fail properly shutdown the deamon properly, this can recover from that so you don't have to delete your database and resync the whole blockchain.

make.sh This just makes all the scripts executable on linux system it simply runs the command chmod +x *.sh. To run it just type bash make.sh and all scripts will be instantly made executable so from now on to run a script you simply type ./scriptname.sh and hit enter.

Usage:

These scripts should be copied into the folder with the ETN applications reside and should all be made executable by either running bash make.sh or chmod +x *.sh. If you have installed ETN to run natively in your system when you open a terminal, then these scripts should run natively as well. Otherwise you will have to navigate to the folder where the applications reside and open a terminal in that folder to run them.

To do:
Get the mine-etn.sh script to prompt for an etn wallet address and number of threads and detect if those have been entered before then use those settings.
