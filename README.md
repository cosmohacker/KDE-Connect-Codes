Some useful codes for KDE:Connect that i use for my phone to pc connection
I hope it helps.
# //Begin::Installation

How to install KDE:Connect [PC] -> KDE:Connect Installation [PC]

How to install KDE:Connect [Android] -> KDE:Connect Installation [Android]

# //End::Installation

### Note

If there is any additional command you want, I will add it.

This code on reddit - > [reddit](https://www.reddit.com/r/linux/comments/y6mfnw/some_useful_codes_for_kdeconnect_that_i_use/?utm_source=share&utm_medium=android_app&utm_name=androidcss&utm_term=1&utm_content=share_button "reddit"

|   |   |
| ------------ | ------------ |
|  Title | Code  |
| Close All Vaults  | qdbus org.kde.kded5 /modules/plasmavault closeAllVaults |
| Forcefully Close All Vaults  |  qdbus org.kde.kded5 /modules/plasmavault forceCloseAllVaults |
|  Kill all process and logout | killall -u cosmohacker  |
| Maximum Brightness  |  qdbus org.kde.Solid.PowerManagement /org/kde/Solid/PowerManagement/Actions/BrightnessControl org.kde.Solid.PowerManagement.Actions.BrightnessControl.setBrightness qdbus org.kde.Solid.PowerManagement /org/kde/Solid/PowerManagement/Actions/BrightnessControl org.kde.Solid.PowerManagement.Actions.BrightnessControl.brightnessMax |
|Minimum Brightness   | qdbus org.kde.Solid.PowerManagement /org/kde/Solid/PowerManagement/Actions/BrightnessControl org.kde.Solid.PowerManagement.Actions.BrightnessControl.setBrightness 0  |
|  Reboot | systemctl reboot  |
| Suspend  | systemctl suspend  |
|  Unlock Screen | loginctl unlock-session  |
|Cancel Shutdown   |  shutdown -c |
| change webcam shot names  |  for f in /home/cosmohacker/Documents/*.png; do mv "$f" "$(echo "$f" |
|  delete audio records |  rm --force /home/cosmohacker/Music/* |
| delete screenshots  | rm --force /home/cosmohacker/Pictures/*  |
 |delete video records |	rm --force /home/cosmohacker/Videos/* |
 |delete webcam shots |	rm --force /home/cosmohacker/Documents/* |
 |empty trash |	rm -rf ~/.local/share/Trash/* |
 |lock screen |	qdbus org.freedesktop.ScreenSaver /ScreenSaver Lock |
 |mute/unmute |	amixer sset Master toggle |
 |record audio 10 min |	sox -t alsa default /home/cosmohacker/Music/$(date "+%Y%m%d_%H%M%S")audio.wav trim 0 600 |
 |record audio 30 sec |	sox -t alsa default /home/cosmohacker/Music/$(date "+%Y%m%d_%H%M%S")audio.wav trim 0 30 |
 |record audio 5 min |	sox -t alsa default /home/cosmohacker/Music/$(date "+%Y%m%d_%H%M%S")audio.wav trim 0 300 |
 |record video 10 min |	ffmpeg -f alsa -f video4linux2 -s 320x240 -i /dev/video0 -t 600 /home/cosmohacker/Videos/$(date "+%Y%m%d_%H%M%S")out.mpg |
 |record video 30 sec |	ffmpeg -f alsa -f video4linux2 -s 320x240 -i /dev/video0 -t 30 /home/cosmohacker/Videos/$(date "+%Y%m%d_%H%M%S")out.mpg |
 |record video 5 min |	ffmpeg -f alsa -f video4linux2 -s 320x240 -i /dev/video0 -t 300 /home/cosmohacker/Videos/$(date "+%Y%m%d_%H%M%S")out.mpg |
 |send audio to phone |	for FILE in /home/cosmohacker/Music/*.wav;do kdeconnect-cli -d $(kdeconnect-cli -a --id-only) --share echo $FILE;done |
 |send screenshots to phone |	for FILE in /home/cosmohacker/Pictures/*.png;do kdeconnect-cli -d $(kdeconnect-cli -a --id-only) --share echo $FILE;done |
 |send video records to phone |	for FILE in /home/cosmohacker/Videos/*.mpg;do kdeconnect-cli -d $(kdeconnect-cli -a --id-only) --share echo $FILE;done |
 |send webcam shot to phone |	for FILE in /home/cosmohacker/Documents/*.png;do kdeconnect-cli -d $(kdeconnect-cli -a --id-only) --share echo $FILE;done |
 |shutdown |	shutdown |
 |spotify |	spotify |
 |take screenshot |	import -window root /home/cosmohacker/Pictures/$(date "+%Y%m%d_%H%M%S")screenshot.png |
 |volume down -10 |	amixer set Master 10%- |
 |volume down -5 |	amixer set Master 5%- |
 |volume up +10 |	amixer set Master 10%+ |
 |volume up +5 |	amixer set Master 5%+ |
 |webcam shot 	 |mplayer -vo png:outdir=/home/cosmohacker/Documents -frames 10 tv:// |

