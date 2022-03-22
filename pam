#!/usr/bin/env python3

                        ########## PAM #############

if __name__ == "__main__":
    import os, sys, getopt
    if len(sys.argv) == 1:
    	print("Pam is a searching utillity made for pacman to ease searching packages")
    argv = sys.argv[1:]

    try:
        opts, args = getopt.getopt(argv, "r:i:l:L:s:")

    except:
        print("Error")

    for opt, package in opts:
        if opt in ['-r']:
            os.system("pacman -Qsq ^" + package + " | sudo pacman -Rs -")
        elif opt in ["-i"]:
            os.system("pacman -Ssq ^" + package + " | sudo pacman -S --needed -")
        elif opt in ['-l']:
            os.system("pacman -Qsq ^" + package)
        elif opt in ["-L"]:
            os.system("pacman -Ssq ^" + package)
        elif opt in ["-s"]:
            os.system("pam -L '' | grep " + package)







