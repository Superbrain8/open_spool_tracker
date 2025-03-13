# Open Spool Tracker

This Project is a Loadcell Based Filament tracker running of a ESP32

## Planed Features

- Loadcell Based Weighting
- RFID Tag based Management of spools (ntag216)
- Integration into Spoolman https://github.com/Donkie/Spoolman
- I2C Screen for Display of Current Weight on the Spool

## Eventually Supported

- Webinterface for easier data input

## The Idea

This project aims to provide a way to track the content of filament on mutiple spools using inexpensive RFID tags and Spoolman
Its planned to have the RFID tags run standalone from Spoolman in the future, but for Stage 1 the Data will be mostly handled by Spoolman

### How does it work?

1. RFID Reader on the Spoolholder reads a RFID tag attached to the Spool
2. an API Request is made to Spoolman with an ID fetched from the RFID tag
3. Data Stored on the Tag and Spoolman gets crosschecked -> Missing data on the tag gets completed
4. Filament usage will get tracked by Loadcell readings and then written to spoolman

### Planed Structure of Data

the Data Structure is defined within the Open Tag Standard https://github.com/Bambu-Research-Group/RFID-Tag-Guide/blob/main/OpenTag.md

### Contact

Discord https://discord.gg/vYQKyug5Cv


### Changelog

2025.03.09 - Moved standard to open Tag
