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

![](https://lh3.googleusercontent.com/UaUXQVfJoIfCLGoAIplt_Op0_Qisqh18Ac8HC1IQ5SjKgJsaETtP4R96M6t62ATNdzoLyutA2PCIgJerRBonzrJn2Al4juFAhXC_yFhiJe5tYZGnBdD9h1kd0fEjZgAoOwngFN-6VdDjaKaJk1eFEopabToo2Wy3_q92JYVb1e9QEemCY_cZo2_nryvs9jy2R-xgWXycMqyx0kyPYPos74VufCWD_GuMZSFdjVSBoCv2ZxPYLHCp_59XiFSX0bZRM5FbhODw_lMhc_1Z996zbaPNDEJiOZzRAqkYLfVC9XzKX3QFn65-M38HJtZbSW78-bdmzLo3mErEPtSIVgWxMdR74aFlUtLm-KYZP7_QDR49x1H6yleYBfSTLhWN4hAToOPbCwqTuf55f1vhr4CflLp0uF0ocxvhNwECzyqiKjC7d5BeOUXi6Bm-vcUijbfXuJmTNPKQ_3kC_jecafGpLYnkmiZb5cv6MzKmPZbWiRbZAAww5BqjNtGR1fKFOdb6hALGOwSb9Rh13x4YjdeYE7rof-iC1J-nLThIYkhzAOaHjDWk7SsauLZJojkTfh_bN2Dthv1zcM2WRqMPhxjvjFemydALtmBWJNASo_lVWXD1Pet3VTdnwJuoZ3vvnlL4qF4IYSmaR28HezxxpPl85MvIAxM8akNlI8muN-ZYpAo0WiHnxJUghqkPikofdh7fYrFy92rSFynPurbQZKJr3u_Xps3zYn08E8KLi5Mn0I3jFKVMyQ=w3017-h1778-no)

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

![](https://lh3.googleusercontent.com/TCWIH4cYQfNV_wn9ngQIMXgSmDwNebcHdq-mrfCydtF7CJb7Lt4cXZKPve3HeC9SpEIkCJUI5WkPksRKuFCbbijKBp45ed6cqww0y9QMWa9bZY858_Ektj3XLBYC-BTaUEx_3hYujlshLo6HuXPMFbHrMrE9D_Bj885_ul9Yrgls6jMxVjbpoCCLpml6ecQNNatBYfsV3bXKb5aLo4WLF_Pz9S19SkUn0-NL5c1nPyG350zHAPoQN1w4ScbSYf5Fa9TroTEGUEiZNeT55_Lpt6v0ZwpSD_z1IW1aZdV_1b-SsuEo1drxMMgkcg2RsThKXILkwKKWuSNI0ozIlh5w238jBbOAj7a3CS8Q_dk07KBx5t4-YEYWlqSn4eGsGq8JaIJ7BrG7e7Nu7ZfsgUTX-WI4MkikJDZoimKtLgmef5HWkIa1jMUTWq1KzTmiD8MwPmM2zXvZddTuoB2fgCJWCgBZ1g9bRznR2hIsN-JE4THguKh_HcznQP7yHM0x8ZDkEN0BLqKWxKamOD4SleTvcGWmkVQ_DR2HCcuJPoC6lKcTYFlWBziuASIO5dNZDW8QRcuXBNDrbIqqPJPkT-jxlXr5S3nx7uyjURHeyMpOQ1cl1_fuY94pwHuKfjB_yJoiOWACPNke1LO5Uzem4l_uV6IcucsGbPAnsaxoygAPo18jBqfk79h0CPDC8yCexmRugQVi4so29xkQ9V35M9tHomwji4mk8zVX5_wu8L2s3p51lzmrNA=w2940-h1640-no)


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

![](https://lh3.googleusercontent.com/NpFOJZWHlahDh_-Ni4q9CP0DNQliVQR84kEyADlWsOHt0Q1zpnT0utCmb2JNpy9-tOhur4u9h3e1m418JYzeBAhSrF5KIuY9GwR1907-5TtJkMIRH4lim_PLnb-Xaz2arhxzcKHq7HYdJOkTNkwhqMV1YzqmgkMcHhx1jVyin1Hd_Tuoe1uvph6C7C6VHXY3_oF2bLONKy1ftsPci0TyAlH4Sjjeq6XTAVpLKNpyU6s30ejGW_EVRozl9B37Ljht2G8Nbj6CC4prhdR9xmAOwVODvHbKSdUYOdGhDkT296cMrQ1I_Z25ceNob1xzy7mYLCljd2tLMmdctVevCC4prjYSiWLsH8rXcjKFTTKN4uK8acZHK5a11nly_AyeAmTKFJTf5mrcZzGp5feNsfS2I0tzHCriDT8CL4Fu_9-_HyEnPtBM9Q6wHXdgezB_40qR9i5YIflHlaGyQMPGpwIsGEX1MTCBDIFWn02i5MUcldPnrlf6RY7HM67BTSMUWyJXAdxjD-3g8ETWDL2J99PgPLslQP7l4sQidj3W94MXz5ESW9Guz5g-NfWEiFMqFQ2nCMpulou4EO3j4G_i5FbmI84ASvY9OgOAx6zA-eLjU1KCFuHv8GnKqVysLVB36uhbKUCnGxtw7Qspkz6WVkdYqbSJo0uCZCQeewSEpj6IYDNpUhWV26qaIZgxDGzn92xURtR6_8dHMXNtGpzp03SNZvrV19IYgSpCqhlqZ0O9yudW80DfWA=w2956-h1664-no)


### Step 6. Add Non-functioning Buttons [[link]](https://github.com/glossiergoogler/Intro-to-Android-CalHacks-2019/commit/5f1574d387237d6ea965d9dda47a7e6d042b9bf2)
Ignore the items in the commit link about edit_text_background.xml -- we are not doing that anymore.

#### A. Add two (currently non-functional) buttons.

A [Button](https://developer.android.com/reference/android/widget/Button) is a user interface element the user can tap or click to perform an action. 

We add two buttons -- one for sending an email and one for accessing someone's facebook profile.

![](https://lh3.googleusercontent.com/RKsFwIIRByi6eDNfeOQPepHicCocrVN8jfudaU0Eio9T3go2d6j0MS9h_GWJdcjJztx2DHDi76A8jtAESz39P7RtdtvcUZkrLsJwZF3eJwT_4RCcghTJNvcjDKu6h4Db5T6jTuNbK_9xriLOquyxETNuDpKtbwVyu_cE7p9YO5AFboLPQivHmDT92c7Xa6hMS3vfUpYqgyU6QQOO424mGr7pctwN2Vksd6y6SmH_UQjhIcbMX8O1uZaFYvu8GpmaBZdLfPPw87atdnC7EzWclzjT-wuGQCRDAvKxD6nd9vhkEPZcQjE1BMO-89n3O_pvSddEbxhHyJfGZnpn9NzAqI-RSHc8sk7JG-c69y_x71uoyhASDGDloVbzk5EJVhdRJvzJ8ha_xdtYw_3iwv4o2VqmGmhgK5XOAhuQ4D0tKTt-UB2Sgc1757xjMz0lNp7nwlWcHrVxTdsfX25z4giiFZI_lUWZVfUHBNdptLkTDa0Vx_NvMsyb1OytKCEDTWVXiDLEIJdu2fNEhyDMzhfmtZHyNwlsGA2hysotsnQYOuOC-HsOQsG01-PN61gPIenTL-FXrJfkBGrnlXsFwymUHJU0sYP1uAzT5_5vQ9Y9m1mDyU2EYSkxvF-65LWxpYtCuFwS3dSNGD7fvDsfiQjQQJ3h4mbWWHDy5yQkE9ugkk-LI8tYRtejkRzdvNp_uPOiUt-9ElR4KlY3KVj97FB6lQM8DwSc21gFLgb9XzKeldQRLJyQ5w=w2823-h1778-no)

The app should now look like this:


![](https://lh3.googleusercontent.com/vH2lNM-IerqGr3k21QWyZYM7-0KyxYFnaIVMuCXC1-mzxsQkjhIjKnoebGOAuHFjdyQf1PpyulsoW-ozat6jyMAT72AkFk2wJMWLiphMiWbJtjsnzzcZ0NTpxFFtbDhMWmkxfhGCeeurSnTjsSZUPd-w1JijASBDLFgt2I4rUTlP9TeWxRvg-41ypQpDkHMR9AYFXGCuNxjKtl7PMgCiB9cy_S8pCou441duxVTDAa_zwewMncK0m8CS953BKB8pCLwiXAJQDJpGNLqUzSZlBN1uUlV5PRLtCTM-cCqrhcHUGSyubkbacDJX3gJpZcvQ3d8l1tESSgUmTIGGsIcndUA9bNvBCJ-EGgZpwgFBBCW3mC8TXuoECAKvTXrlNKI-lqRtwhukj_5_9EhSAPg-KFOxFgtrISYAJbNbQI_jw6MGcctnkLlSOvUglRQbvZcib6jAifkJBmO2IhNdmrMaygyxp3agtA2GwZHqoxWxJrfwLGZYpzTwYUZVCCw-_ZtsEmSjPdPICUF_B1J0tx2clz8bJOe_C7RfZeOBfzyoKCJ2KR50cYJb52M-ryeVW_1dNpT5G2Rpz5uZ0o8O4ea_0ljzTtijglUIl3oPouXfvFRw9N5pbSrCCu5rO3N-BVrfSH1FRK1yuszEhU-YuUMWYGYK2irgfrA8OQS1tlOSKroVDRAMcS4oV2_09-P7KVqJlOmp7RzGg6nG9cFB_ZkrsPq62ZyKct0rkKQS58grtSE6GvCWIQ=w2898-h1706-no)


### Step 7A. Introduce Email Intent [[link]](https://github.com/glossiergoogler/Intro-to-Android-CalHacks-2019/commit/f4bac671e3dba8f20152fa2890bafc3a3d851df1)

Now that we have most of our UI elements, we are going start the business logic and write some Java  ☕ (mmm I am sipping Java as I am writing up this tutorial for you guys at 6am).

#### A. Add Android Ids to Edit Text and Button in activity_main.xml

First, we assign an id to every UI element in activity_main.xml currently of interest using the android:id attribute. This creates an identifying tag that can be used to reference this particular UI element from the Java code.

Assign an id to the 2 EditTexts and the 2 Buttons.

![](https://lh3.googleusercontent.com/UM0FoTUO0UgbiU9lyo7W8cuWZazBelw-MybfQqvWlR9BVGclVZsZGLdNCInihJVgC3kcICNUkKbJEWOTj2HLCM_Wld97NTu11gbaEbY0F38vtaHFw_XotuFE1C1ivOQnILz-7ZsGHjtyfZBTcCfATiru_4HIKFyUu_xrwDDqJ2etHpwkHBDQzQy_Lkm5biiGe2hGxYUEoy8AayVXCMMf5hGcI5i9JeFeJs1C0Dc2pp1GUB-GRFL3NI1gcBqMjwU2ShFEw24s8keIhFi5zq--bpoqJgJ-IW-e2PPYy10ngyqzk5fSbvKTK0RTZJWdx2jzevhGzcshBG9dpLvo9iGldqS0VJH__j31WKHJFCZfbmBI499D2cnhc1AT8wpHx6GDVx_S93Hix_FORhuyAv_MhebwKogJuF83AXMgvcUs93sbarDjhQuH30zjIFdi683JtReEygL6_qhfgtStLk1OW6zMAykVmqLi1xYL4vOZEtsuJM-pWZ2F120EVRFDuunlLaXlgAqX0Y76VHyw8aMrNOjYzX4VuFuiVfdKgokwVrorSJq1Lf9tBtJNHKumxigoPmPy9Ic51N9IdVE6c5ehzzPU9R5eHpc6S_vbiODLFAUIypYFRwdzkx8BA_YMfZomGWSlbrpVny0AMhi4HGInOchW0o5z-D9yjj6SEqyNK6Vg25K6qZ8Jl0MDX1Ro2UhJnelCRQYQJmiJWzoH0TCCDLco40wyPMj-1Hfb_JNxpMolkMNm1A=w2856-h1561-no)

#### B. Reference and link these UI elements to the Java Code in MainActivity.java

We need to import some classes at the header of MainActivity:
~~~
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
~~~

And create some instance variables for the 4 UI elements you linked above:

~~~
private EditText nameEditText;
private EditText emailEditText;
private Button emailButton;
~~~

In **onCreate()** within MainActivity -- this is called at the beginning when the Activity is initialized (read more about the Android Lifecycle here) -- initialize these variables:

~~~
this.nameEditText = findViewById(R.id.name_edit_text);
this.emailEditText = findViewById(R.id.email_edit_text);
this.emailButton = findViewById(R.id.email_button);
~~~

#### C. Create an onClickListener for the emailButton

When we click on the emailButton, our desired behavior is for (1) CalHacksStarterApp to redirect us to an email application such as GMail (2) The body of the email is pre-populated with "Hi I'm {content of this.nameEditText}" along with our message which is the content of this.emailEditText.

Let's enable our button to do something by creating an onClickListener for emailButton.

![](https://lh3.googleusercontent.com/gGiVy-b8bCcK6GhSWsHxpgYlD69ZW--UEPDX7v6xFVtQt-s8izWg7_VK3Sz7EWoWbZAVogPNS34b0IlIoiYhlBuwj3ZKV-4B9YqKeJD3twmuvuR8HNGDpriAc5Tx6GccZrZekFwZzV8nIsXPlhNItMkhjtKJbgM1QEt6lNaJhBsmy7BKdUYjvJQWJexrgMdYrxWzbY2hP-O1BVRnn2wIj4JxmLu2kfmzZJpFW6xUtZ_lxn7Zgyck528cH9eVZ5I6dXAWx8C0AJ9iV7K1ixc3wHWORiUkAHrQ0pN1Y32GHE6iB61jSWkZddiPfmB-yrPatg_od4jvWndRoHdVUeEU3sNYPJU0-mlxhaldbSeayr5Ef9E2bXej8fZa5N-r4pggiVv8vh7FZ6ZOJ7-xInShoGT7PW00V4md-ny8cRjfEhunOH22awACfyGdKck_A-4-Co2RCu-0igpK-T3h9FP_gx3W_m17HX5NZ0cpKAzf9jYcRpHTn03LKwerQL5PoB-_MOWxhComcgye64qDqZkicNzFb9t5nH4UEuylUVw1Hj5rxGt06jegmvsFOV1aL_2dtTWJO2nUzsDwAxIUZGVjEsMAuEgxquCq72EAHk6YP4Qql9FEu7EYAVZfv2Dz4BfOCH29EU9f1h5_MW9l25ZoFv8B9OQwk0ufuRem4cfcCm6wbPB7kfm_eUosQ6goLRdNE8mxahR-IvsbWYdUe-41hcJed7ROGT_66SSOnK5aTiB99eo4KA=w2926-h1336-no)

#### D. Create an Intent for the emailButton

To perform the emailing operation we will need to use an Intent.

An [Intent](https://developer.android.com/reference/android/content/Intent) is an abstract description of an operation to be performed. An Intent provides a facility for performing late runtime binding between the code in different applications. Its most significant use is in the launching of activities, where it can be thought of as the glue between activities. It is basically a passive data structure holding an abstract description of an action to be performed.

We want to import Intent and URI:
~~~
import android.net.Uri;  
import android.content.Intent;
~~~

In the emailButton.setOnClickListener() method, we build a new Intent that will allow us to carry out the business logic. 

We indicate that this is an email intent by 
~~~
intent.setData(Uri.parse("mailto:"));
~~~

We include additional information by using intent.putExtra(...). [Intent.EXTRA_EMAIL](https://developer.android.com/reference/android/content/Intent#EXTRA_EMAIL) and [Intent.EXTRA_TEXT](https://developer.android.com/reference/android/content/Intent.html#EXTRA_TEXT) are standard constants that have specialized functions within Intents. Here, they let us specify the email recipient and message content, respectively.

You can read more about what kinds of data are supported in Intents [here](https://developer.android.com/reference/android/content/Intent.html).

![](https://lh3.googleusercontent.com/6YhZwaxRwF1uhA5HsB6lFInRZ1gHsSA7x1L-5cV6l_ihhChjyTSCS6MRTVZXrobGG0bQq6kEnWVGCDDmSzcqW8_NFfUh_PleYL8bjKCnUmYJOfwXGIPvhf6VKmJjRXyRO8z_kSWmDNj-fO5YIvwJUjeW8ZmeNV52aq6BbFip-Xl_wE0jIPkbWIJNAR0ZPOdZOQK3J-I3Olk1xeXyKhNsGK-zOw_-CXy_vOllVc0I7om2kPgCIAbrpUVuPX9ZIdu75EdbMjN6pZRbRXL2KJZAdFHt_HYsmARPe0KcoUGyr0frpd4TlPPDtbR54_5dN4RyceJTHlmSI-JGJH8FYNHiAm05LJftXh3H9al_5pow9lY34IEc6rDthOqVTTNfR_YoqAKhfTq5Gv7eN9mMMH61aRsD4Rd7eIdcxYabhfHRbkP3P8WbNTPunZN291c3_NRiklrClgzV7si6OE5cW9fLVlGkbY9jTmUpSCStXbemocOHwwQrE4Tyjv-T-rCjy38QH6ho9kb25uWBU-SMb1NfWOgQy13mtZHJx4icUhi-h2ZBd8yvyWYZ5yrkLhmbYFthfauMhfH_24dYH5CsoiOyrcKROfVEudhKODJXpS5vxjlUIC7ELCy8hJ7MR-bIC-TmX9-lJqJbgflEQHwRZJinslnOkbIZTXl947bgK_8V8SPN6xv-38rETZn4CXLK-WbzsOhmK9-MOOiXD6IN2oQMvFzaGurmuAFtfWBJzTztITUrvZCHPA=w2851-h1476-no)


Finally, we need to make sure our app won't crash! We only want to execute the intent via **startActivityForResult()** if the activity exists. **intent.resolveActivity()** resolves the Intent into an ActivityInfo describing the activity that should execute the intent. If it is null, then we are in trouble. If all looks good, we call  **startActivityForResult()** with flags = 0, signifying that everything is ok!
~~~
if(intent.resolveActivity(getPackageManager()) != null) {  
    startActivityForResult(intent, /* flags= */0);  
}
~~~

Woohoo! If all goes well, Oski should be able to email Sujeeth now:

![](https://lh3.googleusercontent.com/2uWalRub5JqJeDr92y0zUO6GzNA9RHJW7Fg3UOrg1MrgZuWm8C_aVW12Ctrrbe7ujbID7PuL7Wpm0UpYNlck7CRLLJ-kO9zjhVEDtrzTvhdm6ZBE86cNgh4msKuXtI5bbFsckHpVWw14ZqVdRlqzSwhk_JlEttS7lQUrKzaWA6G0hUSPx9Yccmj9GQ5jty1VWmOni6rMxEjMHhUlMnExux_j1ty8cwQU24NGgfB7TwvnlzL6e_A15vBmqwsG-5mF8BnkImUUq3LV6jmkBxWPajXaHz4swy16GrLBMfI0mG21wSYJKLrXleYMJR7afcrhTFmNG7kJj8xo91jUz0fzVa2YIkuLPC27wPtH6L8ovf-e59LTB7aCe07Mpx_hrJPOWeVD-MwX7P1zSjUpo752OhrrcmeHzvfffzdcMQjuH0sWxqUl1HM0llsSR7GTSMyHW6WpqqeRGUFhXkd9B62gv7sVS1X_F6t6zm6asuEbuGTN05FRjmf8KAFpzMdDdcx2wP_1Z2Gy_RdGaA6T7HiadKZ9VpG4SWJCbIJi54yIBDOWkp0vARDIr86pXBCCa5cHm7qSaFm01lUOR2Cd4a7iq-f90ugcOZx9ev1Ws1UDdQCOu4n34pYyZjMr3VDPwbfE8zHvoOkYD_kv3MP96vJxMU8jpk3DvWIRUlowTPZgIVfuxebMTzwYJb7MUE3RAtim-knG-5Tab1BoolGldWAP3DJyzLo7TgzKTNtQ8of1TxQI9dK8pg=w2830-h1634-no)
![](https://lh3.googleusercontent.com/gqnDJZoSOLNg1apQVhN3diSOycvIc-XGLS4UXjSSxBhwkIi82Xi27ikccJEkgYYnosRes5-RemWUb4HGC1HAPnPxuI5wzyndx7LPl2hbsAP-EUWGobfEQwW95VxbtKEybffxg0oCOsNU350f9Q1esyqWpeCpPbKo7WQLULiJHgxwlKxyskcM0yTCpJ6yyFSxzixvqA6LqaWXKKehXy4gxWu_dZh_dixxRVOTqy1Vhp47gExvybfdl6kyhgtKXIDwPhte17tDjKriZwaEukVCqi-oFcnPaH7jP04QtSKRsz6bqUY8AQYXgdG9czZsOEI-EYr2iFyUM2l54KPkG7qafk9KmTor5Kl-YA9smketXQlL-nvvOUEaEmrhfjOvCKqHlnny6zT0uvm51nJi4fnHriiVsSdm4CjapapdYdNaTngCBjtGb--Ffsxn3NOgNabTScQRix7ZaOXdYdy41GUtFYumCx_ppmysdBpJD6ovbKJ_m7gMWAXDT2Q8yTqNEGvQ3gK3aaSxNz759Lz68TA9mTHoW712qqM6Bgv_D9Kad-6BRXYfJNjZ2NRb-yVVgoBlYy80YZ1AtqomHBM-t6_6XrYo1mjeWIUbTOxJ283FFJkaB2TuuY1lzpoC92zRISz_vhfvuURwIo-epcwzCCwOA9foSLjik9nItmb2xLglyxQRMNBVLk4YH6EpBr2llWBwPaOnvdz9ms86B-v8ZIrQDeTqsmwpnMtqbXToy0I_pkOiXyPtsA=w2712-h1674-no)
![](https://lh3.googleusercontent.com/lcHSLpYB3M5iA1b_egCSPuyM-MadlfIYU2DJufQou_fNhkvFZpmEqj24igJHAhVWQVxtskBAp9RTVifQkPDgQ7dtnmIQVVcZewfrSdxmPPX_5ON_SPCVVsQheqgJDkFopy35V6rGCjk5xcW2ZeG6M0LI-KFYgG_8Ltm8BtjKgLlN9Ty1xxnSA2E2yP3USGDqadEBAD86JRzs2MSlHebxZeLKOPuCY_I7P32jCXvgNru9U0-7FXepRlM0_Fe5klSBt9u6-GFTTmCIbjVu4U3x_bT3BgxASfZFzC37iZTr7by94evimNZpFnE5_55fEtbZuJVhQQO8ExCI9lCRJSFBJB8vhFGKVQ95Mi2tSDHVbzIDVRjIwGz7Q_QO80kS1IH9FaivE-0qS6hDdkr4HdFbWDiU49Wsbr-acMZqX8yzPZu4GyL91jv1k7Y4WS2E6m7gk3huPg1ZRoIpUEWNxqr1x7fldL8sehzQv0vC3P6spWxK5xXu_pSIHAJu5uHh3s6edI8vHeBUSeekG4cIYpxMGUEIOw9uTc_w5OiFa5fEPqyJQRiHZ5hmh7x4-9exArtNFt1z_xlDeiErvJdkHTVxEWStuN8SUJ55CmhXMa4OKmBcXY_Y6kpq5vuK5OttchADE5Nrtmc09qoaSNig2HrTxnAoPSltED3VjSabD5XKveZFz5kBi7QbolWWqBQ_55XgYi-ahqWmd7h8-fL-fguDpiPkMaKhw-ZBcUF0T2LBKvVmLcHmQA=w2410-h1692-no)

#### E. Coding Challenge 😮

Create an additional EditText that says "Recipient Email" that allows the user to choose who to send their email to, and work through that logic. We don't want to overload poor Sujeeth's DMs, after all 😉

### Step 7B. Introduce Facebook link Intent [[link]](https://github.com/glossiergoogler/Intro-to-Android-CalHacks-2019/commit/f4bac671e3dba8f20152fa2890bafc3a3d851df1)

### Step 8. Add Firebase

### Step 9. Add Write to Firebase

### Step 10. Finishing Touches


## Additional Resources

The codelab I recommend the most for learning about Android in-depth is the one provided by Google themselves: [Android Developer Fundamentals](https://developer.android.com/courses/fundamentals-training/toc-v2). It is well-documented, maintained and kept-up-to-date, and even has a series of accompanying [video lectures](https://www.youtube.com/playlist?list=PLlyCyjh2pUe9wv-hU4my-Nen_SvXIzxGB). 

Additional Notable concepts: 
