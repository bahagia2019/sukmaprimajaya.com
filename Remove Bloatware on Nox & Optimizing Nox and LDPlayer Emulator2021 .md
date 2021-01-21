# Debloating Nox by [kosmara.org](https://kosmara.org)

Nox, despite being the most feature-filled Android emulator, has a lot of negativity surrounding it due to their antics when it comes to making income off of their program. It is known for running repeated advertisments in the background, calling home and passing along system information (outside of your Android instance) as well as a vast amount of potentially sensitive data in an encrypted payload back to their multitude of servers. With the following preventitive measures, we can stop a majority of this happening as well as greatly improve the overall performance.


1. [Download and Install](https://www.bignox.com/en/download/fullPackage) a fresh copy of Nox. The latest version is fine (for now). If you already have it installed, that is fine too. No need to reinstall.

2. Enable Root Mode on Nox by clicking the gear icon and then checking the `Root Startup` box.

3. Install a new Launcher from the Play Store. ANYTHING but Nox's default. I suggest [Nova Launcher](https://play.google.com/store/apps/details?id=com.teslacoilsw.launcher&hl=en_US).

4. Once your launcher of choice is installed, click the Home icon and choose Nova Launcher and to Always Use This Launcher.

5. Go to your App Drawer and open File Manager and navigate to `system` -> `app`. In this folder, find `Launcher_X.X.X_*.apk` and `com.facebook.lite.apk` – delete them. If it says they are not found after tapping delete, just tap delete again.

6. Close Nox and navigate to `C:\Windows\System32\drivers\etc` and right click the `hosts` file and open it in Notepad (Run as Administrator if needed) or a plain text editor of your choice (e.g. [Notepad++](https://notepad-plus-plus.org/), [VS Code](https://code.visualstudio.com/), etc.) – once open, append the following list to the bottom of the file:

```json
127.0.0.1 8.bignox.com
127.0.0.1 alog.umeng.com
127.0.0.1 android.bignox.com
127.0.0.1 androiden.duapp.com
127.0.0.1 api-new.bignox.com
127.0.0.1 api.bignox.com
127.0.0.1 api.mobula.sdk.duapps.com
127.0.0.1 app.bignox.com
127.0.0.1 app.static.bignox.com
127.0.0.1 app.test.bignox.com
127.0.0.1 attitude.applinzi.com
127.0.0.1 au.umeng.com
127.0.0.1 bbs.bignox.com
127.0.0.1 bi.yeshen.com
127.0.0.1 bignox.com
127.0.0.1 cn.bignox.com
127.0.0.1 common.duapps.com
127.0.0.1 de.bignox.com
127.0.0.1 dev.bignox.com
127.0.0.1 download.bignox.com
127.0.0.1 en.bignox.com
127.0.0.1 es.bignox.com
127.0.0.1 feed.bignox.com
127.0.0.1 fr.bignox.com
127.0.0.1 game.bignox.com
127.0.0.1 gift.bignox.com
127.0.0.1 gray.bignox.com
127.0.0.1 group.bignox.com
127.0.0.1 hm.e.shifen.com
127.0.0.1 hmma.baidu.com
127.0.0.1 id.bignox.com
127.0.0.1 image.bignox.com
127.0.0.1 info.bignox.com
127.0.0.1 ios.bignox.com
127.0.0.1 kr.bignox.com
127.0.0.1 launcher-us.yeshen.com
127.0.0.1 launcher.us.yeshen.com
127.0.0.1 log.bignox.com
127.0.0.1 mail.bignox.com
127.0.0.1 mis.bignox.com
127.0.0.1 mobile.bignox.com
127.0.0.1 ms.bignox.com
127.0.0.1 my.bignox.com
127.0.0.1 news.bignox.com
127.0.0.1 noxagile.bceapp.com
127.0.0.1 noxagile.duapp.com
127.0.0.1 nrc.tapas.net
127.0.0.1 open.bignox.com
127.0.0.1 passport-us.bignox.com
127.0.0.1 passport.bignox.com
127.0.0.1 pasta.esfile.duapps.com
127.0.0.1 pay.bignox.com
127.0.0.1 ph.bignox.com
127.0.0.1 phone.bignox.com
127.0.0.1 plat-api.bignox.com
127.0.0.1 player.bignox.com
127.0.0.1 pop3.bignox.com
127.0.0.1 pt.bignox.com
127.0.0.1 pubstatus.sinaapp.com
127.0.0.1 res02.bignox.com
127.0.0.1 res05.bignox.com
127.0.0.1 res06.bignox.com
127.0.0.1 res09.bignox.com
127.0.0.1 res11.bignox.com
127.0.0.1 res12.bignox.com
127.0.0.1 res.bignox.com
127.0.0.1 res.noxmobi.com
127.0.0.1 ru.bignox.com
127.0.0.1 sdk.bignox.com
127.0.0.1 sdk.open.inc2.igexin.com
127.0.0.1 shouyou.bignox.com
127.0.0.1 sj.bignox.com
127.0.0.1 sns.bignox.com
127.0.0.1 st.bignox.com
127.0.0.1 survey.bignox.com
127.0.0.1 t.bignox.com
127.0.0.1 tdcv3.talkingdata.net
127.0.0.1 tl.bignox.com
127.0.0.1 tracking.apptrackerlink.com
127.0.0.1 tracking.trnox.com
127.0.0.1 tui.bignox.com
127.0.0.1 tv.bignox.com
127.0.0.1 tw.bignox.com
127.0.0.1 unauthorized.bignox.com
127.0.0.1 union.bignox.com
127.0.0.1 user.bignox.com
127.0.0.1 vip.bignox.com
127.0.0.1 wap.bignox.com
127.0.0.1 www.bignox.com
127.0.0.1 www.yeshen.com
127.0.0.1 www.yeshen.com.w.kunlungr.com
```

Once appended, save and close Notepad.

7. Navigate to `C:\Users\USERNAME\AppData\Local\Nox` and open `Conf.ini` in the same editor used for `hosts` above. Once open, change the following options to the values defined below:

```ini
pop_ads_refresh_time=9223372036854775807
service_qq=0
service_qq_link=<a target=\"_blank\" href=\"#\" style=\"display: none;\"></a>
collect_behavior_enable=false
collect_behavior_interveral=9223372036854775807
root=false
```

Afterwards, save and close the file. Right Click it, go to Properties, and check `Read Only` so Nox will not revert these changes.

Once this is all done, you are free to re-open Nox and continue playing as usual.

# Optimization

Ragnarok Mobile as well as a select few of other games have an in-game 2K resolution mode achievable by the iPad Pro and high-end 4K Android tablets. It can be enabled while using Nox by setting a proper resolution and DPI.

If you have already performed the steps above, you will need close Nox and temporarily uncheck `Read Only` on your `conf.ini`. Afterwards, open Nox and click the Cog on the top right and go to Advanced settings.

**Performance Settings**  
These are computer-specific, so go to Start Menu -> Right Click My PC -> Properties and see how many cores your CPU has and how much memory you have.

**Cores**  
Same amount as your processor has (e.g. i7-8700k has `6`)

**Memory**  
If your system has `16GB` or more of memory, `8096MB` is more than sufficient.  
If your system has `8GB` of memory, `4096MB` is sufficient.  
If your system has `4GB` or less of memory, I'm sorry– but you shouldn't attempt 2K.  

**Startup settings**  
Width: `2560`  
Height: `1440`  
DPI: `320`  

**Miscellaneous**  
Graphics rendering mode: `Speed (DirectX)`  
Frame settings: `60`  
Mouse acceleration: `Checked (Turn off mouse acceleration in Windows)`  

<p>Bloatware apps are one of the main problems of most android emulator today. Looking for an alternative emulator that has less bloatware is difficult to find, if you happen to find one &ndash; you suffer from low performance in terms of games because these emulators are built for applications only. Popular android emulators that are built for gaming like Nox Player and LDPlayer gives faster performance but due to its bloatware, it makes laggy for some PC owners specially to those who have low specs.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2100 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-emulator-bloatware.jpg?fit=1024%2C597&amp;ssl=1" sizes="(max-width: 1170px) 100vw, 1170px" srcset="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-emulator-bloatware.jpg?w=1598&amp;ssl=1 1598w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-emulator-bloatware.jpg?resize=300%2C175&amp;ssl=1 300w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-emulator-bloatware.jpg?resize=1024%2C597&amp;ssl=1 1024w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-emulator-bloatware.jpg?resize=768%2C447&amp;ssl=1 768w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-emulator-bloatware.jpg?resize=1536%2C895&amp;ssl=1 1536w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-emulator-bloatware.jpg?resize=370%2C216&amp;ssl=1 370w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-emulator-bloatware.jpg?resize=770%2C449&amp;ssl=1 770w" alt="" width="1598" height="931" data-pagespeed-url-hash="2217186936" data-lazy-loaded="1" /></figure>
<p>We tried to find ways to remove it and luckily, we found a way to do it and we&rsquo;ll share it here in this guide. This is by uninstalling those apps using Google&rsquo;s SDK Android Debug Bridge or adb.</p>
<p><strong>Table of Content</strong></p>
<ol>
<li><a href="/#enable-developer-options">Enable Developer Options</a></li>
<li><a href="/#enable-usb-debugging">Enable USB Debugging</a></li>
<li><a href="#install-basic-launcher">Install a Basic Launcher</a></li>
<li><a href="/#nox-player-emulator">Step for NOX Player Emulator</a></li>
<li><a href="/#ldplayer-emulator">Step for LD Player 3.0 Emulator</a></li>
<li><a href="https://codefaq.org/emulator/how-to-remove-bloatware-on-nox-and-ldplayer-emulator/#ldplayer4">Step for LD Player 4.0 Emulator</a></li>
<li><a href="/#final-touch">Final Touch</a></li>
<li><a href="/#troubleshoot">Troubleshoot</a></li>
<li><a href="/#appendix">Appendix</a></li>
</ol>
<p>The steps are easy and readily available in your emulator packages, so our step-by-step process is a no brainer for everyone.</p>
<h2 id="enable-developer-options">Enable Developer Options</h2>
<p>To start, we need to enable the Developer Options from your emulator. This will allow us to access the Android Debug Bridge (adb).</p>
<p>To do that, Go to<strong>&nbsp;Settings</strong>&nbsp;&gt;&nbsp;<strong>About Tablet</strong>. Then scroll down to the bottom of the page and look for the&nbsp;<strong>Build number</strong>. Tap it&nbsp;<strong>7 times</strong>&nbsp;to enable the Developer Options.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2079 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/build-number-android-emulator.jpg?fit=1024%2C542&amp;ssl=1" sizes="(max-width: 1170px) 100vw, 1170px" srcset="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/build-number-android-emulator.jpg?w=1596&amp;ssl=1 1596w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/build-number-android-emulator.jpg?resize=300%2C159&amp;ssl=1 300w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/build-number-android-emulator.jpg?resize=1024%2C542&amp;ssl=1 1024w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/build-number-android-emulator.jpg?resize=768%2C407&amp;ssl=1 768w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/build-number-android-emulator.jpg?resize=1536%2C813&amp;ssl=1 1536w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/build-number-android-emulator.jpg?resize=370%2C196&amp;ssl=1 370w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/build-number-android-emulator.jpg?resize=1170%2C618&amp;ssl=1 1170w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/build-number-android-emulator.jpg?resize=770%2C408&amp;ssl=1 770w" alt="" width="1596" height="845" data-pagespeed-url-hash="483652145" data-lazy-loaded="1" /></figure>
<p>Once activated, it will show an message saying&nbsp;<em>&ldquo;You are now a developer!&rdquo;</em>.</p>
<h2 id="enable-usb-debugging">Enable USB Debugging</h2>
<p>Our next step is to enable the USB debugging, you can do this by going to&nbsp;<strong>Settings&nbsp;</strong>&gt;&nbsp;<strong>Developer Options</strong>.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2077 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/developer-option-android.jpg?fit=1024%2C543&amp;ssl=1" sizes="(max-width: 1170px) 100vw, 1170px" srcset="https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/developer-option-android.jpg?w=1594&amp;ssl=1 1594w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/developer-option-android.jpg?resize=300%2C159&amp;ssl=1 300w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/developer-option-android.jpg?resize=1024%2C543&amp;ssl=1 1024w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/developer-option-android.jpg?resize=768%2C407&amp;ssl=1 768w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/developer-option-android.jpg?resize=1536%2C814&amp;ssl=1 1536w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/developer-option-android.jpg?resize=370%2C196&amp;ssl=1 370w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/developer-option-android.jpg?resize=770%2C408&amp;ssl=1 770w" alt="" width="1594" height="845" data-pagespeed-url-hash="3583207405" data-lazy-loaded="1" /></figure>
<p>Look for&nbsp;<strong>USB debugging</strong>&nbsp;option from the list and enable it.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2078 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/usb-debugging-android-emulator.jpg?fit=1024%2C542&amp;ssl=1" sizes="(max-width: 1170px) 100vw, 1170px" srcset="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/usb-debugging-android-emulator.jpg?w=1596&amp;ssl=1 1596w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/usb-debugging-android-emulator.jpg?resize=300%2C159&amp;ssl=1 300w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/usb-debugging-android-emulator.jpg?resize=1024%2C542&amp;ssl=1 1024w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/usb-debugging-android-emulator.jpg?resize=768%2C406&amp;ssl=1 768w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/usb-debugging-android-emulator.jpg?resize=1536%2C812&amp;ssl=1 1536w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/usb-debugging-android-emulator.jpg?resize=370%2C196&amp;ssl=1 370w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/usb-debugging-android-emulator.jpg?resize=1170%2C618&amp;ssl=1 1170w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/usb-debugging-android-emulator.jpg?resize=770%2C407&amp;ssl=1 770w" alt="" width="1596" height="844" data-pagespeed-url-hash="2596220742" data-lazy-loaded="1" /></figure>
<p>If you&rsquo;re using LDPlayer, you also need to change the option for&nbsp;<strong>Root access</strong>&nbsp;to&nbsp;<strong>Apps and ADB</strong>.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2082 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/root-access-android.jpg?fit=1024%2C552&amp;ssl=1" sizes="(max-width: 1170px) 100vw, 1170px" srcset="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/root-access-android.jpg?w=1737&amp;ssl=1 1737w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/root-access-android.jpg?resize=300%2C162&amp;ssl=1 300w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/root-access-android.jpg?resize=1024%2C552&amp;ssl=1 1024w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/root-access-android.jpg?resize=768%2C414&amp;ssl=1 768w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/root-access-android.jpg?resize=1536%2C829&amp;ssl=1 1536w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/root-access-android.jpg?resize=370%2C200&amp;ssl=1 370w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/root-access-android.jpg?resize=770%2C415&amp;ssl=1 770w" alt="" width="1737" height="937" data-pagespeed-url-hash="1840085181" data-lazy-loaded="1" /></figure>
<h2 id="install-basic-launcher">Install a Basic Launcher</h2>
<p>Most of the bloatware that comes from the emulator are from its stock launcher. Replacing it with a much faster but basic launcher will do the trick.</p>
<p>There are lot of good launcher available on the internet. One of them is Google Now Launcher, Lean Launcher or the Rootless Launcher.</p>
<p>What we recommend using is&nbsp;<strong>Rootless Launcher</strong>&nbsp;because it is open source, easy to setup and available in Google Play. If you know programming, you can also make your own version of launcher at&nbsp;<a href="https://github.com/amirzaidi/Launcher3">github.com/amirzaidi/Launcher3</a>.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2080 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/rootless-launcher.jpg?fit=1024%2C575&amp;ssl=1" sizes="(max-width: 1170px) 100vw, 1170px" srcset="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/rootless-launcher.jpg?w=1593&amp;ssl=1 1593w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/rootless-launcher.jpg?resize=300%2C169&amp;ssl=1 300w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/rootless-launcher.jpg?resize=1024%2C575&amp;ssl=1 1024w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/rootless-launcher.jpg?resize=768%2C431&amp;ssl=1 768w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/rootless-launcher.jpg?resize=1536%2C863&amp;ssl=1 1536w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/rootless-launcher.jpg?resize=370%2C208&amp;ssl=1 370w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/rootless-launcher.jpg?resize=770%2C433&amp;ssl=1 770w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/rootless-launcher.jpg?resize=270%2C152&amp;ssl=1 270w" alt="" width="1593" height="895" data-pagespeed-url-hash="2268344505" data-lazy-loaded="1" /></figure>
<p>Download and install Rootless Launcher on Google Play.</p>
<ul>
<li><a href="https://play.google.com/store/apps/details?id=amirz.rootless.nexuslauncher" target="_blank" rel="noreferrer noopener">https://play.google.com/store/apps/details?id=amirz.rootless.nexuslauncher</a></li>
</ul>
<p>Once installed, you need to choose the default launcher of your emulator to Rootless Launcher. You can do that by going to&nbsp;<strong>Settings</strong>&nbsp;&gt;&nbsp;<strong>Home</strong>.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2093 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/settings-device-home-android.jpg?fit=1024%2C542&amp;ssl=1" sizes="(max-width: 1170px) 100vw, 1170px" srcset="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/settings-device-home-android.jpg?w=1598&amp;ssl=1 1598w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/settings-device-home-android.jpg?resize=300%2C159&amp;ssl=1 300w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/settings-device-home-android.jpg?resize=1024%2C542&amp;ssl=1 1024w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/settings-device-home-android.jpg?resize=768%2C407&amp;ssl=1 768w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/settings-device-home-android.jpg?resize=1536%2C813&amp;ssl=1 1536w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/settings-device-home-android.jpg?resize=370%2C196&amp;ssl=1 370w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/settings-device-home-android.jpg?resize=1170%2C618&amp;ssl=1 1170w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/settings-device-home-android.jpg?resize=770%2C408&amp;ssl=1 770w" alt="" width="1598" height="846" data-pagespeed-url-hash="137295631" data-lazy-loaded="1" /></figure>
<p>Select&nbsp;<strong>Rootless Launcher</strong>&nbsp;as the default. Don&rsquo;t mind the old launcher, that will be removed on the other step.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2094 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/rootless-pixel-launcher-android-primary.jpg?fit=1024%2C543&amp;ssl=1" sizes="(max-width: 1170px) 100vw, 1170px" srcset="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/rootless-pixel-launcher-android-primary.jpg?w=1595&amp;ssl=1 1595w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/rootless-pixel-launcher-android-primary.jpg?resize=300%2C159&amp;ssl=1 300w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/rootless-pixel-launcher-android-primary.jpg?resize=1024%2C543&amp;ssl=1 1024w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/rootless-pixel-launcher-android-primary.jpg?resize=768%2C407&amp;ssl=1 768w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/rootless-pixel-launcher-android-primary.jpg?resize=1536%2C815&amp;ssl=1 1536w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/rootless-pixel-launcher-android-primary.jpg?resize=370%2C196&amp;ssl=1 370w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/rootless-pixel-launcher-android-primary.jpg?resize=770%2C408&amp;ssl=1 770w" alt="" width="1595" height="846" data-pagespeed-url-hash="2603417494" data-lazy-loaded="1" /></figure>
<p>To set Home for&nbsp;<strong>LDPlayer 4.0</strong>, just click the&nbsp;<strong>Home</strong>&nbsp;tabs on the emulator and it will prompt you to set the default Home launcher.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2205 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-22.png?fit=1024%2C583&amp;ssl=1" sizes="(max-width: 1170px) 100vw, 1170px" srcset="https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-22.png?w=1640&amp;ssl=1 1640w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-22.png?resize=300%2C171&amp;ssl=1 300w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-22.png?resize=1024%2C583&amp;ssl=1 1024w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-22.png?resize=768%2C437&amp;ssl=1 768w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-22.png?resize=1536%2C875&amp;ssl=1 1536w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-22.png?resize=370%2C211&amp;ssl=1 370w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-22.png?resize=770%2C439&amp;ssl=1 770w" alt="" width="1640" height="934" data-pagespeed-url-hash="567116933" data-lazy-loaded="1" /></figure>
<p>Since we are done now with the settings and the launcher, we can now proceed to access the ADB from our emulator. We separate the guide for each emulator, please pick the one you&rsquo;re using:</p>
<ul>
<li><a href="/#nox-player-emulator">Nox Player</a></li>
<li><a href="/#ldplayer-emulator">LD Player 3.0</a></li>
<li><a href="/#ldplayer4">LD Player 4.0</a></li>
</ul>
<h2 id="nox-player-emulator">Step for Nox Player Emulator</h2>
<p>Look for the installation directory of your Nox Player, you can find it by right clicking the&nbsp;<strong>Nox</strong>&nbsp;shortcut icon then&nbsp;<strong>Open file location</strong>.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2161 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-6.png?resize=834%2C479&amp;ssl=1" sizes="(max-width: 834px) 100vw, 834px" srcset="https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-6.png?w=834&amp;ssl=1 834w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-6.png?resize=300%2C172&amp;ssl=1 300w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-6.png?resize=768%2C441&amp;ssl=1 768w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-6.png?resize=370%2C213&amp;ssl=1 370w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-6.png?resize=770%2C442&amp;ssl=1 770w" alt="" width="834" height="479" data-recalc-dims="1" data-pagespeed-url-hash="319498556" data-lazy-loaded="1" /></figure>
<p>In our case its&nbsp;<code>D:\program files\Nox\bin</code>, we will use this to access the directory from the command prompt, so make sure to remember or copy it.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2085 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-player-file-directory.jpg?fit=1024%2C544&amp;ssl=1" sizes="(max-width: 1170px) 100vw, 1170px" srcset="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-player-file-directory.jpg?w=1208&amp;ssl=1 1208w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-player-file-directory.jpg?resize=300%2C159&amp;ssl=1 300w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-player-file-directory.jpg?resize=1024%2C544&amp;ssl=1 1024w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-player-file-directory.jpg?resize=768%2C408&amp;ssl=1 768w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-player-file-directory.jpg?resize=370%2C197&amp;ssl=1 370w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-player-file-directory.jpg?resize=770%2C409&amp;ssl=1 770w" alt="" width="1208" height="642" data-pagespeed-url-hash="1023850199" data-lazy-loaded="1" /></figure>
<p>Run a command prompt by going to cortana, and search&nbsp;<code>cmd</code>. Then choose Command Prompt or hit enter.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2086 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/cortana-cmd.jpg?resize=873%2C694&amp;ssl=1" sizes="(max-width: 873px) 100vw, 873px" srcset="https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/cortana-cmd.jpg?w=873&amp;ssl=1 873w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/cortana-cmd.jpg?resize=300%2C238&amp;ssl=1 300w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/cortana-cmd.jpg?resize=768%2C611&amp;ssl=1 768w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/cortana-cmd.jpg?resize=370%2C294&amp;ssl=1 370w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/cortana-cmd.jpg?resize=770%2C612&amp;ssl=1 770w" alt="" width="873" height="694" data-recalc-dims="1" data-pagespeed-url-hash="1967623079" data-lazy-loaded="1" /></figure>
<p>Then type the following, don&rsquo;t forget to change the directory with your own installation directory. Paste here if you copy the full path of installation directory earlier. In our case its&nbsp;<strong>D:\program files\Nox\bin</strong>.</p>
<pre class="wp-block-code"><code>cd /d D:\program files\Nox\bin</code></pre>
<p>Once inside, we can now call the built-in adb from our emulator.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2087 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/cmd-nox-player-directory.jpg?resize=978%2C509&amp;ssl=1" sizes="(max-width: 978px) 100vw, 978px" srcset="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/cmd-nox-player-directory.jpg?w=978&amp;ssl=1 978w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/cmd-nox-player-directory.jpg?resize=300%2C156&amp;ssl=1 300w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/cmd-nox-player-directory.jpg?resize=768%2C400&amp;ssl=1 768w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/cmd-nox-player-directory.jpg?resize=370%2C193&amp;ssl=1 370w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/cmd-nox-player-directory.jpg?resize=770%2C401&amp;ssl=1 770w" alt="" width="978" height="509" data-recalc-dims="1" data-pagespeed-url-hash="3261613428" data-lazy-loaded="1" /></figure>
<p>Let&rsquo;s call the devices command to list all of the available emulators that are connected to our PC. It will also enable us to connect automatically to the emulator.</p>
<pre class="wp-block-code"><code>adb devices</code></pre>
<figure class="wp-block-image size-large"><img class="wp-image-2088 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/adb-devices-command.jpg?resize=977%2C511&amp;ssl=1" sizes="(max-width: 977px) 100vw, 977px" srcset="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/adb-devices-command.jpg?w=977&amp;ssl=1 977w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/adb-devices-command.jpg?resize=300%2C157&amp;ssl=1 300w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/adb-devices-command.jpg?resize=768%2C402&amp;ssl=1 768w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/adb-devices-command.jpg?resize=370%2C194&amp;ssl=1 370w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/adb-devices-command.jpg?resize=770%2C403&amp;ssl=1 770w" alt="" width="977" height="511" data-recalc-dims="1" data-pagespeed-url-hash="3581414907" data-lazy-loaded="1" /></figure>
<p>Then, we need to remount our emulator partition drive so that it will become writable. This will allow us to make modifications to the emulator&rsquo;s file system.</p>
<pre class="wp-block-code"><code>adb remount</code></pre>
<figure class="wp-block-image size-large"><img class="wp-image-2089 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/adb-remount.jpg?resize=976%2C507&amp;ssl=1" sizes="(max-width: 976px) 100vw, 976px" srcset="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/adb-remount.jpg?w=976&amp;ssl=1 976w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/adb-remount.jpg?resize=300%2C156&amp;ssl=1 300w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/adb-remount.jpg?resize=768%2C399&amp;ssl=1 768w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/adb-remount.jpg?resize=370%2C192&amp;ssl=1 370w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/adb-remount.jpg?resize=770%2C400&amp;ssl=1 770w" alt="" width="976" height="507" data-recalc-dims="1" data-pagespeed-url-hash="3602071374" data-lazy-loaded="1" /></figure>
<p>After that, we can now enter to the shell command of our emulator.</p>
<pre class="wp-block-code"><code>adb shell</code></pre>
<figure class="wp-block-image size-large"><img class="wp-image-2090 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/adb-shell.jpg?resize=977%2C510&amp;ssl=1" sizes="(max-width: 977px) 100vw, 977px" srcset="https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/adb-shell.jpg?w=977&amp;ssl=1 977w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/adb-shell.jpg?resize=300%2C157&amp;ssl=1 300w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/adb-shell.jpg?resize=768%2C401&amp;ssl=1 768w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/adb-shell.jpg?resize=370%2C193&amp;ssl=1 370w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/adb-shell.jpg?resize=770%2C402&amp;ssl=1 770w" alt="" width="977" height="510" data-recalc-dims="1" data-pagespeed-url-hash="2142296572" data-lazy-loaded="1" /></figure>
<p>If you get an error message saying&nbsp;<em>&ldquo;error: more than one device/emulator&rdquo;</em>, please check&nbsp;<a href="https://codefaq.org/emulator/how-to-remove-bloatware-on-nox-and-ldplayer-emulator/#troubleshoot">troubleshoot</a>.</p>
<p>Once you&rsquo;re inside the emulator&rsquo;s shell, we can now remove the apps that are unnecessary such as Facebook Lite, Sound Recorder, Live Wallpaper, default Launcher and many more. Just enter the command below one by one.</p>
<pre class="wp-block-code"><code>cd system/app
ls -la
rm -r LiveWallpapersPicker
rm -r FacebookLite
rm -r SoundRecorder
rm -r PhaseBeam
rm -r Launcher
rm -r PackageInstaller
rm -r gpLogin
rm -r AppStore
rm -r Helper
rm -r BasicDreams
pm list packages
pm uninstall --user 0 com.facebook.lite
pm uninstall --user 0 com.android.packageinstaller
pm uninstall --user 0 com.android.soundrecorder
pm uninstall --user 0 com.android.wallpaper.livepicker
exit</code></pre>
<figure class="wp-block-image size-large"><img class="wp-image-2096 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/remove-bloatware-nox.jpg?resize=977%2C506&amp;ssl=1" sizes="(max-width: 977px) 100vw, 977px" srcset="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/remove-bloatware-nox.jpg?w=977&amp;ssl=1 977w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/remove-bloatware-nox.jpg?resize=300%2C155&amp;ssl=1 300w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/remove-bloatware-nox.jpg?resize=768%2C398&amp;ssl=1 768w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/remove-bloatware-nox.jpg?resize=370%2C192&amp;ssl=1 370w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/remove-bloatware-nox.jpg?resize=770%2C399&amp;ssl=1 770w" alt="" width="977" height="506" data-recalc-dims="1" data-pagespeed-url-hash="4039726378" data-lazy-loaded="1" /></figure>
<p>You&rsquo;re then now exited from the emulator shell command. Lastly, we can now reboot our emulator. Type the following command to reboot.</p>
<pre class="wp-block-code"><code>adb reboot</code></pre>
<p>Once done, your Nox emulator is now free from bloatware. The only thing you need to do now is to arrange the icons for your new launcher and play. Enjoy!</p>
<figure class="wp-block-image size-large"><img class="wp-image-2098 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-player-free-from-bloatware.jpg?fit=1024%2C596&amp;ssl=1" sizes="(max-width: 1170px) 100vw, 1170px" srcset="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-player-free-from-bloatware.jpg?w=1602&amp;ssl=1 1602w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-player-free-from-bloatware.jpg?resize=300%2C175&amp;ssl=1 300w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-player-free-from-bloatware.jpg?resize=1024%2C596&amp;ssl=1 1024w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-player-free-from-bloatware.jpg?resize=768%2C447&amp;ssl=1 768w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-player-free-from-bloatware.jpg?resize=1536%2C894&amp;ssl=1 1536w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-player-free-from-bloatware.jpg?resize=370%2C215&amp;ssl=1 370w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/nox-player-free-from-bloatware.jpg?resize=770%2C448&amp;ssl=1 770w" alt="" width="1602" height="932" data-pagespeed-url-hash="493496641" data-lazy-loaded="1" /></figure>
<p>If you&rsquo;re using the Nox&rsquo;s MulDrive, you need to copy the instance and repeat this&nbsp;<a href="https://codefaq.org/emulator/how-to-remove-bloatware-on-nox-and-ldplayer-emulator/#nox-player-emulator">step</a>.</p>
<p>You can also watch the step by step here:</p>
<figure class="wp-block-embed-youtube wp-block-embed is-type-video is-provider-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio">
<div class="wp-block-embed__wrapper"><span class="embed-youtube"><iframe class="youtube-player trx_addons_resize" src="https://www.youtube.com/embed/ZNGvFVdX6b8?version=3&amp;rel=1&amp;showsearch=0&amp;showinfo=1&amp;iv_load_policy=1&amp;fs=1&amp;hl=en-US&amp;autohide=2&amp;wmode=transparent" width="1170" height="659" sandbox="allow-scripts allow-same-origin allow-popups allow-presentation" allowfullscreen="allowfullscreen" data-last-width="770" data-mce-fragment="1"></iframe></span></div>
</figure>
<h2 id="ldplayer-emulator">Step for LDPlayer 3.0 Emulator</h2>
<p>The step are similar with NOX emulator, look for the installation directory of the LDPlayer by going to its shortcut icon from your desktop and right click then&nbsp;<strong>Open file location</strong>.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2158 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-5.png?resize=820%2C459&amp;ssl=1" sizes="(max-width: 820px) 100vw, 820px" srcset="https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-5.png?w=820&amp;ssl=1 820w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-5.png?resize=300%2C168&amp;ssl=1 300w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-5.png?resize=768%2C430&amp;ssl=1 768w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-5.png?resize=370%2C207&amp;ssl=1 370w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-5.png?resize=770%2C431&amp;ssl=1 770w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-5.png?resize=270%2C152&amp;ssl=1 270w" alt="" width="820" height="459" data-recalc-dims="1" data-pagespeed-url-hash="3686512084" data-lazy-loaded="1" /></figure>
<p>This will open the directory, copy the full path of the installation folder.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2121 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/ldplayer-installation-directory.jpg?fit=1024%2C524&amp;ssl=1" sizes="(max-width: 1078px) 100vw, 1078px" srcset="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/ldplayer-installation-directory.jpg?w=1078&amp;ssl=1 1078w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/ldplayer-installation-directory.jpg?resize=300%2C154&amp;ssl=1 300w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/ldplayer-installation-directory.jpg?resize=1024%2C524&amp;ssl=1 1024w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/ldplayer-installation-directory.jpg?resize=768%2C393&amp;ssl=1 768w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/ldplayer-installation-directory.jpg?resize=370%2C189&amp;ssl=1 370w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/ldplayer-installation-directory.jpg?resize=770%2C394&amp;ssl=1 770w" alt="" width="1078" height="552" data-pagespeed-url-hash="4155842739" data-lazy-loaded="1" /></figure>
<p>Once done, open up a CMD. Go to Cortana and search for&nbsp;<strong>CMD</strong>. Select&nbsp;<strong>Command Prompt</strong>&nbsp;from the result or hit Enter.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2086 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/cortana-cmd.jpg?resize=873%2C694&amp;ssl=1" sizes="(max-width: 873px) 100vw, 873px" srcset="https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/cortana-cmd.jpg?w=873&amp;ssl=1 873w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/cortana-cmd.jpg?resize=300%2C238&amp;ssl=1 300w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/cortana-cmd.jpg?resize=768%2C611&amp;ssl=1 768w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/cortana-cmd.jpg?resize=370%2C294&amp;ssl=1 370w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/cortana-cmd.jpg?resize=770%2C612&amp;ssl=1 770w" alt="" width="873" height="694" data-recalc-dims="1" data-pagespeed-url-hash="1967623079" data-lazy-loaded="1" /></figure>
<p>At the command prompt. We need to enter the installation directory, to do that type cd \d followed by the installation directory. Paste the path here.</p>
<pre class="wp-block-code"><code>cd \d E:\LDPlayer</code></pre>
<p>Once inside, we can now access the built-in Android Debug Bridge (ADB). To check what is android OS connected to the PC, call this command.</p>
<pre class="wp-block-code"><code>adb devices</code></pre>
<figure class="wp-block-image size-large"><img class="wp-image-2124 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/ld-player-adb-devices.jpg?resize=977%2C508&amp;ssl=1" sizes="(max-width: 977px) 100vw, 977px" srcset="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/ld-player-adb-devices.jpg?w=977&amp;ssl=1 977w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/ld-player-adb-devices.jpg?resize=300%2C156&amp;ssl=1 300w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/ld-player-adb-devices.jpg?resize=768%2C399&amp;ssl=1 768w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/ld-player-adb-devices.jpg?resize=370%2C192&amp;ssl=1 370w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/ld-player-adb-devices.jpg?resize=770%2C400&amp;ssl=1 770w" alt="" width="977" height="508" data-recalc-dims="1" data-pagespeed-url-hash="411239456" data-lazy-loaded="1" /></figure>
<p>Next is, we need to remount the partition drive of our emulator. To do that, just call:</p>
<pre class="wp-block-code"><code>adb remount</code></pre>
<figure class="wp-block-image size-large"><img class="wp-image-2125 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-1.png?resize=976%2C511&amp;ssl=1" sizes="(max-width: 976px) 100vw, 976px" srcset="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-1.png?w=976&amp;ssl=1 976w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-1.png?resize=300%2C157&amp;ssl=1 300w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-1.png?resize=768%2C402&amp;ssl=1 768w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-1.png?resize=370%2C194&amp;ssl=1 370w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-1.png?resize=770%2C403&amp;ssl=1 770w" alt="" width="976" height="511" data-recalc-dims="1" data-pagespeed-url-hash="3438469648" data-lazy-loaded="1" /></figure>
<p>Now, we can proceed on entering the emulator&rsquo;s shell.</p>
<pre class="wp-block-code"><code>adb shell</code></pre>
<figure class="wp-block-image size-large"><img class="wp-image-2126 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-2.png?resize=975%2C507&amp;ssl=1" sizes="(max-width: 975px) 100vw, 975px" srcset="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-2.png?w=975&amp;ssl=1 975w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-2.png?resize=300%2C156&amp;ssl=1 300w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-2.png?resize=768%2C399&amp;ssl=1 768w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-2.png?resize=370%2C192&amp;ssl=1 370w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-2.png?resize=770%2C400&amp;ssl=1 770w" alt="" width="975" height="507" data-recalc-dims="1" data-pagespeed-url-hash="3036503787" data-lazy-loaded="1" /></figure>
<p>If you get an error message&nbsp;<em>&ldquo;error: more than one device/emulator&rdquo;</em>, please check&nbsp;<a href="https://codefaq.org/wp-admin/post.php?post=2074&amp;action=edit#troubleshoot">troubleshoot</a>.</p>
<p>From here, we can now delete the unnecessary app installed in the LDPlayer emulator like LDAppStore, Launcher and the PackageInstaller.&nbsp;<em>(However, LD Appstore is quite useful for installing APK&rsquo;s that are not downloadable from Google Play &ndash; you can re-install it later by going to LDPlayer official website, the step here is important to make sure it will not load on the boot and to make it as non-system app.)</em></p>
<pre class="wp-block-code"><code>cd system/app
ls -la
rm -r LDAppStore
rm -r Launcher3
rm -r PackageInstaller
exit</code></pre>
<figure class="wp-block-image size-large"><img class="wp-image-2123 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/ldplayer-delete-unecessary-program.jpg?resize=908%2C474&amp;ssl=1" sizes="(max-width: 908px) 100vw, 908px" srcset="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/ldplayer-delete-unecessary-program.jpg?w=908&amp;ssl=1 908w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/ldplayer-delete-unecessary-program.jpg?resize=300%2C157&amp;ssl=1 300w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/ldplayer-delete-unecessary-program.jpg?resize=768%2C401&amp;ssl=1 768w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/ldplayer-delete-unecessary-program.jpg?resize=370%2C193&amp;ssl=1 370w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/ldplayer-delete-unecessary-program.jpg?resize=770%2C402&amp;ssl=1 770w" alt="" width="908" height="474" data-recalc-dims="1" data-pagespeed-url-hash="1255225977" data-lazy-loaded="1" /></figure>
<p>Everything is now removed, we can now reboot our emulator.</p>
<pre class="wp-block-code"><code>adb reboot</code></pre>
<p>For LDPlayer, after rebooting from ADB, the emulator screen will just show a black screen. To fix that, just close the emulator and click&nbsp;<strong>Restart</strong>.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2127 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-3.png?fit=1024%2C585&amp;ssl=1" sizes="(max-width: 1170px) 100vw, 1170px" srcset="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-3.png?w=1778&amp;ssl=1 1778w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-3.png?resize=300%2C171&amp;ssl=1 300w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-3.png?resize=1024%2C585&amp;ssl=1 1024w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-3.png?resize=768%2C439&amp;ssl=1 768w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-3.png?resize=1536%2C878&amp;ssl=1 1536w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-3.png?resize=370%2C211&amp;ssl=1 370w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-3.png?resize=770%2C440&amp;ssl=1 770w" alt="" width="1778" height="1016" data-pagespeed-url-hash="3528710013" data-lazy-loaded="1" /></figure>
<p>It will show the home screen and you&rsquo;re done with removing all of the bloatware in your LDPlayer emulator. You can now arrange the icon and install your favorite games. Enjoy!</p>
<figure class="wp-block-image size-large"><img class="wp-image-2128 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-4.png?fit=1024%2C585&amp;ssl=1" sizes="(max-width: 1170px) 100vw, 1170px" srcset="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-4.png?w=1779&amp;ssl=1 1779w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-4.png?resize=300%2C171&amp;ssl=1 300w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-4.png?resize=1024%2C585&amp;ssl=1 1024w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-4.png?resize=768%2C439&amp;ssl=1 768w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-4.png?resize=1536%2C877&amp;ssl=1 1536w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-4.png?resize=370%2C211&amp;ssl=1 370w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-4.png?resize=770%2C440&amp;ssl=1 770w" alt="" width="1779" height="1016" data-pagespeed-url-hash="108050550" data-lazy-loaded="1" /></figure>
<p>If you missed some parts of the step, you can also check the video guide below.</p>
<figure class="wp-block-embed-youtube wp-block-embed is-type-video is-provider-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio">
<div class="wp-block-embed__wrapper"><span class="embed-youtube"><iframe class="youtube-player trx_addons_resize" src="https://www.youtube.com/embed/LKlQwiqo44M?version=3&amp;rel=1&amp;showsearch=0&amp;showinfo=1&amp;iv_load_policy=1&amp;fs=1&amp;hl=en-US&amp;autohide=2&amp;wmode=transparent" width="1170" height="659" sandbox="allow-scripts allow-same-origin allow-popups allow-presentation" allowfullscreen="allowfullscreen" data-last-width="770" data-mce-fragment="1"></iframe></span></div>
</figure>
<h2 id="ldplayer4">Step for LD Player 4.0 Emulator</h2>
<p>First, we have to find the installation path of our LD Player 4 emulator. You can get it by right clicking the desktop shortcut icon and click&nbsp;<strong>Open File Location</strong>.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2193 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-11.png?fit=1024%2C590&amp;ssl=1" sizes="(max-width: 1037px) 100vw, 1037px" srcset="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-11.png?w=1037&amp;ssl=1 1037w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-11.png?resize=300%2C173&amp;ssl=1 300w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-11.png?resize=1024%2C590&amp;ssl=1 1024w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-11.png?resize=768%2C442&amp;ssl=1 768w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-11.png?resize=370%2C213&amp;ssl=1 370w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-11.png?resize=770%2C443&amp;ssl=1 770w" alt="" width="1037" height="597" data-pagespeed-url-hash="991344312" data-lazy-loaded="1" /></figure>
<p>Then it will open the directory in a new window. Copy the installation path.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2194 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-12.png?resize=848%2C466&amp;ssl=1" sizes="(max-width: 848px) 100vw, 848px" srcset="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-12.png?w=848&amp;ssl=1 848w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-12.png?resize=300%2C165&amp;ssl=1 300w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-12.png?resize=768%2C422&amp;ssl=1 768w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-12.png?resize=370%2C203&amp;ssl=1 370w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-12.png?resize=770%2C423&amp;ssl=1 770w" alt="" width="848" height="466" data-recalc-dims="1" data-pagespeed-url-hash="1886858457" data-lazy-loaded="1" /></figure>
<p>Open up a command prompt by going to Cortana and search for &ldquo;CMD&rdquo;.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2195 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-13.png?resize=831%2C597&amp;ssl=1" sizes="(max-width: 831px) 100vw, 831px" srcset="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-13.png?w=831&amp;ssl=1 831w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-13.png?resize=300%2C216&amp;ssl=1 300w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-13.png?resize=768%2C552&amp;ssl=1 768w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-13.png?resize=370%2C266&amp;ssl=1 370w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-13.png?resize=770%2C553&amp;ssl=1 770w" alt="" width="831" height="597" data-recalc-dims="1" data-pagespeed-url-hash="2745816663" data-lazy-loaded="1" /></figure>
<p>Then type the following command. Change the&nbsp;<strong>I:\XuanZhi\LDPlayer</strong>&nbsp;with your own installation directory.</p>
<pre class="wp-block-code"><code>cd /d I:\XuanZhi\LDPlayer</code></pre>
<figure class="wp-block-image size-large"><img class="wp-image-2196 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-14.png?resize=978%2C506&amp;ssl=1" sizes="(max-width: 978px) 100vw, 978px" srcset="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-14.png?w=978&amp;ssl=1 978w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-14.png?resize=300%2C155&amp;ssl=1 300w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-14.png?resize=768%2C397&amp;ssl=1 768w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-14.png?resize=370%2C191&amp;ssl=1 370w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-14.png?resize=770%2C398&amp;ssl=1 770w" alt="" width="978" height="506" data-recalc-dims="1" data-pagespeed-url-hash="2952059936" data-lazy-loaded="1" /></figure>
<p>Then to show all of the available devices connected in your pc. Type the following.</p>
<pre class="wp-block-code"><code>adb devices</code></pre>
<figure class="wp-block-image size-large"><img class="wp-image-2197 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-15.png?resize=978%2C509&amp;ssl=1" sizes="(max-width: 978px) 100vw, 978px" srcset="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-15.png?w=978&amp;ssl=1 978w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-15.png?resize=300%2C156&amp;ssl=1 300w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-15.png?resize=768%2C400&amp;ssl=1 768w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-15.png?resize=370%2C193&amp;ssl=1 370w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-15.png?resize=770%2C401&amp;ssl=1 770w" alt="" width="978" height="509" data-recalc-dims="1" data-pagespeed-url-hash="2784369528" data-lazy-loaded="1" /></figure>
<p>Then we need to remount our emulator to be able to modify the system file.</p>
<pre class="wp-block-code"><code>adb remount</code></pre>
<figure class="wp-block-image size-large"><img class="wp-image-2198 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-16.png?resize=975%2C507&amp;ssl=1" sizes="(max-width: 975px) 100vw, 975px" srcset="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-16.png?w=975&amp;ssl=1 975w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-16.png?resize=300%2C156&amp;ssl=1 300w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-16.png?resize=768%2C399&amp;ssl=1 768w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-16.png?resize=370%2C192&amp;ssl=1 370w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-16.png?resize=770%2C400&amp;ssl=1 770w" alt="" width="975" height="507" data-recalc-dims="1" data-pagespeed-url-hash="105189532" data-lazy-loaded="1" /></figure>
<p>Then open the shell terminal of our emulator.</p>
<pre class="wp-block-code"><code>adb shell</code></pre>
<figure class="wp-block-image size-large"><img class="wp-image-2199 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-17.png?resize=978%2C507&amp;ssl=1" sizes="(max-width: 978px) 100vw, 978px" srcset="https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-17.png?w=978&amp;ssl=1 978w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-17.png?resize=300%2C156&amp;ssl=1 300w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-17.png?resize=768%2C398&amp;ssl=1 768w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-17.png?resize=370%2C192&amp;ssl=1 370w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-17.png?resize=770%2C399&amp;ssl=1 770w" alt="" width="978" height="507" data-recalc-dims="1" data-pagespeed-url-hash="3439985907" data-lazy-loaded="1" /></figure>
<p>After entering the command, it will show some gibberish text, just press&nbsp;<strong>Enter</strong>&nbsp;on your keyboard twice.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2200 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-18.png?resize=977%2C506&amp;ssl=1" sizes="(max-width: 977px) 100vw, 977px" srcset="https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-18.png?w=977&amp;ssl=1 977w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-18.png?resize=300%2C155&amp;ssl=1 300w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-18.png?resize=768%2C398&amp;ssl=1 768w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-18.png?resize=370%2C192&amp;ssl=1 370w, https://i1.wp.com/codefaq.org/wp-content/uploads/2020/05/image-18.png?resize=770%2C399&amp;ssl=1 770w" alt="" width="977" height="506" data-recalc-dims="1" data-pagespeed-url-hash="158889060" data-lazy-loaded="1" /></figure>
<p>Now, we can remove the stock launcher and LDAppStore.&nbsp;<em>For players that wants to use LD Appstore for installing app that cannot be downloaded from Google Play, you can reinstall later by going to LD Player official website. The step here will make sure that the app will not load on the boot and make it as non-system app.</em></p>
<pre class="wp-block-code"><code>cd /system/app
rm -r /system/app/Launcher3
rm -r /system/app/LDAppStore
pm list packages
pm uninstall --user 0 com.ldmnq.launcher3
exit</code></pre>
<figure class="wp-block-image size-large"><img class="wp-image-2201 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-19.png?resize=976%2C508&amp;ssl=1" sizes="(max-width: 976px) 100vw, 976px" srcset="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-19.png?w=976&amp;ssl=1 976w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-19.png?resize=300%2C156&amp;ssl=1 300w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-19.png?resize=768%2C400&amp;ssl=1 768w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-19.png?resize=370%2C193&amp;ssl=1 370w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-19.png?resize=770%2C401&amp;ssl=1 770w" alt="" width="976" height="508" data-recalc-dims="1" data-pagespeed-url-hash="923838633" data-lazy-loaded="1" /></figure>
<p>This will show an error on the emulator that saying .com.android.ld.appstore.app.MyApplication has stopped. Now, we can reboot our emulator.</p>
<pre class="wp-block-code"><code>adb reboot</code></pre>
<p>The emulator will show a Black Screen, wait for 5 to 10 seconds and just Restart the emulator to fix it.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2203 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-20.png?fit=1024%2C596&amp;ssl=1" sizes="(max-width: 1170px) 100vw, 1170px" srcset="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-20.png?w=1598&amp;ssl=1 1598w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-20.png?resize=300%2C175&amp;ssl=1 300w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-20.png?resize=1024%2C596&amp;ssl=1 1024w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-20.png?resize=768%2C447&amp;ssl=1 768w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-20.png?resize=1536%2C894&amp;ssl=1 1536w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-20.png?resize=370%2C215&amp;ssl=1 370w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-20.png?resize=770%2C448&amp;ssl=1 770w" alt="" width="1598" height="930" data-pagespeed-url-hash="1933006358" data-lazy-loaded="1" /></figure>
<p>After that, your emulator is now free from bloatware.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2204 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-21.png?fit=1024%2C597&amp;ssl=1" sizes="(max-width: 1170px) 100vw, 1170px" srcset="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-21.png?w=1601&amp;ssl=1 1601w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-21.png?resize=300%2C175&amp;ssl=1 300w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-21.png?resize=1024%2C597&amp;ssl=1 1024w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-21.png?resize=768%2C448&amp;ssl=1 768w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-21.png?resize=1536%2C895&amp;ssl=1 1536w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-21.png?resize=370%2C216&amp;ssl=1 370w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image-21.png?resize=770%2C449&amp;ssl=1 770w" alt="" width="1601" height="933" data-pagespeed-url-hash="2744058000" data-lazy-loaded="1" /></figure>
<p>You can also watch our step-by-step video guide below.</p>
<figure class="wp-block-embed-youtube wp-block-embed is-type-video is-provider-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio">
<div class="wp-block-embed__wrapper"><span class="embed-youtube"><iframe class="youtube-player trx_addons_resize" src="https://www.youtube.com/embed/t3_vmbyv3r0?version=3&amp;rel=1&amp;showsearch=0&amp;showinfo=1&amp;iv_load_policy=1&amp;fs=1&amp;hl=en-US&amp;autohide=2&amp;wmode=transparent" width="1170" height="659" sandbox="allow-scripts allow-same-origin allow-popups allow-presentation" allowfullscreen="allowfullscreen" data-last-width="770" data-mce-fragment="1"></iframe></span></div>
</figure>
<h2 id="final-touch">Final Touch</h2>
<p>If you&rsquo;re done and satisfied with your improve emulator, don&rsquo;t forget to return back the values of USB Debugging and Root Access.</p>
<p>Here are the default values:</p>
<ul>
<li>USB Debugging &ndash; Off</li>
<li>Root Access &ndash; Apps</li>
</ul>
<p>You may also experiment and delete some of the system apps that you think unnecessary.</p>
<p>For those who wants to re-install LD Appstore, just open up a browser in the emulator and open www.ldplayer.net. Then click the Download LDPlayer.</p>
<figure class="wp-block-image size-large"><img class="wp-image-2209 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-23.png?fit=1024%2C593&amp;ssl=1" sizes="(max-width: 1170px) 100vw, 1170px" srcset="https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-23.png?w=1595&amp;ssl=1 1595w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-23.png?resize=300%2C174&amp;ssl=1 300w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-23.png?resize=1024%2C593&amp;ssl=1 1024w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-23.png?resize=768%2C444&amp;ssl=1 768w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-23.png?resize=1536%2C889&amp;ssl=1 1536w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-23.png?resize=370%2C214&amp;ssl=1 370w, https://i2.wp.com/codefaq.org/wp-content/uploads/2020/05/image-23.png?resize=770%2C446&amp;ssl=1 770w" alt="" width="1595" height="923" data-pagespeed-url-hash="1638004724" data-lazy-loaded="1" /></figure>
<p>It will download the APK and allow you to install the app. The only difference is that it is now a non-system app.</p>
<h2 id="troubleshoot">Troubleshoot</h2>
<p>If you have multiple device connected. An error message will show once you entered the command above, saying&nbsp;<em>&ldquo;error: more than one device/emulator&rdquo;</em>. To connect to the specific device, use the following command instead.</p>
<pre class="wp-block-code"><code>adb -s YOUR_DEVICE_NAME remount
adb -s YOUR_DEVICE_NAME shell</code></pre>
<p>The&nbsp;<strong>YOUR_DEVICE_NAME</strong>&nbsp;is the name you found once you type the command adb devices. Example:&nbsp;<code>adb -s 127.0.0.1:62001 remount</code></p>
<figure class="wp-block-image size-large"><img class="wp-image-2107 jetpack-lazy-image jetpack-lazy-image--handled" src="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image.png?resize=959%2C508&amp;ssl=1" sizes="(max-width: 959px) 100vw, 959px" srcset="https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image.png?w=959&amp;ssl=1 959w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image.png?resize=300%2C159&amp;ssl=1 300w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image.png?resize=768%2C407&amp;ssl=1 768w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image.png?resize=370%2C196&amp;ssl=1 370w, https://i0.wp.com/codefaq.org/wp-content/uploads/2020/05/image.png?resize=770%2C408&amp;ssl=1 770w" alt="" width="959" height="508" data-recalc-dims="1" data-pagespeed-url-hash="554031481" data-lazy-loaded="1" /></figure>
<p>Do the same on reboot&nbsp;<code>adb -s YOUR_DEVICE_NAME reboot</code>.</p>
<h2 id="appendix">Appendix</h2>
<p>If you&rsquo;re interested on exploring more with your emulator. Here are the meaning of the command used in this guide.</p>
<ul>
<li><strong>ls -la</strong>&nbsp;&ndash; List all files and folders of a directory.</li>
<li><strong>pm list packages&nbsp;</strong>&ndash; List all installed apps in the emulator.</li>
<li><strong>pm uninstall [PACKAGE_NAME]&nbsp;</strong>&ndash; Uninstall an app in the emulator
<ul>
<li><strong>&mdash; user 0</strong>&nbsp;&ndash; Option to use root user to forcely remove the app</li>
</ul>
</li>
<li><strong>rm -r [FOLDER_NAME]&nbsp;</strong>&ndash; Remove a folder in a directory</li>
<li><strong>cd [PATH]</strong>&nbsp;&ndash; Change directory to specific path
<ul>
<li><strong>/d&nbsp;</strong>&ndash; Option to change current drive</li>
</ul>
</li>
<li><strong>adb devices&nbsp;</strong>&ndash; List all available android devices or emulators</li>
<li><strong>adb remount&nbsp;</strong>&ndash; Remount the partition drive of the device/emulator</li>
<li><strong>adb shell&nbsp;</strong>&ndash; Access the shell command of a device/emulator</li>
<li><strong>adb reboot&nbsp;</strong>&ndash; Reboot the device/emulator</li>
</ul>
