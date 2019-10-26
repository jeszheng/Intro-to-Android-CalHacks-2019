# Introduction to Android @ CalHacks 2019

**Foreward**

Fall 2019 CalHacks, October 26th 4-6pm.

This workshop will walk participants through building a simple Android app that showcases Android fundamentals and programming practices. This will provide you with a solid foundation to build off of when you develop more complex applications that go beyond the scope of this workshop. Open to all levels of programmers, experience with Java recommended.

Q&A following the workshop is open for deeper questions about Android, questions about our experience navigating the hiring process, and our day-to-day lives as engineers :)

**Setup**: Please install Android Studio. Download [here](https://developer.android.com/studio). Please do this ASAP, *preferably before the workshop*. If you are using a physical Android phone, make sure that USB debugging is enabled under settings and developer options and you [follow the setup instructions here](https://codelabs.developers.google.com/codelabs/android-training-hello-world/index.html?index=../../android-training#5).

Workshop lead by Jessica Zheng and Sujeeth Jinesh.

**Demo App**

The application we will build today is a simple app that shows a user profile and contact information. It has image, text, and button views. It also links to email and a facebook profile. It uses Firebase to store data. A video demo can be found [here](https://www.youtube.com/watch?v=mxhGB-C4tbw&feature=youtu.be).


## Tutorial Walkthrough
### Step 0. Download and install Android Studio.
[https://developer.android.com/studio](https://developer.android.com/studio)

If you have a physical Android phone to test with, follow the setup instructions [here]. (https://codelabs.developers.google.com/codelabs/android-training-hello-world/index.html?index=../../android-training#5). Otherwise, briefly read on how to use a Android Virtual Device (AVD) [here](https://codelabs.developers.google.com/codelabs/android-training-hello-world/index.html?index=../../android-training#4).

### Step 1. Get Hello World Set Up [[link]](https://github.com/glossiergoogler/Intro-to-Android-CalHacks-2019/commit/dd2e1fbcb38c334a330edc21e16572dbf7e1bb77)
Open Android Studio, start a new project, and choose "Empty Activity". Name the project a cool name like "CalHacksStarterApp". Click finish, and wait for the Gradle Sync and build to complete.

![](https://lh3.googleusercontent.com/GtbctSawYyI5xqmUegtEsIfqr8gR6ECdhlVLns5rCfCmx6soZSLmkZNozpSDxRT58YusxgdH7htsa7Ib4yGNPHqjb0bvdRB9oeYK5S2GmIEorkutcZ2HMrQJ9G4Gq84bfZ1VHMPkh0i1IpF5aGUO65BU16MWaYfUrXOh85CfTD5JRCIZkCs5VqL1Py_C35-g2cE88fNwk3yGp5p43RnuQBu6mNXKdt8CYk3C7vid2qIiSHMOwOPIKd6p6knz6ssA7d0fBiXETvr0UfxpbFHA9DnEiAs0n1D6JlBzQf6Frdo2uV9AjlGzkqm_RJerh-aY-wS-bg6VeurxkCUiq3zmBlauvZ8kATZ9B0Q4_9zs3LEDywAX9wqw2ES459HiW6xJ8ixjg4e4QE9YURS83Hnw0agvnmx51HM4Xs_6bsmdoKITdwWId0vtd4A6tPv5dCdszoE2iZ62AXZsKd-Nu3mUS-2qkOQ_sabImgF8n1mPX6DCR7nKApNLLlFtv2GZvKkiAowj-qGb1WgW--661Tv2xmwuSViV90frIG6wPQDCS77kA-harvcFaGsX1XydD_QH6XVIurori05SnSXp1riBL5edb1Y5LnlXBSdxfb_Ll1ADq25XABwCuiF4lfmeH6upBppKSGnscfsWCmWAy-awCSOpS39Zij-BDTNiGHdt69A7NPuAZSK7qQOs0Kmwf79lqYGIzO3Xqixfs8IxT3fucHvW8QUBrBQ0p--6J2_rE8OmiN656g=w2310-h1702-no)

![](https://lh3.googleusercontent.com/Z7FXLY4eQYiV3IcnlZvCrliuS1tdvAHy4_z9hdNBcncdDG8So2GoaTXZzD2yfHwvvMa9XW7GWU0FCv6_Lk3FzcPoDZgOrBIcDcbp6nKRHMEiTXd43sdVedTipRN3bfMvrI9XUiz1fhHOFhN8orJ0j7Q07J4Psc_ltGmmjBGJ8KcBPiXuPr2nafI8KBNtxaAwRsfQhBIjLqWngdfT4lbucd1r0V70WoM0YghMo7GMUZmm5xdXIRTvs2aPhRHi0OW4oxu48ueRM8eudUkrmpBKVZ3M3IsqpjTl_eNjUnBp96L28appdNsHGb6i9rXynr-WLRDflgFQsa95Ar976h5-IE-eylLc3ZbWMEjQxww50TZa3aynrwSN81Vvub8P8flo0T0BoPX0WYhT9IZoulFt-tre8dh6SizcMrT-NM9Ezsm78xTGdLymKvwZlZRy6IpGC2jTziWSbijFMOasJyURwhD_CXMGi9nyqpsOFysJQet3qEBbQ15YX73Bp71Qzo-z48-3PaYlu-Xc1BtRo7MNEZoiEttQ4A-ohMscldtlu-sujhMbe-ZaS8naqZmhrl9_cm-x3b8Ut7iWERU0rBHa02bSh9Gw1k2VrIqTqL5m6-v-IG9L2kq8yvOuhd0MiGXC5NeoPszRRO5tg3RRniQAbL9QO5b3UqzJ9Z7rq_cWZBuZcExrfr8kTKju=w1988-h1578-no)

Let's try running the app to see what we have now. We can use an [emulator device](https://codelabs.developers.google.com/codelabs/android-training-hello-world/index.html?index=../../android-training#4) or a [physical android phone](https://codelabs.developers.google.com/codelabs/android-training-hello-world/index.html?index=../../android-training#5) to test this. This is what we should see:

![](https://lh3.googleusercontent.com/SGItDJWEShfRcVNJ8Iy0V2t7qmTf8_SQcpwDp1T57ce8JEVZM0yt5mFVJWWb7yfyniXqOAKIhZWcdr7fV9OB1bBOXGQpY-IW4KgZS4JRPaXdcEY8OzaKfki4zuA-1pQ6vRXjiraIEjj-LvKKEATvOoOeWjXzJ7DSAYTsbt13TWUi3prWfpzER_9mK31ym1wrtG0Fe-QgPEPPde_SMqHlhaGDvCc7O1GD8BBRjOozdS2CcIf6o64VZmzsKDMOprrVj8-rSgplPJ4TMOxrD3g0hAhJXmNjgCcInUvdltZRYbVWgYIWmmVCCTPE6LRsMyJWEfV8rDznm4EUz79hg6j1XGYgPAAM4TxwT-m0Zmm9ETaf8K3jgLHtH0DiJMWD_irObKaeAShGBdfqJbZEzPzd2x8JF9dx5fHRIzMdY--PydXexklO3UmmK9GCq7j4ORCQtsY50bwK-RqCZJ6L-pDrUaijQAmYmO9AUph2YdM9vr5Hm-SuDyiJSJ6XXVQPDZchsYomv6F53n3LtrsXdDgpD1__i7h5vWtxgCz4xv0cMNnoo4qRvBD_TE9MPoZDo87OP6GeBGGBNDQ6H7ANAIEI82N59SKBiSEhM9VhUBtWLxM7nQc0HegT5BNgNxXL8RnpogEfgT5FcnObvs9IZlwfjbELENS473gTELFaPXOGMVT19Z1JzqEQHYNPgFfpLzA09Fgy997gHjGbxBEChAkBfF4qlk-QHF_BySFzFhTD9ajIEFtIjw=w2993-h1778-no)

### Step 2. Use Linear Layout and introduce Text Alignment/Gravity [[link]](https://github.com/glossiergoogler/Intro-to-Android-CalHacks-2019/commit/9a1c6b6975b78a0c908998f48ac777134827ff88)


#### A. Change the constraint layout to a linear layout in activity_main.xml

A [`ConstraintLayout`](https://developer.android.com/reference/androidx/constraintlayout/widget/ConstraintLayout.html) allows you to create large and complex layouts with a flat view hierarchy (no nested view groups), but it is more complex than what we need. We will use a [LinearLayout](https://developer.android.com/reference/android/widget/LinearLayout.html) instead. A LinearLayout is a view group that aligns all children in a single direction, vertically or horizontally.

![](https://lh3.googleusercontent.com/yh7E-M4HqMBdH_m2umf9tp6Bl5wCkhFooRVLbdZspFfHVaRcrmwGlLHG-yXW22ow2GvyXOlvVOGBLuk1fnrJilDu4WSSph_f42wo4yqtffBdIdQVY7GjO3YwYICuFMIocE2Oh-38vIql0x0fqKPEXz-I6Dosh1LEymw2OwwY7T03ftQJPrVZoamrmnE7snS106kyvpcuxd90IFDb_hjWRIRbCypSqkGxbC5roQPWjF9OAFUM1R-uNGf4DhNOFiRGjrvOS3wlk7HB4jzRj3i277tdhtiPp7hFWptJO2JdrmIQw2rPyWZ9HcZ4SjeMoDYt4ztb8oUPCtnRpxm_R4SKuFLfS57XIOE-vmnFX81aeQxA-SJWEE01ezrz_Yj4pzQr5fhZuD0CEjVFw21BgRmggdwo4Qui6K6xZN96i3rR0w9Re3NP15NiCZGkPy8Xsus1rrDlppxgd4KqsbX0WLlUut8yNCYyksRLlvm-AYYWlcnAFJNHt5GcmNh-yUKvdYDnA5clWUcnppokSvXjeh943myjAOA5xOnM_jDJcq6LF3h7E2ffgcv5FcXAhnriEYGyueU0P9pWvLEPrKtv87LCgs8q9On7LpzgqPBa9u-_O4d3CgFUP3hLn-Ntz_kg-h9ukh_HcHFj7LEivlYwjJZRFYR07o1Rrm9VtGFUHj4UdCn23J0ZN2Fw0ed752i1-OczWzr9_lLnBYdTiuikXLWecycUUjbi-iMNbAhqkU6fW6peFqRVmA=w2936-h1276-no)

Rebuild and re-run, the app should look like this:
![](https://lh3.googleusercontent.com/7DfmgGg3Xhz6GKjSvw46w86zve4tPCtz7N1C5q6rh-gfhc7hwjVkj6FQ6DewQuvIyqCthlQJYDqMKNstcPDLg9N5edIQLpPAJ2lc7xw7YOhX3aIvcD23W0gnL7nZuvTuox1LFd5Z5bRG8_z2yDPB7gpNxNyYDCpThn4kWAycKq47etnoj9gHodICMN4_6N74l0mpWgb9uGhTEiGlpLCmssPArMUoEkVlckQ2dEP71ZtsnLubqXhIy1JzhjcbUdHt4F267jH2wuBaOJfNSvXiZD2SWDRgHtWc6Fzrdqi94Vuz1yFwZmRlfs9WfQ9xKLtQvpHKHReykbnvH-7B0CmvgIVyx1Br-cMepKq1TwPzapN3SPPqDmulJCIbNrUGFFQTXgWdF_tmX9vrk-JGOYBWWqcz_p2gDYll8eAG76WYsRaJoF1zqgwqsfwKUe-c2c8EDs7YvtAlo1IY16BC6DU2HlIijUNTrEHeoQeucePAPXBqmatD_iFC-xEXeLqY1aMjjV2AP1OxESkH7AABy3WiEGAHW6S1MOvJGZwdlWktIKLCGkX8wbzczN_O1Ski_xbEZ9vCRcZTcrxV903ah0bdQQP2kd6vWxTMVDzZTdZDS4NT93YbLPwx43pcgkuVB9mf7IVVf13YYs8hdTWKG861WCH883ERQiT8ZzEVMygelQDHC9JWCyWx_VG0eSYgpTR-QsnEq6X0DPg-MmmslQEIDGJti4ct-Vuaa-VDHMknWniEvVZk1g=w527-h311-no)

#### B. Change the width of the TextView from "wrap_content" to "match_parent".

A [TextView](https://developer.android.com/reference/android/widget/TextView) is a user interface element that displays text to the user -- currently it displays "Hello World." Changing the width to match_parent allows the TextView to take up the entire width of the screen (since the parent is the LinearLayout that takes up the entire width of the screen), rather than just the contents of the TextView itself (whose width would be a function of how long the text string is).

![](https://lh3.googleusercontent.com/OdII854SRHlQMJNKMU29k70TblrFORCmD7t34yAmpvEGGB26qq8Ft2kKXmTcxJfYgSJ94DNJ18Uq-LC3Gg6SfL2ivik2-a4KMed4ApJuTRoA5j0rBhCGbgNslxGLNco9ODj3bovBMBGpn5YTYrAVmrMspt7zVpa8CxhAr-fimrtbOAc6rQhwavQhEOEpj8UN-s290FiumFnl-Gk7ftvXhUTa_gVWXRoAVw_hXL50Dr7tnYhYCp3zLzhZaO57dRXuolAK7GNsjlK5OLwoRpWwHdWgmhokKFOjrsvDh1tgOCt9-GMP-28tCFeBLpZo10lRw80S4y5EFwRzJYxFbzMAaN2WnRoAgQ4iE_FbxbQdZsGaSkrPVl-AS81wxhQKJTOv3OOkoATg4yQDpgjedXjNFgRtGf7YH8YhscJPpBo8lz_DqL8MBAAFxG4LhIcUJF88OJdiWZXRbVSsDEZEMQDkwGAwuTPGBB1NE5pL776RGSQl3ua6S3wJ7U6nFrVUW4Zp8fIFyCS4cvQPX3taXEMXbYw_IxljWQi6VagIAHyOR63j5eVRUFENF8BFKoi2p9CcEHfickn9VlShBozoDFWbdvc2a5twqdG_nQ5xvgVmvWLHSRE52Twt4sZVS7bq6aBEj74E3vzqMSJN6dytoQGT4N_XRM8qg8NxnlHrsnQ5Uhdl18onJuHBAbGtQ8oMGeIwXl6fajr4j59DA9Q1WTWgOp6VxS5zKQgB0vFfRbviSAKlx3Zf5g=w2056-h918-no)

### Step 3. Fix Linear layout orientation, Introduce Image View [[link]](https://github.com/glossiergoogler/Intro-to-Android-CalHacks-2019/commit/ff52887b6d69cdc20dade22e8f65f881b13c4e48)

#### A. Set the android:orientation attribute to vertical in the LinearLayout within activity_main.xml

For a [LinearLayout](https://developer.android.com/reference/android/widget/LinearLayout.html) it is good practice to explicitly specify the layout direction with the  [`android:orientation`](https://developer.android.com/reference/android/widget/LinearLayout.html#attr_android:orientation)  attribute. 

![](https://lh3.googleusercontent.com/lj6g2wIIbiwErSesl9LP-EP8xTSf7eOsBUlr-wnImc1C-NUmmHMKy8QXEojOID9caSb2XzRXAXzAWqmCZXmjqLx_nDY3NuOWDUBukMI8o9oH4Gd3L8wqy71VzdcRtvB6KSdaCV1YpklnNbCba7fZsD-GEH30oMmZ4wBYV2cpx7XaQb5cgbvB1SNZBDnSyTDbk-fn-zylf_KVJk4Uf-4-lzAbSBthssUOORXvEPEh5H1A8xA5a-aWcZm27b_fy4x4kRqDDT-CuG-QI3rgiQ0uMLFSNpsiB9eX5vJ3J74p7uSM6TUenzQaMp0SMVdi-I4DlJ8CVC4t8WKdljPq3FcyrmbfI1-LUN6D18GuVr0KH_-8TiQU0dJhHYX-zc5YNfkHoPP3Atw3t6rNwY4AXZ368EebaQIleMBdJjuhgB4JiuWsfbnSvX1TAdtN9QWaAaCW4WMwYZmI-2OaXImru_m2uNFQ-KhyRjwCDJ2x0jnP15Ht3zrHyreouvDKYeHYpJmUYTbMLGu1HvERxP2Gr9GD5A5fnNEtoLzKTD_q4tpI0PeYXz6IgfU01t5OTZ_yP5B66DQCIBORccz60qh01I4PjIhyRrXCJ5wnzSbAU3IjKKYMnOBU4CLgedR-b4bow0bQwwr3SFShSzYYd8mxiDVfIQoZ9uyEvLrjUABx7URzdRZNacKXFVblAi0UN9Rb706XFyywg1yCX2O5CEoX8ndPW3GAOFZvZi9rWndOtxI7PocUZd7ROA=w701-h348-no)

#### B. Add a PNG image to the res/drawable folder to serve as your profile picture.

It is the convention in Android to place drawable resources into res/drawable

Unlike Sujeeth, I am using [Oski](https://cdn.shopify.com/s/files/1/0135/6222/products/Screen_Shot_2015-07-04_at_1.05.58_PM_480x480.png?v=1441307597) as my profile picture because this is CalHacks, not Georgia Tech hacks. SMH Sujeeth.

![](https://cdn.shopify.com/s/files/1/0135/6222/products/Screen_Shot_2015-07-04_at_1.05.58_PM_480x480.png?v=1441307597)


#### C. Add an ImageView that we will use for our profile picture.

An [ImageView](https://developer.android.com/reference/android/widget/ImageView) displays image resources, for example [Bitmap](https://developer.android.com/reference/android/graphics/Bitmap.html) or [Drawable](https://developer.android.com/reference/android/graphics/drawable/Drawable.html) resources. We will use it to display Oski.

![](https://lh3.googleusercontent.com/sTA2pcknsk_415YhSyB-IJ9mptSEQiqOXKvzYKH2ffmXbiqfvCYJcW6A8hxutR1Iuy7VV7XD577XTXGYALkmyl_6wDuMeZ5Io5ItWNkjumnaHF1OSI8lY7zjmKDNLG3Un16SHfB_rjEEI8lhF4FfmE-CW-FHoUKThd-CZt-KmDHhHLjlokQjEa8SviyRif0Lt24DdMFsQWVjLs--8tsw8Y0OdiWChug1jZ-zIiyXYSTNT70Tq4-FIel0EmJn9jkITx652hkPYk_L_LgrpapuCVkAYnuRVTUqmTGKIYa0ySsPDH8o8QRp8rq0VrIJuSlsJF4aXQdJGNyH1nxRbL1EmU2kqMjb9iDuCWsnpKiLx3qKQF2rl32Ih30byvXdm-jw855xzpZrMD1Wc272jjQ45iP3_-yEPSsWoVs5FvYlLikw9tEamDLyKeVMHU38VkpRl4fRRsHHy2Hx-YNNjKLR4GpWi9XyoGlitYMY-xxEo9vHFdzEq0GNUUeUwcdzg8NJJBK4UxpJ5OmyBvh148Da0UZEhZaaN9pmKy-7PVv4s-qtTcmZrsoZDnOWvpbSC93rOIs14zcTon5XHoT1inpQQKIBpPuGSKSc3aWn1gDULcMqa7jALVBq_8sJxHmsQwl2RhRVIp4pLwnju0iH0ndwR_z-4U4W5zKSTONqJuTF8pR0e76AmRHFDWSxlZbPAoec3C9Frn21_ivf-FD8EuVpWU1bNyC_WmriIYzyUE9rUzFom2vG2A=w684-h302-no)

Your app should look like this:
![](https://lh3.googleusercontent.com/mamc6rgBrg8syP9AFYNuq_uZwtA6yJzFumuCy3gaPg7sp0TtL9_7_0igWnMWIKjL9smN8ds7yW7v0dz8D8KV2b9fp1MwnUUxFMRa9J33dj1Sk2g7Aph5i4HM3FzBn_ymfjJMxkqzbxy91VQ3iseBxd5-MhYL5jjxtJ3sQswP13MKM1BQlMXf-gcblBUpxJ9mpVTOPnDZ8x4x-bm_w6rMscgCTxoYfa7Zs7_Dg3vvuXkRwsT3kcm7Y9dAIu42RObKRfsjFlu3jSJovRKRhu3sT-rSW6sobLPb0cdGN431Sm9VAvCyjYNte_lVaJiQjjr6iScOYeCnS43DN-zYKk2G65VLYZpOmDKHGSHhMorxFIcnKkdef53FHl3OHMmGoKqO-mx4fXC0WA36WYPS-QzyFBXOG584WRVtDFBY7tghGSb7GrZzSYO6Ijy9sIZ1Y7mWZbBTMdq7HokwOYKzmBxlLArqFA9cJQ9uXSrW9C9uUepOneyZDOkx0tQQ8tapFNV3Axnn3ev-bSxl2Gc0iTXwg6dtQM-CLKoKLCUW1TO_t0VpBJpPtJvqksScflnD_7XgOYYPTgzIIcah-xp8ipKgTfLmsiyWZx81zZBAvP1EjSrFCljtHNOXlLziwMuXiPufRmBh3ETLqCPcAWfNzv6Otk1odhBelOr8wZE8i8tasJFXdjOrU6dkuY03=w2852-h1714-no)


### Step 4. Introduce Edit Text

### Step 5. Introduce ScrollView and Minor Changes

### Step 6. Introduce Email Intent

### Step 7. Add Non-functioning Buttons and Styling

### Step 8. Add Non-functioning Buttons and Style



### Step 9. Add Write to Firebase

### Step 10. Finishing Touches


## Additional Resources

The codelab I recommend the most for learning about Android in-depth is the one provided by Google themselves: [Android Developer Fundamentals](https://developer.android.com/courses/fundamentals-training/toc-v2). It is well-documented, maintained and kept-up-to-date, and even has a series of accompanying [video lectures](https://www.youtube.com/playlist?list=PLlyCyjh2pUe9wv-hU4my-Nen_SvXIzxGB). 
