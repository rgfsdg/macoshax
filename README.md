# macoshax
so youve got your brand new macbook pld from sst. what now? well i havent got much tutorials yet but this is my first one.
# admin. this wont work if ur recovery is locked  (for ventura and below)
so u want admin but the school and parents dont allow you. well screw them. this is how u get admin access:
step 1: power off your macbook
step 2: press and hold your power button. a text appears (loading startup options)
step 3: press and hold your power button until the options come up.
step 4: select options and you should see the apple logo with the spinning beachball
step 5: once the macos recovery loads click utilities in the toolbar and press terminal.
step 6: here comes the hard part: type ```cd /volumes``` then ```cd macintosh\ hd``` after that ```cd var\db```
step 7: removing ```rm .applesetupdone```
step 8: reboot ```reboot```
step 9: go through the macos setup. **your existing data is not erased** create an account with name admin and passwd admin123.
step 10: login with the username admin
step 11: go to settings and click users & groups. then click the "i" icon near your student account.
step 12: now allow the user to administer the computer. turn it on
step 13: shutdown your laptop and turn on
step 14 (optional): remove the admin account by doing step 11 but instead click the admin one. then delete user. delete home folder.
step 15: shutdown your laptop and turn on
step 16: make sure the admin account is gone and login to your student account.
step 17: 😆

# for sonoma and above (this wont work if ur recovery is locked)
step 1: power off your macbook
step 2: press and hold your power button. a text appears (loading startup options)
step 3: press and hold your power button until the options come up.
step 4: select options and you should see the apple logo with the spinning beachball
step 5: once the macos recovery loads click utilities in the toolbar and press terminal.
step 6: here comes the hard part: type ```cd /volumes``` then ```cd macintosh\ hd``` after that ```etc```
step 7: change sudoers by typing ```chmod 645 sudoers```
step 8: modify file ``` vi sudoers```
step 9: scroll down using arrow buttons to the part ``` # root and users in group wheel can run anything on any machine as any user ```
step 10: below %admin press esc and the press capital A and enter
step 11: now type in like this ``` testuser       ALL = (ALL) ALL ```
step 12: change testuser to your username E.G test user will become testuser
step 13: press esc and then type :wq
step 14: type reboot
step 15: once into macos open up terminal and type ```sudo su ``` type in ur password
step 16:  and then type ``` dscl . -append /Groups/admin GroupMembership testuser ``` remeber to change to ur username
step 17: type reboot and make sure ur admin by going into settings and users and groups.
step 18: if they find out and remove ur admin you can get it back by executing steps 15 - 17. ur admin is permanantly hardcoded
now u got admin


