
<table>
<tr>
<th><img src="https://github.com/Aayushpatel007/Android-Security/blob/master/android.png" width="150" height="100"></th>
    <th><h3> Enhancing Security of Android based Smart Devices: Preventive Approach </h3></th>
</tr>
<table>

## Abstract
In the current era of smart devices, mobile phones are rapidly emerged and increasingly being used as primary computing, communication device with sensing capabilities, running more performance intensive task. Secure and healthy working environment of this smarty is required to be maintained. Major work is done in the area of security, misuse detection, privacy of data and threat detection and even efficient solution are also provided by the researchers. Though sufficient peripheral protection mechanisms described, authentication and access control are not alone sufficient to provide integral protection against intrusions. This raises need for smart analysis techniques, particularly in application code, to materialize. There are many security detective and preventive solutions available in market, but still this research field is immature. Majority of solutions provided in area of Smartphone handle specific issue for particular device and environment. 
Our goal is to identify Unsecure permissions going to use by the applications after getting install on device, 
As prevention is better than detection and cure, intended to work in the said direction, we define a framework aimed to help, identify and warn users for the resources going to acquire by the applications downloaded to install on smart devices and the risk behind resource acquisition / access. That way, it will try to intimate the users for the resources going to acquire in future, at runtime by application processes directly or indirectly, can uncover the malicious intention of resource access hidden in the application. Having this in mind, our solution will establish a strong footstep in device security in the form of preventive notification alarm.

For the same we focused on Android based smart devices looking to the popularity, availability, market shares, usage statistics and download statistics of android app, also due to the open Android’s philosophy, benign or malignant applications can be published easily with limited controls; Android is having very high risk against security and challenges in working environment.

Keywords:  Access Permission, Intrusion, Malware, Device Security, Dynamic Analysis, Security Risk

## Proposed Framework to Enhance Security

With the objective in mind to enhance security of Android devices by providing intelligent, resource intensive and robust solution we proposed a framework. Our goal is to provide a preventive measure by warning the smart users at the time of app start establishing its footprint into the device passing through installation, for resources going to access by the app in future. Here the purpose is by providing alarming notification, user come to know about the resources actually required by the application, risk associated with it and that way the illogical access control permission acquisition intention will be exposed. So that misuse of resource can be reduced, privacy and security of personal informations reside on device can be achieved. But it again depend on alerness of the smart device user only.  Our idea is to reduce the damage going to take place  to the device by malicious activity performed by processes running on device as a result of application execution than to identify and take recovery actions after device is harmed maliciously. In later case recovery and cure will not be 100% sure and even it needs extra efforts. 
We proposed a monitoring and detection framework to maintain and provide safe working environment in Android base smart devices (Fig.3). It will reside in application and application framework layer of four layer Android architecture. 

Our frame work will continuously monitor for the app download event and as it will found any app download, it will analyze the components of installable application. From this it will identify all the resources required by the app at run time in future after it gets installed with risk factor associated with it. The objective behind resource requirement assessment is to identify needless resource acquisition done dynamically at run time by app which can be used for malicious purposes. Our aspiration is to prevent such misuse and that way tend to provide security and privacy. Our intention behind this work can be clearly understood by taking one example. If one user wants to install some game on his device, it will be downloaded from the app store. If contact / camera or any such resources acquisition request is there in the app code, which is in reality not essential but for malicious purpose it is defined may create devastation.

<img src="https://github.com/Aayushpatel007/Android-Security/blob/master/img1.png" width="350" height="350" style="vertical-align:center;">

#### Supporting Android Versions

* **Android 7.0 to 7.1: Android Nougat**
* **Android 6.0 to 6.0.1: Android Marshmallow**
* **Android 5.0 to 5.1.1: Android Lollipop**
* **Android 4.4 to 4.4.4: Android KitKat**

Note: This functionality doesnot work for Android Oreo and later versions of Android due to deprecation of services like Broadcast Receivers, Background Services, etc.


## Implementation Details and Results

Proposed framework is developed for the smart Android devices with minimum SDK version 16 (Android 4.1, Jelly Bean), which is highly used minimum mobile version in market, so our work can cover majority of all the smart Android users. That can be justified looking to the latest December, 2017 statistics, which says that 99% Android users make use of Android 4.1 (Jelly Bean) or higher version. 
For identification of risk factors and permissions, we used PackageInfo, PermissionInfo and ApplicationInfo classes from Android SDK.
Figure 5 shows O/p generated by our framework for the Sales Master App selected from un-official repository and figure 4 shows Outputs generated for the BookMyShow App selected from Google Play store. Our frame work analyzed the components of installable application and identified all the resources required by the app at run time in future with risk factor associated with it as shown in the figures 4 and 5.
We assessed the performance of our app for different sizes (2MB to more than 30 MB) of Android installable, where we found that it takes 5 seconds or less for showing us the analysis results. Our experiments show that our framework works efficiently with very low performance overhead. Even we compare our outputs with apps installed on smart device’s app permission as “APP PERMISSIONS” from settings. One such for Sales Master is shown in figure 6.
From the figures 5 and 6 for the app Sales Master, it is clear that the results of app permissions are just names of permission going to use as in figure 6 which is provided by installed app’s show permission utility, whereas our output give one an idea about details of permissions and risk associated with it as in figure 5. Even our framework will show all the permissions and associated risk (Protection Level) automatically when any app is selected for installation and user need not to go and select the respective options to see the permissions. The users will get the notification in the form of warning for a specific app before its installation gets over. This provides preventive alarm before one uses specific app.


<table>
<tr>
<th><img src="https://github.com/Aayushpatel007/Android-Security/blob/master/img2.png" width="240" height="340"></th>
<th><img src="https://github.com/Aayushpatel007/Android-Security/blob/master/img3.png"width="240" height="340"></th>
<th><img src="https://github.com/Aayushpatel007/Android-Security/blob/master/img4.png" width="240" height="340"></th>
</tr>
<table>

## Conclusion

In this paper we gave an overview on how an android based smart device can be securely used. To overcome the loopholes in work done where major work is done in the area of intrusion detection and very less amount of work is done in the vicinity of intrusion prevention, we proposed dynamic preventive architecture for android security. We show the results for our proposed framework and compare it with the similar results provided by the available utility of Android smart device. In our previous work we proposed design for our framework and in continuation to that in this paper we show the implementation scenario and the results. The results are tested for different sizes of apps from different official / unofficial sources to get the assurance of the proposed work. 
