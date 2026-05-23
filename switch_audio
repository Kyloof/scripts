#!/bin/bash

wpctl set-default "$1"

for i in $(wpctl status | grep -oP '\d+(?=.*sink-input)'); do
	wpctl move-sink-input "$i" "$1"
done
