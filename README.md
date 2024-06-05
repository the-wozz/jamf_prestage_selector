# jamf_prestage_selector
GUI (Swift Dialog) Jamf Pro tool for viewing and changing pre-stages of a device

What does it do?
Shows a selectable list of 'pre-stages' for a device WITHIN its current ABM instance.

How to use:
Enter the serial number of a device that you would like to view the current ABM instance or pre-stage and press 'Return' or click 'Submit'

The tool will then search through ALL Apple Business Manager (ABM) instances of the Jamf Pro environment. 

If the serial number inputted is found, the tool will return a window with available Pre-Stages to select from. Only one 'Pre-Stage' can be selected and then pressing 'Submit'.
A confirmation window will be shown next, this is to ensure the correct selection was made. Confirm the selection and the script will then go about removing its current 'Pre-Stage' and then adding the new desired 'Pre-Stage'. A success window will be shown if the device was sucessfully added. Likewise, for a failure to add.

You will have 60 seconds to make a selection, if no decision is made within 60 seconds, the submission will error. THIS IS BY DESIGN to ensure security. Please ONLY run the tool when a change (or viewing of the current ABM instance and pre-stage) is to be done right away.

If the serial number CAN NOT be found in any ABM instance, you will recieve an error message. Contact an ABM Admin for further steps.

Notes:
You will ONLY be shown 'Pre-Stages' that are available to the SPECIFIC Apple Business Manager (ABM) instance the device is found in! (Visible at the top of the result window)
Example, two 'Pre-Stages' could have very similar names, but the ABM instance takes precendence of the 'Pre-Stages' shown
