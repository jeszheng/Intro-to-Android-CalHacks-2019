# Introduction to Android @ CalHacks 2019

**Foreword**

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

If you have a physical Android phone to test with, follow the setup instructions [here](https://codelabs.developers.google.com/codelabs/android-training-hello-world/index.html?index=../../android-training#5). Otherwise, briefly read on how to use a Android Virtual Device (AVD) [here](https://codelabs.developers.google.com/codelabs/android-training-hello-world/index.html?index=../../android-training#4).

### Step 1. Get Hello World Set Up and Background on Android [[link]](https://github.com/glossiergoogler/Intro-to-Android-CalHacks-2019/commit/dd2e1fbcb38c334a330edc21e16572dbf7e1bb77)

#### A. Getting Started

Open Android Studio, start a new project, and choose "Empty Activity". Name the project a cool name like "CalHacksStarterApp". Click finish, and wait for the Gradle Sync and build to complete.

![](https://lh3.googleusercontent.com/GtbctSawYyI5xqmUegtEsIfqr8gR6ECdhlVLns5rCfCmx6soZSLmkZNozpSDxRT58YusxgdH7htsa7Ib4yGNPHqjb0bvdRB9oeYK5S2GmIEorkutcZ2HMrQJ9G4Gq84bfZ1VHMPkh0i1IpF5aGUO65BU16MWaYfUrXOh85CfTD5JRCIZkCs5VqL1Py_C35-g2cE88fNwk3yGp5p43RnuQBu6mNXKdt8CYk3C7vid2qIiSHMOwOPIKd6p6knz6ssA7d0fBiXETvr0UfxpbFHA9DnEiAs0n1D6JlBzQf6Frdo2uV9AjlGzkqm_RJerh-aY-wS-bg6VeurxkCUiq3zmBlauvZ8kATZ9B0Q4_9zs3LEDywAX9wqw2ES459HiW6xJ8ixjg4e4QE9YURS83Hnw0agvnmx51HM4Xs_6bsmdoKITdwWId0vtd4A6tPv5dCdszoE2iZ62AXZsKd-Nu3mUS-2qkOQ_sabImgF8n1mPX6DCR7nKApNLLlFtv2GZvKkiAowj-qGb1WgW--661Tv2xmwuSViV90frIG6wPQDCS77kA-harvcFaGsX1XydD_QH6XVIurori05SnSXp1riBL5edb1Y5LnlXBSdxfb_Ll1ADq25XABwCuiF4lfmeH6upBppKSGnscfsWCmWAy-awCSOpS39Zij-BDTNiGHdt69A7NPuAZSK7qQOs0Kmwf79lqYGIzO3Xqixfs8IxT3fucHvW8QUBrBQ0p--6J2_rE8OmiN656g=w2310-h1702-no)

![](https://lh3.googleusercontent.com/Z7FXLY4eQYiV3IcnlZvCrliuS1tdvAHy4_z9hdNBcncdDG8So2GoaTXZzD2yfHwvvMa9XW7GWU0FCv6_Lk3FzcPoDZgOrBIcDcbp6nKRHMEiTXd43sdVedTipRN3bfMvrI9XUiz1fhHOFhN8orJ0j7Q07J4Psc_ltGmmjBGJ8KcBPiXuPr2nafI8KBNtxaAwRsfQhBIjLqWngdfT4lbucd1r0V70WoM0YghMo7GMUZmm5xdXIRTvs2aPhRHi0OW4oxu48ueRM8eudUkrmpBKVZ3M3IsqpjTl_eNjUnBp96L28appdNsHGb6i9rXynr-WLRDflgFQsa95Ar976h5-IE-eylLc3ZbWMEjQxww50TZa3aynrwSN81Vvub8P8flo0T0BoPX0WYhT9IZoulFt-tre8dh6SizcMrT-NM9Ezsm78xTGdLymKvwZlZRy6IpGC2jTziWSbijFMOasJyURwhD_CXMGi9nyqpsOFysJQet3qEBbQ15YX73Bp71Qzo-z48-3PaYlu-Xc1BtRo7MNEZoiEttQ4A-ohMscldtlu-sujhMbe-ZaS8naqZmhrl9_cm-x3b8Ut7iWERU0rBHa02bSh9Gw1k2VrIqTqL5m6-v-IG9L2kq8yvOuhd0MiGXC5NeoPszRRO5tg3RRniQAbL9QO5b3UqzJ9Z7rq_cWZBuZcExrfr8kTKju=w1988-h1578-no)

Let's try running the app to see what we have now. We can use an [emulator device](https://codelabs.developers.google.com/codelabs/android-training-hello-world/index.html?index=../../android-training#4) or a [physical android phone](https://codelabs.developers.google.com/codelabs/android-training-hello-world/index.html?index=../../android-training#5) to test this. This is what we should see:

![](https://lh3.googleusercontent.com/SGItDJWEShfRcVNJ8Iy0V2t7qmTf8_SQcpwDp1T57ce8JEVZM0yt5mFVJWWb7yfyniXqOAKIhZWcdr7fV9OB1bBOXGQpY-IW4KgZS4JRPaXdcEY8OzaKfki4zuA-1pQ6vRXjiraIEjj-LvKKEATvOoOeWjXzJ7DSAYTsbt13TWUi3prWfpzER_9mK31ym1wrtG0Fe-QgPEPPde_SMqHlhaGDvCc7O1GD8BBRjOozdS2CcIf6o64VZmzsKDMOprrVj8-rSgplPJ4TMOxrD3g0hAhJXmNjgCcInUvdltZRYbVWgYIWmmVCCTPE6LRsMyJWEfV8rDznm4EUz79hg6j1XGYgPAAM4TxwT-m0Zmm9ETaf8K3jgLHtH0DiJMWD_irObKaeAShGBdfqJbZEzPzd2x8JF9dx5fHRIzMdY--PydXexklO3UmmK9GCq7j4ORCQtsY50bwK-RqCZJ6L-pDrUaijQAmYmO9AUph2YdM9vr5Hm-SuDyiJSJ6XXVQPDZchsYomv6F53n3LtrsXdDgpD1__i7h5vWtxgCz4xv0cMNnoo4qRvBD_TE9MPoZDo87OP6GeBGGBNDQ6H7ANAIEI82N59SKBiSEhM9VhUBtWLxM7nQc0HegT5BNgNxXL8RnpogEfgT5FcnObvs9IZlwfjbELENS473gTELFaPXOGMVT19Z1JzqEQHYNPgFfpLzA09Fgy997gHjGbxBEChAkBfF4qlk-QHF_BySFzFhTD9ajIEFtIjw=w2993-h1778-no)

#### B. Some background on the structure of Android Applications:

An [**Activity**](https://developer.android.com/reference/android/app/Activity) is a single, focused thing that the user can do. Almost all activities interact with the user, so the Activity class takes care of creating a window for you in which you can place your UI. In most cases, activities are often presented to the user as full-screen windows, so for now you can think of activities as "pages" in an application.

A [**View**](https://developer.android.com/reference/android/view/View) is the basic building block for user interface components. A View occupies a rectangular area on the screen and is responsible for drawing and event handling. View is the base class for _widgets_, which are used to create interactive UI components ([Button](https://developer.android.com/reference/android/widget/Button), [TextView](https://developer.android.com/reference/android/widget/TextView.html), [ScrollView](https://developer.android.com/reference/android/widget/ScrollView), [EditText](https://developer.android.com/reference/android/widget/EditText), [RecyclerView](https://developer.android.com/reference/android/support/v7/widget/RecyclerView) etc). You can even create custom views. Views can encapsualte one another.

A [**Layout**](https://developer.android.com/guide/topics/ui/declaring-layout) is how you organize your views within an Activity.  A layout defines the structure for a user interface in your app, such as in an [activity](https://developer.android.com/guide/components/activities.html). All elements in the layout are built using a hierarchy of [View](https://developer.android.com/reference/android/view/View.html) and [ViewGroup](https://developer.android.com/reference/android/view/ViewGroup.html) objects.

![](https://developer.android.com/images/viewgroup_2x.png)

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

### Step 4. Introduce Edit Text [[link]](https://github.com/glossiergoogler/Intro-to-Android-CalHacks-2019/commit/d6fbdd8e8bb1b2dc929320375c9708856de4b7ab)

#### A. Change the string within the existing TextView to something more relevant.

I chose "Oski the Bear".

![](https://lh3.googleusercontent.com/2ddpqb5T_OUpfzy09zMpcw9K8fWv73keZi5AY5htYevSWr9tSI30McJMcadbuRJall3ibVSJ-rigyJW6lwj0_pyRU0iNaYelD_ZL1XCsqn2cLx9B6fS5hk8-UUDZ4Q0RJe3JrQp0ihjM-XRxx0VurxgAJ4X2Ugs0ivRNvq-zDEW3WAzS_RZb6JEUvXHNbr21Fq_0hAwxyh-qf5LCbSR1UmBrEtec_kvIcM39MxUFYqsX_G6N0w_Lk4lxG9LcH7I-qpWe_MZs4WnxgsWPFoHjlP9jekWiE4Dj4MiN-lazAIISP1mbSijO0-TL82xABJvU2AjTlr13tvua_HYoZ91TSQH2w75R_IXyLlvA3_mJJcisnKMA-u3Bebi1ue28xoA139noYcZgFS2DWTtlkAMK2PNHjWlSePGHNT5RnRLCZB3wM7cM2YTSQW6v8ly60nuh_L7vpspPwvN9Fy8uCyrFofpacRtbAj0RsywwZi8jBL9h8CdGz3WWE3bUxawLaIC0V_UCb0EYd1GkhAmb6Wry1JNpO-Tubvu3ui9byt5fjEsAVk4zB_xaS1tI0_ttKTAMb9Q5dv_p2qlysVal9PHHp287Y7MEdb0gqeP3kS2CCpsmOUf8-gPrrF3SVnISZIAH6gGdRtlnoHcakCo0wUzmxCe_jutA70PW5rqNduw8SLYjby_lid-4hKxBTIaR07D9FJv0WAaPjwMpygUfm_mwf0wHwCDNJA_uCteR2SmkoRE118StoQ=w2858-h1778-no)

#### B. Add a new TextView to prompt the user to enter their name.

This should be very straightforward -- duplicate the existing TextView and figure out what changes need to be made.

#### C. Add an EditText component to accept user input for the email.

 An [EditText](https://developer.android.com/reference/android/widget/EditText) is a user interface element for entering and modifying text.

The android:hint attribute is the greyed-out text displayed by default to the user that prompts them to input in the requested information. Here, we set it to "Enter your name."

 ![](https://lh3.googleusercontent.com/lMusjxionF7V_Jowpdozd0l0cOjo9z_jZUQ8eGMQdcS-AFSjxBlQlUnEHpBs-2ZRvx3vtmdJ0tGl2g7kPH7BVHksAWPNM8EWtWOOkSaMAZCq2LyOUGvGW1RpJ1KdPFc2WTiZ7i_Es2qFzGAKIyiYMectl824XIkzi8CijH4l1_0ee684dS0dqUuH5iyYmEcVZULmdxDIERBZXnUst1s5ZLJaBnCfONl1diT2dK0IX0OPBgmnnhD_fV75Yqqq2tMvdEQ04r5bWa1mZejvaprEaf2CAdhsoYAL0Ty97sN-247LcQsWQ1S7YesqZb33DqNxED1K3yqOUeQ--aXX6hcklGsejiuTXu_TzPakH09E5jkHlbwZVuoVe6Du2kcFhSlTzyDgYvDT9U7-dWoCY0PNiztiUjen6VaKXyjhqp-v0DkA1XLDlOQmOLelCJO3gTcWwAbDAq2DM6yEbK7REzw1SSsZOR4jpNLkDJXf0nFVfyvEIWmrAQWEqK29LXfZASkBVxXCapQQh2_Pp3Rb3oA4r-WS6UW8sBMRgLdRwx7UqXo0X3bLHlTnTL7Sk5yBii-piB1FzwmaA24sYTYRvAUHGYAkt14NTKvfw487sQELNs3v5epLETnFONR76LwqNWl5nRhF1BAw1LAgLG-GumDObbXAF25cDyDNXy6iqEakocojcqczx3iswWpgIOGDVAd-Kqmfe8jUK16JqPTowj4APIRntZwBHdER_iJNuZQd6cJzmZvteA=w2813-h1778-no)

Now the app should look like this:
![](https://lh3.googleusercontent.com/Kw5BEZTt6PAW0VB_pVOJ51mmTODBmD3Iorl86unDBg2y95jIfEGpMCac7WwNhOQUZg_aZB8WpMNI4BPJcozmlFzehThg2H9qnq7fCrUzvRlAo8C4-48pPUOwH-NVxEP0zGDunqLqMrfYzQ0sjXmCzM9dsucNtcgu7JOydxLvDIsj-0vzGSD0pWwtogxGGQmDgB8PTvyZeEPbLzbhkTVLmfnxb8576cSocnkMy25m9H-FFbjP_5Xnqb8SbAI8fTx6TIjSufFH1pqCEveKTwjZqPJncZWRPaHerCIZ1bHbav5XOv5H23FHKM6rPkAW3IH4uwZhWFNJM8QJy6PKlOrGVuKHMUOCwMglV19In4XeCPWwFcNlA9oQrjag0id7KUf7sUqRYv6ZtgN7FTFmk9F5BKZmTwGLFods3YkkUdiU3km1MqJT2iOW1OELZFOTiS8CqDLMc41skZtH2xEheKFAgTkIYh3hazMIdJYeO189PvKRTFywx45e9n85OC7--pSSnH_Rx8x056hO5_fXSq_HQQAtaRVFCguxNz17EP8p3G5tKeIWsoTI-TLFayRqQ4sVlvDOKgAeY43cJrUwsP89OyhcwWlYdzW-Pq1Lf6Iwjz8083NsYqW4ewJt912rMdDvJEPBr8tUyJ8O5Cr76jypXx7hnWvChIYzaRH1MC3Zw5vgFsWQ7MYUN6Y6sOTGAKpd0JhzENE66Ek-is5yKNkkPjyit8C8q0qRMG8lb_RjJCda8IPQuw=w558-h311-no)

### Step 5. Introduce ScrollView and Minor Changes [[link]](https://github.com/glossiergoogler/Intro-to-Android-CalHacks-2019/commit/15888b974970aa742af50563165f354e9f3a1db1)

#### A. Set the attribute android:windowSoftInputMode to state "stateHidden" in the activity in AndroidManifest.xml

The [AndroidManifest.xml](https://developer.android.com/guide/topics/manifest/manifest-intro) file is a file in every Android app that describes essential information about your app to the Android build tools, the Android operating system, and Google Play.

"android:windowSoftInputMode" controls the state of the soft keyboard — whether it is hidden or visible — when the activity becomes the focus of user attention. You can find additional details [here](https://developer.android.com/guide/topics/manifest/activity-element).

![](https://lh3.googleusercontent.com/wtcvwDrygO1PDLrs0nybVjSbZVhlndhbNCpf9mMeZcPVhhI1c9IpolHnubzrF-3YjU6oQ-yNKuFaMwBh9VZFRLpnerxRNqYiRmTHaSG42opG0eFzxLIuPRyNaEO0ugwSycUMl0ggULzbq2KGs0Ae5UNW0_u5YwZ2CUYJmSCN_8L400lNYvKeyuqhioNgXZI6i5or-zg-r8R1jXhQ52KOobqa5H1izfWjlBJjy7u6vYzgBqHI4F1EXAMNbdd5jo0RrSpd1IF2VxpAlfE7al34Apq6EXoOH1tQHsRk39tsTFHy7PBNlspHNWpNjPceq2FYeFbcnWg6qvWvdE6u40vfxAI4dUqAfv2vuqXKKAkgI9KVnNcVpCpqWq4rq2_wKLCaGn4aLXgtaPdObZL57js6_lvqn5-qDo7JryN6vnUcmCLIsaMEtizGz8EHtKjD8KcgdxIfuqN5zMYZAtzPDst0n5YIbLTS66jNVaXLcfIxOwgmkPjWWXHxsddKaIrFqwxDnpTETAvZ-5COr_n7Kr0BdaUXyCazmWh0egd8YD03DbKPVVjsiITcjcKM0yOUHGK4bRbRHGKzv2gDuxFdv0edfzaqB-UfCQxSPt-2PFEyOV_QMdRHIqm7Rl5-3hlvsaKuF_0y5Ysui4x9h5F1dGCH9v6RwbieLIBUJMUqQdyE9YvzpaGMQVnVxYk01stK7rHbPkdIXzSpIjXsnpdmAg_v0s9iVfnbdrXcS4uCeL9EWCUCah9Yrg=w2781-h1136-no)

#### B. Add another EditText with the hint message "Enter your email to me here!"

![](https://lh3.googleusercontent.com/eQVKrvlW8W4ZvUvgII0gfuDZVFYL-HgVjzd9lo5QTYIyOJyjhSENz3DvUsy1ItIT_Mx4032dyWsPX32g7z_t1cIMj-mrrzQMkNsS6n1z3mpxp1x64RqMgPjmwPOmF13-Oq92Xcj645W_XjFrewfkjWBIZJVYbBAaDx3K7v7lMB8QU97aCpzhb7YzE1Uq1PaC7_3yAaM5QNG0cPe5JsIIbd9W_HB_AOHZO_0pGFWpChRbD87is2tSqJeIPGqH-pK6hm8Iww63D-Y5-YqqNytY_2VW1wTkIXoFSactEImev7B1Fbvnmk3kMltgjRbmHYeKdohZvQidD52tiSGKqoFMNIQJce1G5QHnsVZ0A6Y7z53QifWA9lK1kWtIqJUYyWCUyaRxo5hPHsWF5_rceBs1TRNsTC1hZeFZwm7Ec1THFuFia8KAwQ0E79XXizDhflwZpkrDiZeJqUaUF-SBBnS9wtS8j3llKCCEaOqmUoBL97MWIjwyB1xAwIqfX8lQrDNHvsqx9g0a4y0JgkEY47d0v90l8n-3OeVdBiNW6Xogq4BaAwJKbP02KjOTI5EXBV9xjV49RXRILDVztR8t0f6xlLJPkyuGJwTEx_eW-HU6aV2wa4s5C18xvbIOeu60F1S-Pw6vv5-xSf47kJSbf81Cx3cP3Cmk2i4Xock6iOrUVCmh8QtP4brML1qN9Y6UwxQBuS1JWqNwhXlfF4RY2CzpDcIfwBFjB4LTnpMcPX-XCyb13gX-cg=w2871-h1296-no)


#### C. Surround the LinearLayout with a ScrollView.

An Android [ScrollView](https://developer.android.com/reference/android/widget/ScrollView)  is a [ViewGroup](https://developer.android.com/reference/android/view/ViewGroup.html) that allows the view hierarchy placed within it to be scrolled. Scroll view may have only one direct child placed within it.

However, we want multiple views within the [ScrollView](https://developer.android.com/reference/android/widget/ScrollView), so we can solve this issue by making the single child a [LinearLayout](https://developer.android.com/reference/android/widget/LinearLayout). 
![](https://screenshot.googleplex.com/ZLtJF8nj0W4.png)

Now your application should look like this:
![](https://lh3.googleusercontent.com/8BoCH0lTXvM7yKCXcd9hjIb5ZItuAsj3vCE7BChtD2gLGmn9ARJBvCy81GtYbFaZY1h5772NsN_zLEn1rFReTFH2H_qZK9xIUitFPW0_SQOMR9qMdWuOmPbc0-H9V1diYK63ENTFMSrRWjirl7JkNWFtVhsvL9kfZT407DIe3VfJp4QMGSQgb9ppnmUoEBm-oOcC5yRqXU4D49IfVHnuB6xfatnFheVsyUJUWvtuhdC2IM_IslXT7y5vC04VxXFtbS8xD6OXE9yy-2_qtzXRLyRAADRqPC5ZyD9aDQjICnEuW3xNiIdinqvzMy5rSfY4Oap9kDibsV9gruSX7T7asbfFSD8k1bYr9xDyY3F9ZK-rh7YavSSpVnKaJnP0i_cOrIkN6R7uB1lXon13q3JCOSU5q5T6ia_XwjzP04nG2BwnmGr9PgkmjcBqY6-bj__dZTmmfnSBG4qWSSV-rpaTwv3wyAjtfQDNRT_oWKLVS3WsTYm18h2kZ27oy3rb4PPnmOsq-BPu5YsfEP1Ae5dPStAR-JvdtNaPsEx-J0R9bJYBY8lW1qMkLv8ESpBhy0q6y1FdVv9sLZK5Zdb0D_kIAj6gxofb6vaFCf8xmVYHGDs3jBGYz-Dbg2iSXKGdL3wJkOtcWqBlzwnYlf_md_mmbaSvzbKqR3elHiqSZWMNkTZrOG4s_WIQLj3t9D8RLtsp6GH5PQjJC7ufmyasr94ojuQXP3iLJIGPqrBiZZfXSt1qR1Vw0Q=w512-h288-no)


### Step 6. Add Non-functioning Buttons and Styling [[link]](https://github.com/glossiergoogler/Intro-to-Android-CalHacks-2019/commit/5f1574d387237d6ea965d9dda47a7e6d042b9bf2)

#### A. Add two (currently non-functional) buttons.

A [Button](https://developer.android.com/reference/android/widget/Button) is a user interface element the user can tap or click to perform an action. 

We add two buttons -- one for sending an email and one for accessing someone's facebook profile.

![](https://lh3.googleusercontent.com/RKsFwIIRByi6eDNfeOQPepHicCocrVN8jfudaU0Eio9T3go2d6j0MS9h_GWJdcjJztx2DHDi76A8jtAESz39P7RtdtvcUZkrLsJwZF3eJwT_4RCcghTJNvcjDKu6h4Db5T6jTuNbK_9xriLOquyxETNuDpKtbwVyu_cE7p9YO5AFboLPQivHmDT92c7Xa6hMS3vfUpYqgyU6QQOO424mGr7pctwN2Vksd6y6SmH_UQjhIcbMX8O1uZaFYvu8GpmaBZdLfPPw87atdnC7EzWclzjT-wuGQCRDAvKxD6nd9vhkEPZcQjE1BMO-89n3O_pvSddEbxhHyJfGZnpn9NzAqI-RSHc8sk7JG-c69y_x71uoyhASDGDloVbzk5EJVhdRJvzJ8ha_xdtYw_3iwv4o2VqmGmhgK5XOAhuQ4D0tKTt-UB2Sgc1757xjMz0lNp7nwlWcHrVxTdsfX25z4giiFZI_lUWZVfUHBNdptLkTDa0Vx_NvMsyb1OytKCEDTWVXiDLEIJdu2fNEhyDMzhfmtZHyNwlsGA2hysotsnQYOuOC-HsOQsG01-PN61gPIenTL-FXrJfkBGrnlXsFwymUHJU0sYP1uAzT5_5vQ9Y9m1mDyU2EYSkxvF-65LWxpYtCuFwS3dSNGD7fvDsfiQjQQJ3h4mbWWHDy5yQkE9ugkk-LI8tYRtejkRzdvNp_uPOiUt-9ElR4KlY3KVj97FB6lQM8DwSc21gFLgb9XzKeldQRLJyQ5w=w2823-h1778-no)

The app should now look like this:
![](https://lh3.googleusercontent.com/lD9u9ISxZOJvyvSXHe7QpruMe78fy0uK6zMv9IaqVq3KczJTR7T9ceJRWYWhFkLs90PnatsEwtHwUMunQJnD5tnYoX26o6sMrCXFSJ4r94uHX9X9E2ZCFR24G6mxsmqWvouN3ZGIQfkfUUV-YV-juEYKd8HxdKmglFXp0hww5BkBadxbGCMJ0Eqt7P6w_DwL_sSOOzwhm_8uNPVfohcyjECAsIaA1jbALCRFQ_ndnSBDklivuNGLommhOBAPoCLqFHJyaO_AO5TIaedpqMq7TJdWXHumKmXgSxeUa-U_SiCH4QEocmJOmtDtVzwnMgMkT6mnmDz5NJgQ-mNK6cT-feNcGrUXnwpO21xcO63ZnrNmQoIhGngvbHUJhov1lXiaaICMp9EgrUmjrUzZ0Pk78YKe1j1hjrLnCLlQFE1QCYeQ-mb6Sld0DeBPFWOsbFtK06nVd8bkIFxmeVh4Uum67-QBEUCkdAKsXdW-sFr5AliE7DIbQa2OPMAKpo9Yf5gF2wr_nYffe_NRFZKJMc1RESH9CQVAY0EP1o0x0y0Ig-SSWPTUeX4BIXO2wUyVjuDj3l3hOUK_anMjXtqGaJq0lXstO2axQmTn-zBT5_7mnMMBb2pFJmyFr2uIIbGmTm1Fr-uwRGjDrZ2lSuvqbGBQ0WCmaJiQj5r5R8w-SGDpPb4OWTns3nNgBxTKqciigmb3I4vxmY6IvJA0R-_IklLuZaA205FfLwnJySiDAf2os-rRZxhHDw=w528-h311-no)

#### B. (Optional) Add styling to the "Enter your email to me here" text field.

Create a new resource file in the res/drawable folder called "edit_text_background.xml". In it, we set a stroke of width 1dp as a border. Here it is set to a pre-defined color called colorPrimaryDark (what I have differs from Sujeeth's commit here slightly, as it appears borderColor hadn't been defined at the time of this commit, causing a build error. You are free to define your own custom colors in res/values/colors.xml if you would rather not use colorPrimaryDark.
![](https://lh3.googleusercontent.com/rzcEb9KGu_HE1_Cv8iNpCn8mBJeY3Z7265NgPrIz7I4rulNFcYvxAaVy5I7_S8C05_Lx6-RvmvM3gJkVUG81G4jlKF8YSme69ugtV3TRdgWvbZS4aibF4yI1bfB7DGxPlzjmiu5gPZ8M-rD4mBcAXOSkRF8Qu9vxqLV7aOA8-8mVH-9BmfC10EcsnMiL6RsK0398qYeSM8VGnqJng975qwrMAf1nnmF4VXMsIH9mY2ufFOMXa2-ScnYVtzKO8j_mlUNQbqWV-qKr10Syf0Nay1u-_MpgRaJf349kMQfg_vLQThvBtE1RZK1Ud6Tu8mJE87PLiGvk9YN-Ogsm571Vdca1KT319r7JehzFYjrTYZs5-S3Q0XvplXaHr5ih38gO5GSEPBZ9MeAmn8QkQW9JJrwSjXG_GnHXVzYTXV3wPQ4iQfBOvAYBPm6sVcAgz9IesyVM9zq5CllDhXbefqeQQ9-CM-bsZ5DwSAgz9IrkrXnrm7Njlmh3yEpPqM5CS4ePMVQHaO4E0EAbL6cy6_FS6AELQtZyVB8xn6tlX63r8w5ic_4AYK7hMa3e-7hscwMNpQAot2l4S52dWhdoJ2roo8_oGYbiUkdoIn2hjeA4eBqGlJ9S2cO3K1BRfqh_hVGJdGtsNgCXx2BJaILPOE_26gCr0qe2F0tprDI6I7dmM3fQ3TmB5DUoFrcsLZhyCyU9CvHfQ9RTWBrSfMKYzTem33mRY9fD6EXOfzvnBPWPvQ6u3wWGSQ=w2826-h1124-no)

Finally, we change the background of the EditText to our new background resource.

![](https://lh3.googleusercontent.com/KPp5lOyj0cbt2zl7w7amtJc3y2nURSM4HgfSPpMIxAJzY0OOIOKPSbdc78B88V8RTn_1XxrzLXO5zckjEdfVlmmkREVFZJfvdr2WfBOT__wmLbp4d7nZTjvsucICrpVJW2y_Jic3kyQLUsWEZ7l46I_b0ijFpQxpoIq96G9SQRJZnmpkgkC7h3vnmNPjiW5ucGzfdEEeu4aTsFHp0DTgv_sDUBSL7G9CeFTUtdJDo3kwhMOWX7-xjOB3Nwh_IIOdsG97XDlxdSah8cwOpqoTmNstlc4-8dwM9EYhQ3IF7NVCfn5Sx8fYsN0so23aQKaNsj54eNxKHM4fB-HBOPvRIFD0UzBm9TkmC1r7q0Gqrh_TPbNzn9xEqpq_lfa4B_6wmrMS6ph1dIdaA-ct2CWyAHB9JmaveIxaWI1_lAy_EV3mOLNrd8Zjn_SgL_HTRx0yZf18MOc_mWlVXNsav-Yuk6sg6TQIpJnzy-mkMnPW4MywqffLIUqw82e1L_VpghNMhLipM7pvkv_xIy7xwAP3t4zUcRWSqYsU5pfezbxz2KfZ5yZ6V9CXDt_MP-n9cabpV0qMBLIOlnopovhBJxdEHDUV87md_nU4-Gk2cCvzF22yrdYkdt1br-sE3Gmbseeg9rzLA_-y8lj4aq5eQ7yCSqOfAz-h4dmdrMKW51IMW9r59R4DcXxqFVHyCTfInb836B32JRLadpvmQnTEww-7E-8dozOjS-4ndHSgtKr2cL3aPooO-Q=w2786-h1521-no)

Now, the app should be at this state:

TODO jessica: left off here.

### Step 7. Introduce Email Intent [[link]](https://github.com/glossiergoogler/Intro-to-Android-CalHacks-2019/commit/5f1574d387237d6ea965d9dda47a7e6d042b9bf2)

### Step 8. Add Firebase

### Step 9. Add Write to Firebase

### Step 10. Finishing Touches


## Additional Resources

The codelab I recommend the most for learning about Android in-depth is the one provided by Google themselves: [Android Developer Fundamentals](https://developer.android.com/courses/fundamentals-training/toc-v2). It is well-documented, maintained and kept-up-to-date, and even has a series of accompanying [video lectures](https://www.youtube.com/playlist?list=PLlyCyjh2pUe9wv-hU4my-Nen_SvXIzxGB). 
