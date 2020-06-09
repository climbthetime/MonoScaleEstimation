## Simple and Effective Scale Estimation Using Multiple Keyframes for Monolcuar Visual Odometry
Additional experimental results for the paper titled above.
### Abstract
In large scale environments, scale drift is a crucial problem of monocular visual SLAM. A common solution is to utilize the camera height, which can be obtained using the reconstructed 3D ground points~(3DGPs) from two successive frames, as prior knowledge.Increasing the number of 3DGPs by using more proceeding frames can be a natural extension of this solution to estimate a more precise camera height. However, merely employing multiple frames based on conventional methods is hard to be directly applicable in a real-world scenario because the vehicle motion and inaccurate feature matching inevitably cause large uncertainty and noisy 3DGPs. In this study, we propose an elaborate method to collect confident 3DGPs from multiple frames for robust scale estimation. First, we gather 3DGP candidates that can be seen in more than a predefined number of frames. To verify the 3DGP candidates, we filter out the 3D points at the exterior of the road region obtained by the deep-learning-based road segmentation model. In addition, we formulate an optimization problem constrained by a simple but effective geometric assumption that the normal vector of the ground plane lies in the null space of a movement vector of the camera center, and provide a closed-form solution. ORB-SLAM with the proposed scale estimation method achieves the average translation error with 1.19\% on the KITTI dataset, which outperforms the state-of-the-art conventional monocular visual 

*****************************************************************************************
#### Example of ATE results obtained using SEMK and GCSEMK for the sequences 00, 02-10.
![](https://lh3.googleusercontent.com/n5Ut3JwguSRFr7uCYuEJqw0wYJfzQPj8mSiginAxSnTXkjCOJ-CwRxn5M7CWVrlS-gp7VfPxlYVtJqCNgWFrnk7XFDV8AIebuXGHr7AXQwGW15VIQlVRPAJ4yrMjsrCRArvp2bk0UNmVal7_ycm7Qy2GMk6KUG9NeR9WOqcsQVUYFrJTIT2nAo2e1h6e_9phJ3XHuBMoK8zNNFSta31jHfsb7meVkDNvlNg1OhV-3fNnp-WAfYCCOdtzrvE6MzvA_MUWoYofPJjKgSAg0e7E-Yu2d1rz_xJ8k1mEoiBqE8pfm5dxgob0Syg6zGdZsRhK9QLutAd9wM8S5AvJNwtkq7lC1CpVtS1ApVQuF5eij04MQMu1QlbEn1WjFaRvrwqIrzMFHlfzYV1STYAX_Y7tqs_xJ9CBwyR52nnEu3p0XeXjw1DAMQd7zXYfwJigtMKKdxumBUzYSywdMC1Oxwor0mut6AgK2M0R3DZEkUnfcDA-wEi2ra_VbGzNs8osSpZ7UrChv2tBBc79IaSmu3rb9HPHZ5QuwVeoW2zPzAbvS6DfY1rf1nQ5jwYDWqOgghqU3-0v7E0TqS2Fg2GcjVFwcxkc3zDTdWL3_yKuJ9EPM4cynqvnWf2GrFTD6lWsrPG9Ew10zl-evd4X5JHV6UHmxL2jl5qzB86-QkakCmuTiM3SjFiXz8DZkLsTRZ3t=w694-h999-no?authuser=0)

*****************************************************************************************
#### Recorded video for sequence 00, 02-10. The trajectory of ground truth, ORB-SLAM without loop closure and GCSEMK are shown in red, black, and blue respectively. The black sparse points are the reconstructed 3D points. The detected feature points on the ground region are shown as red square in the image.
##### Recorded video for sequence 00
will be available soon
##### Recorded video for sequence 02
will be available soon
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
will be available soon

