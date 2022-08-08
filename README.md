# ios16textview
ios 16 uitextview bug

Adding text through uitextview text property have strange effect in ios 16.
Have: uitextview with some text that longer than uitextview height.
The end of text is visible (so the start of the text is not visible).
Testing: Add some string ("a") to the end of the uitextview programatically (txtView.text = txtView.text + "a").
Expected: The txtView shows the the old text + "a"
Observed: After one or two adding the "a" upper part of the old text disappeared from the textview.
After tapping in the textview the the text will appear (is visible again).
I have attached the small project with uitextview and two buttons: button left and button right.
Button right - adding the letter "a" to the end of the text.
Button left - simply removes the soft keyboard if it appears.
This project works correct in ios 15 (emulator and real device) and works wrong in ios 16 (emulator and real device)
