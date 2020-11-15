# Mi-Band-Tasker-Automation

Apps - Tasker, Notify for Mi Band, Mi Band Tools (Optional)

# Menu-

I have used "Mi Band Tools" to trigger an event when a gesture is performed and on the basis of the number of the gesture_count, I decide what to do. You can replace that with "Notify for Mi Band" too, I just felt "Mi Band Tools" was easy to implement in this particular case with no restrictions.

The Menu is displayed when you perform 2 swipe gestures.

# Menu Items -


1) *Battery* - Display the mobile battey% on my band. If mobile is charging we get a "+" symbol.

Example - If not charging - 30%

If charging - 30%+

2) *Alarm* - Set alarm for MI band from the band itself (band needs to be connected to the mobile, you also need to have Notify for Mi Band). The trick is to set a silent mobile alarm and get the alarm alert on the band. We need to enable the "Clock app" option in alarm settings in the Notify app and set alarm in "Google Clock" using the media buttons on the band. We also have to enable the Play, Next, and Previous track actions in the Notify button section in the app. This will send the media button intents to the tasker which we can later use to set our alarm.

Once done -

The previous media button is used to select the tens digit of hours (0x,1x, or 2x, the input format is 24 hours) or minutes(0x,1x,2x,3x,4x, or 5x). The band also gives a vibration alert to let you know when the button is pressed and a double vibration alert when trying to enter something not possible like 25 hours.

The next media button is used to select the one's digit of hours or minutes.

The play media button is used to select the option.

I also have a "Set Band Alarm" profile in the project which is what I'm currently working on - Use Google assistant and auto voice to set the MI band alarm.

Remember the alarm won't' be shown in the band's alarm section and you'll still need connectivity to the mobile phone. It basically allows you to set a mobile alarm that is notified on your band.

3) *Google Assistant* - Triggers google assistant

4) *Exit* - Exit the menu mode. You can also use 4 swipe gesture anytime (without using the 2 swipe gesture before it) to trigger the exit profile.

The custom menu project uses "Set Alarm" to set the alarm.

For more info refer to my Reddit post - https://www.reddit.com/r/miband/comments/jqafea/mi_band_tasker_awesome/
