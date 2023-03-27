#!/bin/bash

if [ $# -eq 0 ]; then
    echo "Pam is a searching utility made for pacman to ease searching packages"
    exit 0
fi

while getopts "s:S:" opt; do
    case "$opt" in
        S)
            \pacman -Ssq | grep "$OPTARG"
            ;;
        s)
            \pacman -Qsq | grep "$OPTARG"
            ;;
        *)
            echo "Invalid option: -$OPTARG"
            exit 1
            ;;
    esac
done
