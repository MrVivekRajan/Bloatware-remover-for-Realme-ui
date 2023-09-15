@echo off
title Realme bloatware remover
color F
chcp 65001
echo Checking connected device...
@echo off
:start0
for /f %%c in ('adb devices') do set device=%%c
:: echo "%device%" goto start
if "%device%" == "List" (
echo NO Connected Device!
goto error
pause
) ELSE (
echo Find Device %device%

)
pause
:start
echo -                                                                  -    
echo -                              BY                                  -                                                                  
echo -                          VIVEK_RAJAN                             -                                                               
echo --------------------------------------------------------------------
echo -                Realme Bloatware Remover tool                     -
echo --------------------------------------------------------------------
echo -            This tool includes all the application                -
echo -                      from ui 1.0 - 4.0                           -
echo --------------------------------------------------------------------
echo -           Now You can select the apps according to your          -
echo -               choice which you want to uninstall                 -
echo -                          or disable.                             -
echo --------------------------------------------------------------------
echo -                                                                  -
echo -                                                                  -
echo --------------------------------------------------------------------

echo 1. Uinstall Apps 
echo 2. Disabe Apps (some ui 4.0 apps which cannot be uninstalled)

:menu
set /p input="Choose any number either 1 or 2 according to your choice:  "
if "%input%"=="1" goto 1
if "%input%"=="2" goto 2

:1
:start1

echo 3. Realme UI applications 
echo 4. Google applications 

:menu
set /p input="Choose any number either 3 or 4 according to your choice:  "
if "%input%"=="3" goto 3
if "%input%"=="4" goto 4
goto start


:3
:start3
echo --------------------------------------------------------------------------------------
echo -                                Realme UI applications                      -
echo -                                   Applicaions List:                                -
echo -                   Choose the applications which you want to remove                 -
echo --------------------------------------------------------------------------------------
echo a. Realme Browser
echo b. Compass
echo c. Games
echo d. GameSpace
echo e. Phone Manager
echo f. FinShell Pay
echo g. Clone phone
echo h. Search box
echo i. Theme store
echo j. File Manager
echo k. Video
echo l. Music
echo m. Photos
echo n. Heytap Cloud
echo o. Hot apps
echo p. ORoaming
echo q. Clock
echo r. Calculator
echo s. Recorder
echo 0. Go to Main Menu

set /p c="Choose which application to delete?: "
if "%c%"=="a" goto browser 
if "%c%"=="b" goto compass
if "%c%"=="c" goto games
if "%c%"=="d" goto gamespace
if "%c%"=="e" goto phonemanager
if "%c%"=="f" goto finshell
if "%c%"=="g" goto clonephone
if "%c%"=="h" goto searchbox
if "%c%"=="i" goto themestore
if "%c%"=="j" goto filemanager
if "%c%"=="k" goto video
if "%c%"=="l" goto music
if "%c%"=="m" goto photos
if "%c%"=="n" goto cloud
if "%c%"=="o" goto hotapps
if "%c%"=="p" goto oroaming
if "%c%"=="q" goto clock
if "%c%"=="r" goto calculator
if "%c%"=="s" goto recorder
if "%c%"=="0" goto ext

:browser
echo ----------------------------------------------------------
echo -                     Realme Browser                     -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.heytap.browser 
if "%c%"=="2" echo The application is not affected!
goto start3

:compass
echo ----------------------------------------------------------
echo -                     Compass                            -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.coloros.compass2 
if "%c%"=="2" echo The application is not affected!
goto start3

:games
echo ----------------------------------------------------------
echo -                      Games                             -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.oplus.games 
if "%c%"=="2" echo The application is not affected!
goto start3

:gamespace
echo ----------------------------------------------------------
echo -                     GameSpace                          -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.coloros.gamespaceui 
if "%c%"=="2" echo The application is not affected!
goto start3

:phonemanager
echo ----------------------------------------------------------
echo -                     Phone Manager                      -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.coloros.phonemanager 
if "%c%"=="2" echo The application is not affected!
goto start3

:finshell
echo ----------------------------------------------------------
echo -                     FinShell Pay                       -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.finshell.fin 
if "%c%"=="2" echo The application is not affected!
goto start3

:clonephone
echo ----------------------------------------------------------
echo -                     Clone phone                        - 
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.coloros.backuprestore 
if "%c%"=="2" echo The application is not affected!
goto start3

:searchbox
echo ----------------------------------------------------------
echo -                     Search box                         -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.oppo.quicksearchbox 
if "%c%"=="2" echo The application is not affected!
goto start3

:themestore
echo ----------------------------------------------------------
echo -                     Theme store                        -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.heytap.themestore 
if "%c%"=="2" echo The application is not affected!
goto start3

:filemanager
echo ----------------------------------------------------------
echo -                    File Manager                        -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.coloros.filemanager 
if "%c%"=="2" echo The application is not affected!
goto start3

:video
echo ----------------------------------------------------------
echo -                     Video                              -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.coloros.video 
if "%c%"=="2" echo The application is not affected!
goto start3

:music
echo ----------------------------------------------------------
echo -                     Music                              -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.heytap.music 
if "%c%"=="2" echo The application is not affected!
goto start3

:photos
echo ----------------------------------------------------------
echo -                     Photos                             -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.coloros.gallery3d 
if "%c%"=="2" echo The application is not affected!
goto start3

:cloud
echo ----------------------------------------------------------
echo -                     Heytap Cloud                       -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.heytap.cloud 
if "%c%"=="2" echo The application is not affected!
goto start3

:hotapps
echo ----------------------------------------------------------
echo -                     Hot apps                           -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.opos.cs 
if "%c%"=="2" echo The application is not affected!
goto start3

:oroaming
echo ----------------------------------------------------------
echo -                     ORoaming                           -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.redteamobile.roaming 
if "%c%"=="2" echo The application is not affected!
goto start3

:clock
echo ----------------------------------------------------------
echo -                     Clock                              -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.coloros.alarmclock 
if "%c%"=="2" echo The application is not affected!
goto start3

:calculator
echo ----------------------------------------------------------
echo -                     Calculator                         -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.coloros.calculator 
if "%c%"=="2" echo The application is not affected!
goto start3

:recorder
echo ----------------------------------------------------------
echo -                     Recorder                           -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.coloros.soundrecorder 
if "%c%"=="2" echo The application is not affected!
goto start3


:ext
goto start


:4
:start4
echo --------------------------------------------------------------------------------------
echo -                                     GOOGLE  APPS                                   -
echo -                                   Applicaions List:                                -
echo -                    Choose the applications which you want to remove                -
echo --------------------------------------------------------------------------------------                           
echo a. Chrome
echo b. Gmail
echo c. Google Photos
echo d. Google calendar
echo e. Map
echo f. Keep notes
echo g. YouTube
echo h. Google Pay
echo i. Google Files
echo 0. Go to Main Menu

set /p d="Choose what you want Delete: "
if "%d%"=="a" goto chrome 
if "%d%"=="b" goto gmail
if "%d%"=="c" goto photos
if "%d%"=="d" goto calendar
if "%d%"=="e" goto map
if "%d%"=="f" goto notes
if "%d%"=="g" goto youtube
if "%d%"=="h" goto gpay
if "%d%"=="i" goto files
if "%d%"=="0" goto ext

:chrome
echo ----------------------------------------------------------
echo -                     Chrome                -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.android.chrome 
if "%c%"=="2" echo The application is not affected!
goto start4

:gmail
echo ----------------------------------------------------------
echo -                     Gmail                -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.google.android.gm 
if "%c%"=="2" echo The application is not affected!
goto start4

:photos
echo ----------------------------------------------------------
echo -                     Google Photos                      -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.google.android.apps.photos 
if "%c%"=="2" echo The application is not affected!
goto start4

:calendar
echo ----------------------------------------------------------
echo -                     Google calendar                    -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.google.android.calendar 
if "%c%"=="2" echo The application is not affected!
goto start4

:map
echo ----------------------------------------------------------
echo -                           Map                          -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.google.android.apps.maps 
if "%c%"=="2" echo The application is not affected!
goto start4

:notes
echo ----------------------------------------------------------
echo -                           Keep notes                   -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.google.android.keep 
if "%c%"=="2" echo The application is not affected!
goto start4

:youtube
echo ----------------------------------------------------------
echo -                           YouTube                      -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.google.android.youtube
if "%c%"=="2" echo The application is not affected!
goto start4

:gpay
echo ----------------------------------------------------------
echo -                          Google Pay                    -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.google.android.apps.nbu.paisa.user
if "%c%"=="2" echo The application is not affected!
goto start4

:files
echo ----------------------------------------------------------
echo -                          Google Files                    -
echo ----------------------------------------------------------                                        
echo 1.Delete
echo 2.Keep
set /p c="Are you sure you want to delete?: "
if "%c%"=="1" adb shell pm uninstall --user 0 com.google.android.apps.nbu.files
if "%c%"=="2" echo The application is not affected!
goto start4

:2
:start2
echo --------------------------------------------------------------------------------------
echo -                                Realme UI applications                      -
echo -                                   Applicaions List:                                 -
echo -                   Choose the applications which you want to disable                 -
echo --------------------------------------------------------------------------------------
echo a. App Market
echo b. Game Center
echo 0. Go to Main Menu

set /p e="Choose which application to disable?: "
if "%e%"=="a" goto appmarket
if "%e%"=="b" goto gamecenter
if "%e%"=="0" goto ext

:appmarket
echo ----------------------------------------------------------
echo -                          App Market                    -
echo ----------------------------------------------------------                                        
echo 1.Disable
echo 2.Keep
set /p c="Are you sure you want to disable?: "
if "%c%"=="1" adb shell pm disable-user --user 0 com.heytap.market
if "%c%"=="2" echo The application is not affected!
goto start2

:gamecenter
echo ----------------------------------------------------------
echo -                         Game Center                    -
echo ----------------------------------------------------------                                        
echo 1.Disable
echo 2.Keep
set /p c="Are you sure you want to disabe?: "
if "%c%"=="1" adb shell pm disable-user --user 0 com.nearme.gamecenter
if "%c%"=="2" echo The application is not affected!
goto start2

:ext
goto start

:error 
echo _______________________________________________________________________________
echo ENABLE USB DEBUGGING FROM DEVELOPER OPTIONS
echo _______________________________________________________________________________
pause 
goto start0