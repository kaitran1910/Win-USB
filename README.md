# Bootable Windows USB Creator for MacOS Users

This script assists MacOS users in creating a bootable USB drive for installing Windows. Ensure to follow the instructions carefully to avoid any data loss.

## Prerequisites

- MacOS machine (not tested on Linux)
- A USB drive with at least 8GB of storage
- Windows ISO file (specifically named `Win10_22H2_English_x64.iso`)

## Instructions

1. **Download the Windows ISO**:

   - Download the Windows ISO file from Microsoft's official website.
   - Rename the ISO file to `Win10_22H2_English_x64.iso` if it has a different name.

2. **Prepare the USB Drive**:

   - Insert the USB drive into your Mac.
   - Ensure there's no important data on the USB drive as the process will erase it.

3. **Run the Script**:

   - Open a terminal window.
   - Navigate to the directory containing the `installer` script.
   - Make the script executable with the following command:

     ```bash
     chmod +x installer
     ```

   - Execute the script by running:

     ```bash
     ./installer
     ```

4. **Follow the Prompts**:

   - The script will initially check for the Windows ISO in the Downloads folder. If not found, you'll be prompted to provide the full path to the ISO file.
   - You will then be prompted to select the USB disk to be used for the Windows installer. The script will list all available disks; please ensure to select the correct disk to avoid data loss.
   - If the selected disk is larger than 256GB, a confirmation will be required to continue.

5. **Completion**:
   - Once the script has completed, your USB drive will now contain the Windows installation files and is ready to use.

## Troubleshooting

- If you encounter any issues, re-run the script and ensure all the provided information is correct.
- Ensure the ISO file name and path are correct.
- Make sure the USB drive is properly inserted and recognizable by your Mac.

## TODO

- Extend support for other Windows ISO files.
- Improve error handling and provide user-friendly error messages.
- Test and possibly extend compatibility for Linux users.
- Include a feature to format the USB drive to the required format if not already formatted correctly.
