# NO THIS IS NOT MALWARE FEEL FREE TO REVERSE ENGINEER IT ( I WILL NOT SHARE THE SOURCE CODE )

# TPM-Modification
Changes MD5, SHA1 and SHA256 hash of your TPM chip.

# Prerequisites:
- Ida 8.0+
- UEFITool 0.25
If your bios doesn't allow flashing of unsigned bios versions:
- Raspberry Pi Pico H
- Female to Female jumper wires (6 for SOIC8)
- SOI8 Clip

### DO NOT USE A CHA314A PROGRAMMER! IT WILL DAMAGE YOUR SOIC8 CHIP AND THE SOUTHBRIDGE BY SENDING A TOO HIGH VOLTAGE (5v)


# Steps:
1. Download the newest bios version from your motherboard manufactuer
2. Modify the bios image provided in the following video: https://files.catbox.moe/4tpfk0.mp4 ( Mirror link: https://streamable.com/kjr73t )
3. Flash the image
4. Download the changer file included in the upload ( Comes with tpm-info checker to check if the change actually worked )
5. Test the results ( Run tpm-info.exe )

### This only changes the TPM's platform & endorsement hierarchies, Clear the TPM via windows to change storage hierarchy, this wont change MB serials.
