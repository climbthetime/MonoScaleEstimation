## Simple and Effective Scale Estimation Using Multiple Keyframes for Monolcuar Visual Odometry
Additional experimental results for the paper titled above.
### Abstract
In large scale environments, scale drift is a crucial problem of monocular visual SLAM. A common solution is to utilize the camera height, which can be obtained using the reconstructed 3D ground points~(3DGPs) from two successive frames, as prior knowledge.Increasing the number of 3DGPs by using more proceeding frames can be a natural extension of this solution to estimate a more precise camera height. However, merely employing multiple frames based on conventional methods is hard to be directly applicable in a real-world scenario because the vehicle motion and inaccurate feature matching inevitably cause large uncertainty and noisy 3DGPs. In this study, we propose an elaborate method to collect confident 3DGPs from multiple frames for robust scale estimation. First, we gather 3DGP candidates that can be seen in more than a predefined number of frames. To verify the 3DGP candidates, we filter out the 3D points at the exterior of the road region obtained by the deep-learning-based road segmentation model. In addition, we formulate an optimization problem constrained by a simple but effective geometric assumption that the normal vector of the ground plane lies in the null space of a movement vector of the camera center, and provide a closed-form solution. ORB-SLAM with the proposed scale estimation method achieves the average translation error with 1.19\% on the KITTI dataset, which outperforms the state-of-the-art conventional monocular visual 

*****************************************************************************************
#### Example of ATE results obtained using SEMK and GCSEMK for the sequences 00, 02-10.
![](https://lh3.googleusercontent.com/2goT4VgLx_JTNded3bjjHaHl-2ka-3kYkt1JDrRd6mzc0FkT0d3bOb0sFJJ38Z3RqPVV7O8y6iFuQF7j-shjNfgO4cx0fvAQRRmfzsJCfAYPQxlfUK6Ux5prJe2gHsuPpZN-u4j8CwmMgPO6miuLfGlTsImeXcxOckathvPr76Wt97LIH-TjT2dQVySQZDLe6G-b9yJA62eEN4Ew62WsybDw89dHPMbAH3vZIJWM1QfYcY6CiyrsuMJRGnmSBvesY0u5-6WEqrAMxV6i6H5uROe_EH_cTeuSc4DHk0rMUiNPH-_R4VpSpt2nYpJM32nkEHSUE_V7WqFtq2GKr9OSRoZB8xqtg0NHZcHeZ1hOqD-UKD07PB06DjCTkeQ93vlxrfDBbahY6MZL6OAoSTp-FPdXI7zX3ArGTekvla83gvXUeYUGbSf3a8IhehWAsGHt5Xg6f7mDCeAJ1CtuVsezq0qGpoC6wfESDY31XsuL-7EO6W59mgjVjgHWMsrO2vhx43PR4IEXtcajvpyRP12ocb5euXWEE1rHslRzFUCsjph9xUPJDhZWeXrIZq-fwKKvihkey-52OlgxTZayfMAtKgWWuQZhWjSNKbwcqyiIxKTjL1Y1PMfFmMt7TH9WCWEdpgI28ARIdiHuCuuc-aAgSrUD4xfNZMHqVBLBehK_K2eqDNg7xkbtk3I0UbYx=w1340-h1928-no?authuser=0)

*****************************************************************************************
#### Recorded video for sequence 00, 02-10. The trajectory of ground truth, ORB-SLAM without loop closure and GCSEMK are shown in red, black, and blue respectively. The black sparse points are the reconstructed 3D points. The detected feature points on the ground region are shown as red square in the image.
##### Recorded video for sequence 00
will be available soon
##### Recorded video for sequence 02
{% include 02.html%}
##### Recorded video for sequence 03
will be available soon
##### Recorded video for sequence 04
will be available soon
##### Recorded video for sequence 05
will be available soon
##### Recorded video for sequence 06
will be available soon
##### Recorded video for sequence 07
{% include 07.html%}
##### Recorded video for sequence 08
will be available soon
##### Recorded video for sequence 09
will be available soon
##### Recorded video for sequence 10
will be available soon

*****************************************************************************************
#### The estimated camere trajectories using SEMK for sequence 00 and 02-10 in the KITTI benchmark
![](https://lh3.googleusercontent.com/pw/ACtC-3fpxjxGrH9vo3aunm7OQlyg-VUT-TtbkOlRomXZZIiFXR_U-j4NkRO6L-5oqwTL2A7WD6UmKX0O8d9IKFGLhk-NtVlWotDj4W-uBuGPvH55rFEC5FdX55SE2NgX7RbmSZ5epWd4J-wo-Bv7SEjdChKC=w682-h984-no?authuser=0)
![](https://lh3.googleusercontent.com/pw/ACtC-3fcM9mUw8NAds1as8qoTsAdJLfhA2VolYVrZ9Age-XeyCp13l_lC6sFWu09uOzvTUjTWbU0k4gRk6X6ryM0n3ej3LV71Q0GSVqalbTzy99E5eq3TNM_Xrb30QbCUy0CYaoTaetAoIQ13fJ-WrIWovm2=w682-h984-no?authuser=0)
#### The translation and rotation errors over different distance segment
![](https://lh3.googleusercontent.com/y-UtdrDdi7BnH2KPBb_cZKSmESmdhCQckg0vuTvdjvbQhJorMHbfNIc-ttkPNZIEC-R37Z0yu8ccHfFiCd1bV3zkTW3vZB7VooGEct6flOCvzxRLH96Ohesv_Lp-05zhzX_K7ArDL2aUFQAKwjbqxjjgL9QYWrViCwb6Qa9x2nHBQ1lyKlGoF9fqpg-b3WF8RYYN7DcvmRexoaVO9H02Vf9f1OCo3KHPXM1Al1zfUdTUkE9swudF_mwINpxxi2KuZAZsvqg2cztE60UnUwIIt0BDOkf5vN_Imcec4URypr-M9FCxmIGNhHNwOCqR7U35FeV_p0vBJJ2P5lfKL3sa4joX_RCfGl8cmmGwQ_tTXPxkPk_s7GnKGnhK-JClzBf2v8jzSbgpzjjCvHT_8MkQJGfNLyBaVGYtQfKVedG4_cjn9xIz-P272mUH_xWbNa9yqY2G-uYrrLKfEdUM1ZdqCMFkFk66AsLNmciYpMJmdVd6Ic_mtURzOnTZ00B26nmBi9sSWbqAxxLGPngg-nZTg6zC_yc_g61VP7Ac1oNj8fV6kSrNzAGIpdn3EPdI2FYcjd0DjPel8TkE2ugCn4djAlLe-vGmq8qqMNkbEpjbvgpoT-_yD-uipEy4Jfv71wbPM0jojMn2RCu5wUUp5V3WMVcQr_rCAhRQEYyf0ZFgDv7TFMe48pRsm-hiY3Qo=w720-h1040-no?authuser=0)
